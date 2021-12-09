<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
export default {
  name: 'App',
  components: {
   Header,
   Main,
   Footer,
  }
}
</script>

<style lang="scss">
*{
   margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Montserrat', sans-serif;
}
#app {
  width: 80%;
  margin: 0 auto;
}
.btn{
      padding: 10px 8px;
      font-weight: 500;
      cursor: pointer;
      color: #fff;
      background-color: #377dff;
      border: 0;
      border-radius: 5px;
      &:hover{
          background-color: #1e1e1e;
      }
  }
</style>
