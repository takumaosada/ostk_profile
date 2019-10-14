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
            <img class="rounded img-fluid" src="../assets/blamtaku.png" alt="blamtaku">
          </div>
          <div class="col-12 col-sm-7">
            <div class="text-left pt-3 pt-sm-0">
              <p>
                #名前 長田 卓馬
                <br><br>
                #大学 東京理科大学経営学部ビジネスエコノミクス学科(２１年卒)
                <br><br>
                #研究 データ分析(安藤ゼミ)
                <br><br>
                #何してる Webサービス/アプリエンジニアになるため趣味で開発・インターンとかしてます
                <br><br>
                #最終的な理想のエンジニア像 サービス志向が強いのでPMやエンジニアであっても意志決定をする立場でありたいと考えています
                <br><br>
                #今後やること アプリ開発
                <br><br>
                #好きなこと UIを見つめる 新しい言語に触れる 新規事業  Apple製品開封
                <br><br>
                #嫌いなこと 大人数の飲み会 急なUIの変更
                <br><br>
                #趣味 ロボットが戦う映画・アニメ ゲーム(実況) 美味しいものを食べる
                <br><br>
                (＊2019/03時点)
              </p>
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
      msg: 'iOS Engineer',
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
