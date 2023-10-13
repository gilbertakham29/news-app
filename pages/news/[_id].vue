<template>

    <div class="col-span-1" >
     <div>

           <div class="  w-fit bg-white border border-gray-200 rounded-lg"  :key="categoryNews._id">
               
               
               <img class=" w-max object-contain" :src=" categoryNews.image_url " alt="news">
               <div class="flex flex-col justify-center items-center border-t-2">
                   <h5 class="text-lg font-semibold text-black mt-3">{{ categoryNews.title }}</h5>
               </div>
               <p class=" ">
                   <span class=" ">
                       {{ categoryNews.details }}
                      
                   </span>
               </p>
               <NuxtLink :to="`/category/${categoryNews.category_id}`">
                <button type="button" class="text-white mt-3 bg-blue-500 hover:bg-blue-600 focus:ring-4 focus:ring-blue-300 font-normal rounded-lg text-sm px-12 py-2.5 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 focus:outline-none dark:focus:ring-blue-800">All News In This Category</button>
               </NuxtLink>
             
           </div>
         
       </div>
     </div>
</template>

<script >
import axios from 'axios'

export default{
  
   data(){
       return{
           
           categoryNews:[],
           
           
       }
   },
   mounted() {
   this.fetchNews();
 },
   methods:{
       
       fetchNews(){
          
           const {_id} = useRoute().params
           const newsItemUrl = `https://news-365-server.vercel.app/news/${_id}`
           
     axios.get(newsItemUrl).then(response => this.categoryNews = response.data).catch(error => {
       console.error('Error fetching news:', error);
     })
   
       },
       
   }
}
</script>

<style lang="scss" scoped>

</style>