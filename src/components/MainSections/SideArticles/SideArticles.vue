<template>
  <div class="sideArticles">
    <div class="sideArticle" v-for="(element,index) in allSideArticles" :key="index">
      <div>
        <img :src="require(`@/assets/project_images/${element.image}`)"> 
      </div>
      <div>
        <a href="#">{{element.link}}</a>
        <p>{{element.text}}</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'SideArticles',
    data(){
      return{
        allSideArticles: [
          {
            image: 'photo-1444664597500-035db93e2323-177x142.jpg',
            link: 'The human story of uniqueness',
            text: 'lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum'
          },
  
          {
            image: 'photo-1447430617419-95715602278e-177x142.jpg',
            link: 'Sustainable trade tactics',
            text: 'lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum'
          },
  
          {
            image: 'photo-1460230525622-630fe3294cd7-177x142.jpg',
            link: 'Farmers making a difference',
            text: 'lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum'
          },
  
          {
            image: 'photo-1460600421604-5e138c208b9c-177x142.jpg',
            link: 'Meeting remote tribes in Peru',
            text: 'lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum'
          }
        ]
      }
    }
  }
</script>

<style lang="scss">
</style>