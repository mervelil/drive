<template>
  <div id="ServiceSelectSmall">
    <div class="w-full rounded-2xl bg-custom-color custom-height relative">
          <div class= "absolute top-1/3 left-1/3 transform -translate-x-1/4 -translate-y-1/4  mt-0.5 ">
            <img width="55" :src="'img/icons/uber/'+image+'.png'" alt="">
          </div>
     
      
    </div>
     
    <div class="text-xs mt-2 text-center text-gray-900 ">
              {{text}}
          </div>
  </div>
</template>
<script setup>
   import { defineProps, toRefs } from 'vue'
   const props=defineProps({
    text:String,
    image:String,
    promo:{Boolean,default:false}
   })
   const { text,image}=toRefs(props)
</script>
<style lang="scss" scoped>
 #ServiceSelectSmall{
  .bg-custom-color {
    background-color: rgb(237, 237, 237);
  }
  .custom-height{
    height: 70px;
  }
 }
</style>
