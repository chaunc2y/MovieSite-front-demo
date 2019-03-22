<template>
  <div>
    <Header></Header>
    <Nav/>
    <Footer></Footer>
  </div>
</template>
<script>
import Header from '../components/index/header.vue'
import Nav from '../components/index/nav.vue'
import Footer from '../components/index/footer.vue'
export default {
  components: {
    Header,
    Nav,
    Footer
  }
}
</script>

