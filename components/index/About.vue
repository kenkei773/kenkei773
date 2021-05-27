<template>
  <section id="about-me">
    <div class="text-center mx-4">
      <h2 class="display-2 font-weight-bold mt-12 mb-3">ABOUT ME</h2>

      <v-responsive class="mx-auto mb-8" width="560">
        <v-divider class="mb-1"></v-divider>
        <v-divider></v-divider>
      </v-responsive>

      <v-responsive class="mx-auto subtitle text-justify font-weight-light mb-8" max-width="720">
        「印刷」という技術は、時間も空間も超越して、語りたいことを多くの人に伝えるものです。そして、常にそこから新しい発展があります。お客様から社会への発信を、「印刷」という技術を通してお手伝いし続けてきた大盛印刷。信頼と実績を評価していただけるのは、私たちがいつも、モノづくりだけでなく、お客様の新たなる未来と飛躍のための誕生に立ち会っているからだと、自負しています。印刷物は、常に新しい時代をリードし、活用範囲もさまざまに広がっています。弊社では、新しい技術と旧来から大切に守り続けてきた技術をフル活用し、お客様のご依頼に応えています。
      </v-responsive>

      <v-avatar class="elevation-12 mb-12" size="128">
        <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
      </v-avatar>
      <div></div>
      <v-btn href="https://www.taisei-print.jp" outlined large @click="btn">会社概要</v-btn>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    btn() {
      this.$router.push('/components/index/About')
    }
  }
}
</script>

<style>

</style>