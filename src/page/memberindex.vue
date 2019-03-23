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
    <div class="container">
      <div class="user-tab mt-4 mx-auto">
        <ul class="nav nav-tabs nav justify-content-center">
          <li role="presentation" class="nav-item">
            <a class="nav-link active" data-toggle="tab" href="#home">主页</a>
          </li>
          <li role="presentation" class="nav-item">
            <a class="nav-link" data-toggle="tab" href="#follow">关注</a>
          </li>
          <li role="presentation" class="nav-item">
            <a class="nav-link" data-toggle="tab" href="#fans">粉丝</a>
          </li>
          <li role="presentation" class="nav-item">
            <a class="nav-link" data-toggle="tab" href="#collect">收藏</a>
          </li>
        </ul>
        <!-- Tab panes -->
        <div class="tab-content">
          <div id="home" class="container tab-pane active">
            <br>
            <h4>HOME</h4>
            <main-page/>
          </div>
          <div id="follow" class="container tab-pane fade">
            <br>
            <h3>关注</h3>
            <Follow/>
          </div>
          <div id="fans" class="container tab-pane fade">
            <br>
            <h3>粉丝</h3>
            <Fans/>
          </div>
          <div id="collect" class="container tab-pane fade">
            <br>
            <h3>收藏</h3>
            <Collect/>
          </div>
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