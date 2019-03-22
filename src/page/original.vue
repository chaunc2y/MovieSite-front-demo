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
import Container from '../components/original/container.vue'
import Footer from '../components/index/footer.vue'
export default {
  components: {
    Header,
    Nav,
    Container,
    Footer
  }
}
</script>

