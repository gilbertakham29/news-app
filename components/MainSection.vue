
   
      <template>
    <div class="col-span-1">
            <h2 class="text-3xl text-black font-normal">Home news: 26</h2>
            <div class=" mb-4 p-3 w-fit bg-white border border-gray-200 rounded-lg"  v-for="news in newsArticles" :key="news._id">
                <div class="flex flex-row justify-between items-center">
                    <div class="flex flex-row justify-between items-center p-2">
                        <img class="border rounded-full h-16 w-16" :src=" news.author.img " alt="person">
                        <div class="mx-2">
                            <p class="text-xs text-black font-light">{{ news.author.name }}</p>
                            <p class="text-xs text-black font-light">2022-08-24 17:27:34</p>
                        </div>
                    </div>
                    <div class="flex flex-row justify-between items-center">
                        <svg class="w-4 h-4 mx-1 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 20">
    <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 19-6-5-6 5V2a1 1 0 0 1 1-1h10a1 1 0 0 1 1 1v17Z"/>
  </svg>
  <svg class="w-4 h-4 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 18 18">
    <path d="M14.419 10.581a3.564 3.564 0 0 0-2.574 1.1l-4.756-2.49a3.54 3.54 0 0 0 .072-.71 3.55 3.55 0 0 0-.043-.428L11.67 6.1a3.56 3.56 0 1 0-.831-2.265c.006.143.02.286.043.428L6.33 6.218a3.573 3.573 0 1 0-.175 4.743l4.756 2.491a3.58 3.58 0 1 0 3.508-2.871Z"/>
  </svg>
                    </div>
                </div>
                <div class="flex flex-col justify-center items-center border-t-2">
                    <h5 class="text-lg font-normal text-black mt-3">{{ news.title }}</h5>
                </div>
                <img class=" w-max object-contain" :src=" news.image_url " alt="news">
            
                <p class=" line-clamp-3">
                    <span class=" overflow-ellipsis">
                        {{ news.details }}
                       
                    </span>
                </p>
                <div>
                    <NuxtLink :to="`/news/${news._id}`" class="text-blue-500">Read more</NuxtLink>

                </div>
                <div class="flex flex-row justify-between items-center border-t-2">
                <div class="flex flex-row justify-between items-center">
            <svg class="w-4 h-4 text-yellow-300 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
    <path d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"/>
  </svg>
  <span class="mx-1">{{ news.rating.number }}</span>
</div>
  <div class="flex flex-row justify-between items-center">
    <svg class="w-4 h-4 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 14">
    <g stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
      <path d="M10 10a3 3 0 1 0 0-6 3 3 0 0 0 0 6Z"/>
      <path d="M10 13c4.97 0 9-2.686 9-6s-4.03-6-9-6-9 2.686-9 6 4.03 6 9 6Z"/>
    </g>
  </svg>
  <span class="mx-1">{{ news.total_view }}</span>
  </div>
        </div>
            </div>
           
        </div>
</template>
<script>
import axios from 'axios'
export default{
    data(){
        return{
            newsArticles:[],
            categoryNews:[],
            dynamicRoute:""
        }
    },
    mounted() {
    this.fetchNews();
   
  },
    methods:{
        
        fetchNews(){
            const apiUrl = 'https://news-365-server.vercel.app/news/'
            axios.get(apiUrl).then(response => this.newsArticles = response.data)
            .catch(error => {
        console.error('Error fetching news:', error);
       console.log(this.newsArticles._id);
      });
     
        },
        
        
    }
}

</script>


       
       
       
    




<style scoped>

</style>