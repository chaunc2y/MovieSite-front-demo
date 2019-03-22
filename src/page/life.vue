<template>
  <div>
    <Header></Header>
    <Nav/>
    <container/>
    <Footer></Footer>
  </div>
</template>
<script>
import Header from '../components/index/header.vue'
import Nav from '../components/index/nav.vue'
import Footer from '../components/index/footer.vue'
import Container from '../components/life/container.vue'
export default {
  components: {
    Header,
    Nav,
    Container,
    Footer
  }
}
</script>

