<script >
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';
import productCard from './components/productCard.vue';

export default{
  name:'App',
  components:{
    Header,
    Main,
    Footer
  }
}

</script>

<template>
  <Header></Header>
  <Main></Main>
  <Footer></Footer>
</template>

<style lang="scss">
@use './sass/main.scss';

</style>
