<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/skill">Skill</router-link>
      <router-link to="/timeline">Timeline</router-link>
    </div>
    <router-view/>
    <div class="container mt-5">
      <ul class="list-inline mb-5">
        <li class="bg-dark rounded-circle p-3 mt-3">
          <a class="text-white" href="https://www.facebook.com/takuma.osada.10?ref=bookmarks">
            <custom-icon name="facebook" base-class="custom-icon"></custom-icon>
          </a>
        </li>
        <li class="bg-dark rounded-circle p-3 mt-3">
          <a class="text-white" href="https://twitter.com/ostk0069">
            <custom-icon name="twitter" base-class="custom-icon"></custom-icon>
          </a>
        </li>
        <li class="bg-dark rounded-circle p-3 mt-3">
          <a class="text-white" href="https://github.com/takumaosada">
            <custom-icon name="github" base-class="custom-icon"></custom-icon>
          </a>
        </li>
        <li class="bg-dark rounded-circle p-3 mt-3">
          <a class="text-white" href="https://www.wantedly.com/users/31623094">
            <custom-icon name="message-circle" base-class="custom-icon"></custom-icon>
          </a>
        </li>
        <li class="bg-dark rounded-circle p-3 mt-3">
          <a class="text-white" href="https://qiita.com/ostk0069">
            <custom-icon name="book-open" base-class="custom-icon"></custom-icon>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

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
