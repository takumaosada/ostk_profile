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
        <li v-for="(icon, index) in icons" :key="index" class="rounded-circle p-3">
          <a :href="icon.url" :aria-label="icon.label">
            <feather :type="icon.icon" stroke="black"></feather>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        icons: [
          {
            'url': 'https://www.facebook.com/takuma.osada.10?ref=bookmarks',
            'label': 'facebook',
            'icon': 'facebook'
          },
          {
            'url': 'https://twitter.com/ostk0069',
            'label': 'twitter',
            'icon': 'twitter'
          },
          {
            'url': 'https://github.com/takumaosada',
            'label': 'github',
            'icon': 'github'
          },
          {
            'url': 'https://www.wantedly.com/users/31623094',
            'label': 'wantedly',
            'icon': 'user-plus'
          },
          {
            'url': 'https://qiita.com/ostk0069',
            'label': 'qiita',
            'icon': 'pen-tool'
          }
        ]
      };
    }
  };
</script>

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
