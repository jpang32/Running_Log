<template>
  <div class='visible' @mouseover='hover=true' @mouseleave='hover=false' v-bind:class='{ hidden : hover }'>
     <p v-if='hover'> {{ info }} </p>
     <p v-else class='title'> {{ title }} </p>
  </div>
</template>

<script>

    export default {
      name: 'Card',
      props: {
        info: String,
        title: String
      },
      data: function() {
        return {
          hover: false
        }
      }
    }
  
</script>

<style scoped>

.slide-enter {
  width: 400px;
  height: 300px;
  border: 6px solid rgb(216, 214, 214);
  border-radius:25px;
  background-color: rgb(216, 214, 214);
  padding-top: 50px;
  padding-bottom: 50px;

}
.visible {
  width: 400px;
  height: 300px;
  border: 6px solid rgb(10, 191, 204);
  border-radius: 25px;
  background-color: rgb(205, 240, 245);
  
}
.hidden {
  width: 400px;
  height: 300px;
  border: 6px solid rgb(216, 214, 214);
  border-radius:25px;
  background-color: rgb(216, 214, 214);
  
}

.title {
  font: bold 30px Arial, sans-serif;
  color: rgb(168, 128, 231);
  text-align: center;
  vertical-align: middle;
}

</style>