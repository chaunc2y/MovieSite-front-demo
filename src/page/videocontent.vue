<template>
  <div>
    <Nav/>
    <div class="bg-light">
      <div
        id="viewbox_report"
        class="container video-info report-wrap-module report-scroll-module pt-4 mb-4"
        scrollshow="true"
      >
        <div class="col-md-12">
          <h1 title="最全的vue.js视频【黑马程序员】" class="video-title">
            <!---->
            <span class="tit">最全的vue.js视频【黑马程序员】</span>
          </h1>
          <div class="video-data">
            <span class="a-crumbs">
              <Router-link target="_blank" to="/index">主页</Router-link>/
              <Router-link target="_blank" to="/tech">科技</Router-link>
            </span>
            <span>2018-11-24 16:44:21</span>
            <!---->
          </div>
          <div class="video-data">
            <span title="总播放数200381" class="view">20.0万播放&nbsp;&nbsp;</span>
            <span class="copyright">
              <i class="van-icon-info_prohibit"></i>未经作者授权，禁止转载
            </span>
            <!---->
          </div>
        </div>
      </div>
      <div class="container">
        <div class="pb-4">
          <video width="100%" height="100%" class="col-md-12 video-frame box-shadow" controls>
            <source src="/static/images/demo.mp4" type="video/mp4">
          </video>
        </div>
      </div>
    </div>
    <div class="container video-content-body">
      <div class="author-info">
        <div class="author-body col-md-12">
          <a
            target="_blank"
            href="/ta/index/guid/2aae7ff0-5925-21eb-5b46-09f0d2703718"
            data-cl-id="2122123489"
          >
            <div class="face">
              <img
                src="http://pic.topys.cn/attachments/avatars/000/19/30/45_avatar_big.jpg?x-oss-process=style/head-pic-min-1x"
                alt
                class="img-fluid"
              >
            </div>
            <div class="author-box">
              <div class="author-name">摇摇冻</div>
              <p class="add-time">2019-03-20 17:26</p>
            </div>
          </a>
          <div class="follow-div follow-tools pull-right text-right">
            <div class="circle-icon pointer-show">
              <i class="icon icon-e-add"></i>
            </div>
            <div class="circle-icon pointer-show g-ml-10">
              <i class="icon icon-comment"></i>
            </div>
          </div>
        </div>
      </div>
      <div class="video-praise-tools al-c">
        <div
          class="u-icon-v2 g-rounded-50 g-bg-primary g-color-white g-mb-10 pointer-show ripple-block up-btn detail-digg g-width-90 g-height-90"
        >
          <i class="icon icon-thumb-up g-font-size-30">
            <img src="/static/images/uncollect.png">
          </i>
        </div>
        <p class="praise-count">
          <span id="praise-count">27</span>人觉得很赞
        </p>
      </div>
      <div class="comment-add-box mt-60">
        <div class="media">
          <div class="d-flex mt-2 mr-5">
            <img
              src="http://thirdwx.qlogo.cn/mmopen/vi_32/jgGAmAeGDJVUw9TlSltm7TMtyLRxReCMkgblbZC7Do8SlgXLs6FibFntqxPz7KOsEJicmDDHk5espnm8pys5dsOA/132"
              class="comment-img rounded-circle ml-3"
            >
          </div>
          <div class="media-body">
            <textarea
              id="inputGroup2_1"
              rows="4"
              placeholder="发表评论..."
              class="form-control form-control-md g-resize-none rounded-0"
            ></textarea>
          </div>
        </div>
        <div class="text-right mt-3">
          <button class="btn bg-primary">发表</button>
        </div>
      </div>
      <div class="comment-list-box g-mt-30">
        <h2 class="h3 u-heading-v1__title g-mb-20">最新评论(1)</h2>
        <div class="comment-list">
          <ul class="list-unstyled">
            <li class="mt-3 mr-3 mb-3 ml-3 pt-4 pb-4 g-brd-y">
              <div class="media">
                <div class="d-flex mt-2 mr-5">
                  <a
                    href="/ta/index/guid/ea235b36-8b62-98dd-0e0b-21567d74ce6f"
                    target="_blank"
                    data-cl-id="1557724892"
                  >
                    <img
                      src="http://thirdwx.qlogo.cn/mmopen/vi_32/Q0j4TwGTfTL3vwNcs8LHPRGlmeDaxyJQeyfToMBsyB4wgAfV0YxTaZfrFqrKr4lWouEMyvr4PJ9BhsPfN0VHqg/132"
                      class="comment-img rounded-circle"
                    >
                  </a>
                </div>
                <div class="media-body">
                  <p class="m-0">
                    <a
                      href="/ta/index/guid/ea235b36-8b62-98dd-0e0b-21567d74ce6f"
                      target="_blank"
                      data-cl-id="418294253"
                    >
                      <strong>星星兜</strong>
                    </a>
                    <span class="g-font-size-12 g-color-gray g-ml-15">3天前</span>
                    <span class="pointer-show" style="float: right;">
                      <span
                        data-toggle="tooltip"
                        data-original-title="分享评论"
                        data-placement="bottom"
                        class="g-rounded-50 pointer-show g-mr-10"
                      >
                        <i class="icon icon-share-2"></i>
                      </span>
                      <span>
                        <i class="icon icon-thumb-up"></i>
                        <span class="g-mr-5">1</span>
                      </span>
                    </span>
                  </p>
                  <p>看完有点饿……</p>
                  <div class="comment-tools">
                    <div class="sub-icon pointer-show">
                      <i class="icon icon-chat-round-content g-font-16"></i> 回复ta
                    </div>
                    <!---->
                  </div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>
<script>
import Nav from '../components/index/nav.vue'
import Footer from '../components/index/footer.vue'
export default {
  components: {
    Nav,
    Footer
  }
}
</script>