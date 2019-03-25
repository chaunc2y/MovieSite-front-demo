<template>
  <div>
    <Nav/>
    <div class="g-pb-100">
      <div class="page-content">
        <div class="user-head">
          <div class="container">
            <div class="row">
              <div class="col-sm-6 pl-5 pt-4">
                <div class="name g-font-weight-600">
                  -陈颠颠
                  <a href="/member/userinfo" data-cl-id="2566565420">
                    <i class="icon icon-edit-file g-font-size-20"></i>
                  </a>
                </div>
                <div class="city"></div>
                <div class="info mt-4 g-font-weight-500">
                  <div class="count-box">
                    <p class="number">0</p>
                    <p class="box-name">获赞</p>
                  </div>
                  <div class="count-box">
                    <p class="number">0</p>
                    <p class="box-name">关注</p>
                  </div>
                  <div class="count-box">
                    <p class="number">0</p>
                    <p class="box-name">粉丝</p>
                  </div>
                </div>
              </div>
              <div class="col-sm-6 pr-5 pt-4 text-right">
                <img
                  src="http://thirdwx.qlogo.cn/mmopen/vi_32/jgGAmAeGDJVUw9TlSltm7TMtyLRxReCMkgblbZC7Do8SlgXLs6FibFntqxPz7KOsEJicmDDHk5espnm8pys5dsOA/132?x-oss-process=style/head-pic-1x"
                  class="user-pic"
                >
              </div>
              <div class="introduction g-font-weight-600 mt-3 ml-5">
                简介：
                <a href="/member/userinfo" data-cl-id="2566565420">
                  <i class="icon icon-edit-file g-font-size-20"></i>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container" style="margin-top: 30px;">
      <div class="row">
        <!-- Sidebar Column -->
        <div class="col-lg-2 mb-4">
          <div class="list-group">
            <Router-link to="/member/contribute" class="list-group-item">视频投稿</Router-link>
            <Router-link to="/member/manager" class="list-group-item list-group-item active">作品管理</Router-link>
          </div>
        </div>
        <!-- Content Column -->
        <div class="col-lg-10 mb-4">
          <h2>作品管理</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta, et temporibus, facere perferendis veniam beatae non debitis, numquam blanditiis necessitatibus vel mollitia dolorum laudantium, voluptate dolores iure maxime ducimus fugit.</p>
        </div>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>
<script>
import Nav from '../components/index/nav.vue'
import MainPage from '../components/memberindex/mainpage.vue'
import Follow from '../components/memberindex/follow.vue'
import Fans from '../components/memberindex/fans.vue'
import Collect from '../components/memberindex/collect.vue'
import Footer from '../components/index/footer.vue'
export default {
  components: {
    Nav,
    MainPage,
    Follow,
    Fans,
    Collect,
    Footer
  }
}
</script>