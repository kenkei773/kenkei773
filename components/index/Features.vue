<template>
  <section id="features" class="grey lighten-3 mt-12">
    <v-container class="text-center">
      <h2 class="display-2 font-weight-bold mb-3 mt-12 text-uppercase">Main department
</h2>

      <v-responsive class="mx-auto mb-8" width="560">
        <v-divider class="mb-1"></v-divider>
        <v-divider></v-divider>
      </v-responsive>

      <v-row>
        <v-col
          v-for="feature in features"
          :key="feature.id"
          cols="12"
          md="4"
        >
          <v-card
            class="py-12 px-4"
            color="grey lighten-5"
            flat
            :to="`${feature.link}`"
          >
            <v-theme-provider dark>
              <div>
                <v-avatar color="primary" size="88">
                  <v-icon large>{{ feature.icon }}</v-icon>
                </v-avatar>
              </div>
            </v-theme-provider>

            <v-card-title class="headline justify-center" font-weight-black >{{ feature.title }}</v-card-title>

            <v-card-text class="title text-justify">{{ feature.text }}</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      features: [
        {
          icon: 'mdi-account-group-outline',
          title: '制作',
          text: '印刷物で、まず目をひくのは“美しい文字と鮮明な画像”です。だから私たちは、日本語組版と画像処理技術に拘りを持ち続けます。我が社が担った印刷物は、書店をはじめ、さまざまなところで注目を浴びています。印刷のプロではない他業界の方々からも「大盛印刷が手掛けた印刷物は、他とは違う印象と品質で、とてもきれいだ」というお褒めの言葉をいただきます。なぜ、弊社が手掛けたものが、他社とは違うのでしょう。それは、私たちが美しい日本語組版と画像処理への徹底した拘りを持ち続けているからです。',
          link: '/department/production/'
        },
        {
          icon: 'mdi-update',
          title: 'CTP',
          text: '「XMF」は、「見える化」と「働き方改革」による収益改善をサポートする統合力を持つ、ワークフローシステムです。2007年の発売開始以来、国内2000台、ワールドワイドで7000台の導入実績を持っています。「XMF」にすべてのジョブを登録しておけば、Ｗｅｂポータル『XMF Remote』によって誰でも・いつでも・どこからでも簡単に、進捗状況をはじめとするさまざま情報を正確に把握できることができ、「時間コスト」を含めた統合管理が可能です。',
          link: '/department/ctp/'
        },
        {
          icon: 'mdi-shield-outline',
          title: '印刷',
          text: '豊富な経験と確かな実績による信頼でさまざまなジャンルの印刷物をてがけてきました。豊富な経験と確かな実績による信頼でさまざまなジャンルの印刷物をてがけてきました。豊富な経験と確かな実績による信頼でさまざまなジャンルの印刷物をてがけてきました。豊富な経験と確かな実績による信頼でさまざまなジャンルの印刷物をてがけてきました。',
        },
      ]
    }
  },
  methods: {
    link() {
      this.$router.push({path: this.feature.link})
    }
  }
}
</script>

<style>

</style>