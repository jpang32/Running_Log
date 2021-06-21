<template>
    <div class="grow">
        hello
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

.grow-enter {
    transition: all .2s ease-in-out;
}
.grow:hover {
    transition: scale(1.1);
}


</style>