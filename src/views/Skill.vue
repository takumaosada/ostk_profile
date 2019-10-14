<template>
  <div class="root">
    <main class="main bg-vue shadow-large rounded">
      <div class="container-fluid">
        <h3>LANGUAGES</h3>
        <div class="row">
          <div class="col-12 p-0 col-sm-7">
            <div class="py-2">
              <h5>MARK UP</h5>
              <ul class="mb-1">
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-html5-plain-wordmark lang-icon"></i>
                </li>
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-css3-plain-wordmark lang-icon"></i>
                </li>
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-bootstrap-plain-wordmark lang-icon"></i>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-12 p-0 col-sm-5">
            <div class="py-2">
              <h5>BACK END</h5>
              <ul class="mb-1">
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-rails-plain-wordmark lang-icon"></i>
                </li>
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-ruby-plain-wordmark lang-icon"></i>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-12 p-0 col-sm-7">
            <div class="py-2">
              <h5>FRONT END</h5>
              <ul class="mb-1">
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-vuejs-plain-wordmark lang-icon"></i>
                </li>
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-jquery-plain-wordmark lang-icon"></i>
                </li>
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-javascript-plain lang-icon"></i>
                </li>
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-coffeescript-original-wordmark lang-icon"></i>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-12 p-0 col-sm-5">
            <div class="py-1">
              <h5>APP</h5>
              <ul class="mb-2">
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-swift-plain lang-icon"></i>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-12 p-0 col-sm-7">
            <div class="py-1">
              <h5>INTERESETED IN</h5>
              <ul class="mb-2">
                <li class="rounded-circle px-3 pt-3">
                  firebase
                </li>
                <li class="rounded-circle px-3 pt-3">
                  flutter
                </li>
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-android-plain-wordmark lang-icon"></i>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-12 p-0 col-sm-5">
            <div class="py-1">
              <h5>LOVE</h5>
              <ul class="mb-2">
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-swift-plain lang-icon"></i>
                </li>
                <li class="rounded-circle px-3 pt-3">
                  <i class="devicon-apple-original lang-icon"></i>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'Root',
  data () {
    return {
      baseClass: 'v-icon',
    }
  },
  methods: {
    info_path: function (url) {
      return url
    }
  }
}
</script>

<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.license {
  color: black;
}
.license a {
  color: #2c3e50;
}
.v-icon, .custom-icon {
  width: 24px;
}
.lang-icon {
  font-size: 4rem
}
.bg-vue {
  background-color:#42b983
}
</style>