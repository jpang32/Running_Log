<template>
  <div>
    <FeedScroll></FeedScroll>
    <FeedFilter></FeedFilter>
  </div>
</template>
  
<script>
  
  import FeedFilter from './FeedFilter.vue'
  import FeedScroll from './FeedScroll.vue'
    
  export default {
    name: 'Main',
    components: {
      FeedFilter,
      FeedScroll
    },
    props: {
      msg: String
    }
  }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .container {
  width: 500px;
  height: 300px;
  border: 6px solid rgb(216, 214, 214);
  border-radius:25px;
  background-color: rgb(216, 216, 214);
}

  
  
</style>