<template>
  <seciton id="blog">
    <v-container>
      <h2 class="display-2 font-weight-bold mb-3 mt-12 text-uppercase text-center">Blog</h2>

      <v-responsive class="mx-auto mb-8" width="560">
        <v-divider class="mb-1"></v-divider>
        <v-divider></v-divider>
      </v-responsive>

          <v-row>
            <v-col
              v-for="({ src, text, title }, i) in articles"
              :key="i"
              cols="12"
              md="4"
            >
              <v-img
                :src="src"
                class="mb-4"
                height="275"
                max-width="100%"
              ></v-img>

              <h3
                class="font-weight-black mb-4 text-uppercase"
                v-text="title"
              ></h3>

              <p
                class="body-2 font-weight-light mb-5 text-justify"
                v-text="text"
              ></p>

              <v-btn
                class="ml-n4 font-weight-black"
                text
              >
                続きを読む
              </v-btn>
            </v-col>
          </v-row>
    </v-container>
  </seciton>
</template>

<script>
export default {
  data() {
    return {
        articles: [
          {
            src: 'https://images.unsplash.com/photo-1423784346385-c1d4dac9893a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80',
            title: 'Mobile first & Responsive',
            text: 'v-containerはその名の通りコンテナです。オプション属性がいろいろとあって、fluid属性を付与することで左右いっぱいにコンテナを広げたり、fill-height属性を付与することでv-containerの内部要素を上下中央寄せにしたりできます。',
          },
          {
            src: 'https://images.unsplash.com/photo-1475938476802-32a7e851dad1?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80',
            title: 'Think outside the box',
            text: 'Vuetifyは美しく整えられたマテリアルコンポーネントを提供するVue UIライブラリです。 デザインスキルは必要ありません 。素晴らしいアプリケーションを作成するために必要な全てが揃っています。',
          },
          {
            src: 'https://images.unsplash.com/photo-1416339442236-8ceb164046f8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1892&q=80',
            title: 'Small changes, big difference',
            text: 'このコマンドは、プロジェクトのテンプレートファイル、コンポーネントフォルダ、vue.config.jsなどに変更を加えます。 Vue-CLI を使用して Vuetify をインストールする場合は、データ損失の可能性を避けるために、コードをコミットしてください。 インストール中にAdvanced installオプションを選択することで、テンプレートの変更をスキップすることができます。',
          }
        ]
    }
  }
}
</script>

<style>

</style>