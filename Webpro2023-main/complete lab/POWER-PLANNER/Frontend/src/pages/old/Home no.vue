<template>
    <div class="bg-white">
      <CarouselBar />
      <ListBook />
    </div>
  </template>


  <script>
  import Navbar from '../../components/old/Navbar old.vue'
  import ListBook from '../../components/old/ListBook.vue'

  import CarouselBar from '../../components/old/CarouselBar.vue'

  export default {
    name: 'App',
    data(){
      fav  : []
  },
  created(){
                this.fav=  JSON.parse(localStorage.getItem("book"))
                this.userdata=  JSON.parse(localStorage.getItem("userdata"))
    },
    components: {
      Navbar,
      ListBook,
      CarouselBar

    },
    computed: {
    },
  }
  </script>
  <style scoped>

  </style>
