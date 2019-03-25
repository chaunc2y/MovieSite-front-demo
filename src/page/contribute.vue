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
            <Router-link to="/member/contribute" class="list-group-item list-group-item active">视频投稿</Router-link>
            <Router-link to="/member/manager" class="list-group-item">作品管理</Router-link>
          </div>
        </div>
        <!-- Content Column -->
        <div class="col-lg-10 mb-4">
          <h2>视频投稿</h2>
          <!-- Text input 用户名-->
          <div class="form-group row mt-4">
            <label class="col-1 col-form-label" for="textinput">用户名</label>
            <div class="col-md-8">
              <input
                id="name"
                name="textinput"
                type="text"
                placeholder="placeholder"
                class="form-control input-md"
                required
                data-validation-required-message="Please enter your name."
              >
              <p class="help-block"></p>
            </div>
          </div>
          <!-- Select Basic 地区-->
          <div class="form-group row mt-3">
            <label class="col-1 col-form-label" for="selectbasic">类型</label>
            <div class="col-md-4">
              <select id="selectbasic" name="selectbasic" class="form-control">
                <option value="1">Option one</option>
                <option value="2">Option two</option>
              </select>
            </div>
          </div>
          <!-- Text input 简介-->
          <div class="form-group row mt-4">
            <label class="col-1 col-form-label" for="textinput">简介</label>
            <div class="col-md-8">
              <textarea class="form-control" rows="3"></textarea>
            </div>
          </div>
          <!-- Text input 封面-->
          <div class="form-group row mt-4">
            <label class="col-1 col-form-label" for="textinput">封面</label>
            <div class="col-md-4">
              <input
                id="userIDImageBack"
                type="file"
                class="file"
                data-preview-file-type="text"
                required
                name="imgPath"
              >
              <p class="help-block"></p>
            </div>
            <div class="col-md-4">
              <img class="col-sm-8" src="/static/images/img13.jpg" alt="样图">
            </div>
          </div>
          <!-- Text input 视频-->
          <div class="form-group row mt-4">
            <label class="col-1 col-form-label" for="textinput">视频</label>
            <div class="col-md-8">
              <input
                id="userIDVideoBack"
                type="file"
                class="file"
                data-preview-file-type="text"
                required
                name="videoPath"
              >
              <p class="help-block"></p>
            </div>
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
  },
  data() {
    return {
      impUploadAPI: '',
      videoUploadAPI: ''
    }
  }
}
</script>