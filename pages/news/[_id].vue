<template>

    <div class="col-span-1" >
     <div>

           <div class="  w-fit bg-white border border-gray-200 rounded-lg"  :key="categoryNews._id">
               
               <div class="flex flex-col justify-center items-center border-t-2">
                   <h5 class="text-lg font-normal text-black mt-3">{{ categoryNews.title }}</h5>
               </div>
               <img class=" w-max object-contain" :src=" categoryNews.image_url " alt="news">
           
               <p class=" ">
                   <span class=" ">
                       {{ categoryNews.details }}
                      
                   </span>
               </p>
               
             
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