<template>
  <div class="container">
    <h1 class="mt-4 mb-3 text-center">个人中心</h1>
    <div class="userinfo-box g-my-30">
      <form name="sentMessage" id="contactForm" novalidate>
        <!-- File Button 头像-->
        <div class="form-group row g-mt-15">
          <label class="col-2 col-form-label text-right" for="filebutton">头像</label>
          <div class="col-md-4">
            <input id="filebutton" name="filebutton" class="input-file" type="file">
          </div>
        </div>

        <!-- Multiple Radios (inline) 性别-->
        <div class="form-group row g-mt-15">
          <label class="col-2 col-form-label text-right" for="radios">性别</label>
          <div class="col-md-5">
            <label class="radio-inline mr-5" for="radios-0">
              <input type="radio" name="radios" id="radios-0" value="1" checked="checked">
              男
            </label>
            <label class="radio-inline mr-5" for="radios-1">
              <input type="radio" name="radios" id="radios-1" value="2">
              女
            </label>
            <label class="radio-inline" for="radios-2">
              <input type="radio" name="radios" id="radios-2" value="3">
              保密
            </label>
          </div>
        </div>

        <!-- Text input 用户名-->
        <div class="form-group row g-mt-15">
          <label class="col-2 col-form-label text-right" for="textinput">用户名</label>
          <div class="col-md-10">
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

        <!-- Text input 密码-->
        <div class="form-group row g-mt-15">
          <label class="col-2 col-form-label text-right" for="textinput">密码</label>
          <div class="col-md-10">
            <input
              id="pwd"
              name="textinput"
              type="text"
              placeholder="placeholder"
              class="form-control input-md"
              required
              data-validation-required-message="Please enter your password."
            >
            <p class="help-block"></p>
          </div>
        </div>

        <!-- Text input 邮箱-->
        <div class="form-group row g-mt-15">
          <label class="col-2 col-form-label text-right" for="textinput">邮箱</label>
          <div class="col-md-10">
            <input
              id="email"
              name="textinput"
              type="text"
              placeholder="placeholder"
              class="form-control input-md"
              data-validation-required-message="Please enter your E-mail."
            >
            <p class="help-block"></p>
          </div>
        </div>

        <!-- Appended checkbox 手机-->
        <div class="form-group row g-mt-15">
          <label class="col-2 col-form-label text-right" for="appendedcheckbox">手机</label>
          <div class="col-md-8">
            <div class="input-group">
              <input
                id="phone"
                name="appendedcheckbox"
                class="form-control"
                type="text"
                placeholder="placeholder"
                data-validation-required-message="Please enter your phone."
              >
              <span class="input-group-addon btn-mk2 primary" id="get-phone-captcha">
                <button class="btn bg-info">验证码</button>
              </span>
            </div>
            <p class="help-block"></p>
          </div>
        </div>

        <!-- Appended checkbox 确认验证码-->
        <div class="form-group row g-mt-15">
          <label class="col-2 col-form-label text-right" for="appendedcheckbox">手机验证码</label>
          <div class="col-md-8">
            <div class="input-group">
              <input
                id="appendedcheckbox"
                name="appendedcheckbox"
                class="form-control"
                type="text"
                placeholder="placeholder"
              >
              <span class="input-group-addon btn-mk2 primary" id="get-phone-captcha">
                <button class="btn bg-info">确&nbsp;&nbsp;&nbsp;&nbsp;认</button>
              </span>
            </div>
            <p class="help-block"></p>
          </div>
        </div>

        <!-- Select Basic 地区-->
        <div class="form-group row g-mt-15">
          <label class="col-2 col-form-label text-right" for="selectbasic">地区</label>
          <div class="col-md-8">
            <select id="selectbasic" name="selectbasic" class="form-control">
              <option value="1">Option one</option>
              <option value="2">Option two</option>
            </select>
          </div>
        </div>

        <div id="success"></div>
        <!-- For success/fail messages -->
        <div class="form-group row g-mt-45">
          <label for="example-text-input" class="col-2 col-form-label text-right"></label>
          <div class="col-10">
            <button type="submit" class="btn btn-primary" id="sendMessageButton">保存</button>
          </div>
        </div>
      </form>
    </div>
  </div>
</template>