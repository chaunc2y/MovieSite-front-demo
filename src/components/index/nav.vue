<template>
  <!-- Navigation -->
  <nav class="navbar fixed-top navbar-expand-lg navbar-light nav-transparent bg-white fixed-top">
    <div class="container">
      <a class="navbar-brand" href="/index">Mars</a>
      <button
        class="navbar-toggler navbar-toggler-right"
        type="button"
        data-toggle="collapse"
        data-target="#navbarResponsive"
        aria-controls="navbarResponsive"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarResponsive">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdownPortfolio"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >动态</a>
            <div
              class="dropdown-menu dropdown-menu-right"
              aria-labelledby="navbarDropdownPortfolio"
            >
              <a class="dropdown-item" href="portfolio-1-col.html">回复我的</a>
              <a class="dropdown-item" href="portfolio-2-col.html">收到的赞</a>
              <a class="dropdown-item" href="portfolio-3-col.html">我的动态</a>
            </div>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdownBlog"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >ME</a>
            <div class="dropdown-menu dropdown-menu-right" aria-labelledby="navbarDropdownBlog">
              <Router-link class="dropdown-item" to="/member/user">个人主页</Router-link>
              <a class="dropdown-item" href="blog-home-2.html">投稿管理</a>
              <Router-link class="dropdown-item" to="/member/settings">个人中心</Router-link>
              <a class="dropdown-item" href="blog-post.html">退出</a>
            </div>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="contact.html">收藏</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>