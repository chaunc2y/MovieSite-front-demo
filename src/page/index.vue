<template>
  <div>
    <Header></Header>
    <Nav/>
    <Swiper/>
    <Container/>
    <div class="article_list">
      <ul>
        <li v-for="i in list">
          <time v-text="$utils.goodTime(i.create_at)"></time>
          <router-link :to="'/content/' + i.id">{{ i.title }}</router-link>
        </li>
      </ul>
    </div>
    <Footer></Footer>
  </div>
</template>
<script>
import Header from '../components/index/header.vue'
import Footer from '../components/index/footer.vue'
import Nav from '../components/index/nav.vue'
import Swiper from '../components/index/swiper.vue'
import Container from '../components/index/container.vue'
export default {
  components: { Header, Footer, Nav, Swiper, Container },
  data() {
    return {
      list: []
    }
  },
  created() {
    this.getData()
  },
  methods: {
    getData() {
      this.$api.get('topics', null, r => {
        this.list = r.data
      })
    }
  }
}
</script>
