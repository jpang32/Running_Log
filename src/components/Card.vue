<template>
    <div class="grandparent" @mouseover="hover=false" @mouseleave="hover=true">
        <div class="parent" v-if="hover">
          <div class="green"></div>
        </div>
        <div class="parent" v-else>
          <div class="red"></div>
        </div>
    </div>
</template>

<script>

    export default {
      name: 'Card',
      data: function() {
        return {
          hover: true
        }
      }
      
    }
  
</script>

<style scoped>

.grandparent {
  width: 500px;
  height: 300px;
}

.parent {
  width: 100%;
  height: 100%;
}

.green {
  width: 100%;
  height: 100%;
  background-color: rgb(10, 204, 42);
}
.red {
  width: 100%;
  height: 100%;
  background-color: rgb(231, 24, 9);
}

</style>