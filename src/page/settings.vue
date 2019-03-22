<template>
  <div>
    <Nav/>
    <container/>
    <Footer></Footer>
  </div>
</template>
<script>
import Nav from '../components/index/nav.vue'
import Footer from '../components/index/footer.vue'
import Container from '../components/settings/container.vue'
export default {
  components: {
    Nav,
    Container,
    Footer
  }
}
</script>