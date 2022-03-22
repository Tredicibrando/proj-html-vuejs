<template>
  <div id="app">
    <MyBar />
    <MyHeader />
    <MyMain />
  </div>
</template>

<script>
import MyHeader from '@/components/MyHeader.vue'
import MyBar from '@/components/MyBar.vue'
import MyMain from '@/components/MyMain.vue'

export default {
  name: 'App',
  components: {
    MyBar,
    MyHeader,
    MyMain,
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

ul,ol{
  list-style: none;
}

a{
  text-decoration: none;
  color: currentColor;
}

#app {
  font-family: 'Montserrat', sans-serif;

}
</style>
