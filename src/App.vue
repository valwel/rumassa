<template>
  <div class="wrapper">
    <header-comp></header-comp>
  </div>
</template>

<script>
import HeaderComp from '@/components/HeaderComp.vue'

export default {
  name: 'app',
  components: {
    HeaderComp
  }
}
</script>

<style lang="scss">
* {
  list-style: none;
  font-family: 'Gothic A1 Regular';
  margin: 0;
  padding: 0;
}

html {
  background-color: #f5f5f5;
}

</style>
