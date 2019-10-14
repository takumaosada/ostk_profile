<template>
  <div class="root">
    <div class="container text-center my-auto">
      <img class="rounded-circle" src="../assets/takumaosada.jpg" alt="takumaosada" width="140" height="140">
      <br>
      <br>
      <h3 class="mb-1 text-muted">Takuma Osada</h3>
      <h5 class="mb-5 text-secondary">
        <em class="license">{{ msg }}</em>
      </h5>
    </div>
    <main class="main bg-info shadow-large rounded">
      <h3>PROFILE</h3>
      <div class="container-fluid py-3">
        <div class="row">
          <div class="col-12 col-sm-5">
            <img class="rounded img-fluid" src="../assets/blamtaku.jpg" alt="blamtaku">
          </div>
          <div class="col-12 col-sm-7">
            <ul class="text-left">
              <li v-for="(info, index) in common_data" v-bind:key="index" class="m-0 container-fluid p-0">
                <div class="text-left pt-3 pb-3 pt-sm-0">
                  #{{ info.option }} {{ info.detail }}
                </div>
              </li>
            </ul>
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
      msg: 'iOS Engineer',
      baseClass: 'v-icon',
      common_data: [
        {
          'option': '名前',
          'detail': '長田 卓馬'
        },
        {
          'option': '大学',
          'detail': '東京理科大学経営学部ビジネスエコノミクス学科(21年卒)'
        },
        {
          'option': '研究',
          'detail': 'データ分析(安藤研究室)'
        },
        {
          'option': '何してる',
          'detail': 'Nativeエンジニアになるため趣味・インターンとかしてます'
        },
        {
          'option': '最終的な理想のエンジニア像',
          'detail': 'サービス志向が強いのでPMやエンジニアであっても意志決定をする立場でありたいと考えています'
        },
        {
          'option': '今後やること',
          'detail': 'アプリ開発全般・新しい技術のキャッチアップ'
        },
        {
          'option': '好きなこと',
          'detail': 'アプリ開発　UI リファクタリング'
        },
        {
          'option': '嫌いなこと',
          'detail': 'プロジェクトコードが汚くなっていくこと'
        },
        {
          'option': '趣味',
          'detail': '映画、Apple製品'
        },
        {
          'option': 'マイブーム',
          'detail': 'ボドゲ'
        }
      ]
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
