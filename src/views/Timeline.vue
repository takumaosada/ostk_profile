<template>
  <div class="root">
    <main class="main">
      <h3>TIMELINE</h3>
      <section class="timeline">
        <ul>
          <li v-for="(info, index) in timeline_data" v-bind:key="index">
            <span></span>
            <div>{{ info.title }}</div>
            <div>{{ info.description }}</div>
            <div><a :href="info_path(info.url)">{{ info.url | truncate(20) }}</a></div>
            <div class="year">
              <span>{{ info.yearEnd }}</span>
              <span>{{ info.yearStart }}</span>
            </div>
          </li>
        </ul>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: 'Root',
  data () {
    return {
      baseClass: 'v-icon',
      timeline_data: [
        {
          'title': 'JX通信社でiOSインターン',
          'description': ' News系アプリの開発',
          'url': 'https://newsdigest.jp/',
          'yearStart': '`19/02',
          'yearEnd': ''
        },
        {
          'title': '株式会社Freneticで受託開発',
          'description': '学生のみでの起業を経験。エンジニアリング領域以外にも触れる。',
          'url': 'https://gamepatch.gg/submissions/recommend',
          'yearStart': '`18/08',
          'yearEnd': ''
        },
        {
          'title': 'BLAMハッカソン',
          'description': '"ダサい大学生をコーディネート"するサービスを発表し審査員賞を２つ獲得',
          'url': '',
          'yearStart': '`18/11',
          'yearEnd': '`18/11'
        },
        {
          'title': 'ZENS株式会社でRailsインターン',
          'description': '外国人だけの開発チームでインターン',
          'url': 'https://www.zens.tokyo/',
          'yearStart': '`17/10',
          'yearEnd': '`18/07'
        },
        {
          'title': '学生団体UNITUSに所属する',
          'description': 'プログラミングに触れる。プロジェクトの立ち上げ、組織運用を経験',
          'url': 'http://www.unitus.tech/topics/blogs/osada_interview',
          'yearStart': '`17/04',
          'yearEnd': '`18/07'
        },
        {
          'title': '東京理科大学経営学部ビジネスエコノミクス学科に入学',
          'description': '',
          'url': '',
          'yearStart': '`17/04',
          'yearEnd': ''
        },
        {
          'title': '静岡県私立加藤学園暁秀高等学校特進科に入学',
          'description': '',
          'url': '',
          'yearStart': '`14/04',
          'yearEnd': '`17/03'
        },
        {
          'title': '静岡県市立三島南中学校に転校',
          'description': '',
          'url': '',
          'yearStart': '`14/04',
          'yearEnd': '`17/03'
        },
        {
          'title': 'ロッテルダム日本人学校に入学(小５〜中２)',
          'description': '',
          'url': 'https://www.jsrotte.nl/index.html',
          'yearStart': '`14/04',
          'yearEnd': '`17/03'
        },
        {
          'title': 'Regional International School in Eindhovenに転校(小２)',
          'description': '',
          'url': 'https://isecampus.nl/Flex/Site/Page.aspx?PageID=&Lang=',
          'yearStart': '`14/04',
          'yearEnd': '`17/03'
        }
      ]
    }
  },
  methods: {
    info_path: function (url) {
      return url
    }
  },
  filters: {
    truncate: function (value, length) {
      var lengthInt = length ? parseInt(length, 10) : 20
      if (!value) return ''
      if (value.length <= lengthInt) {
        return value
      } else {
        return value.substring(0, lengthInt) + '...'
      }
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