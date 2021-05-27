<template>
  <v-sheet
    id="contact"
    class="#333333"
    dark
    tag="section"
    tile>
    <v-container>
      <h2 class="display-1 font-weight-regular mb-3 mt-12 text-uppercase text-center">Contact Me</h2>

      <v-responsive class="mx-auto mb-8" width="560">
        <v-divider class="mb-1"></v-divider>
        <v-divider></v-divider>
      </v-responsive>

      <v-theme-provider light>
        <v-row>
          <v-col cols="12">
            <v-text-field flat label="お名前*" solo></v-text-field>
          </v-col>

          <v-col cols="12">
            <v-text-field flat label="Email*" solo></v-text-field>
          </v-col>

          <v-col cols="12">
            <v-text-field flat label="内容*" solo></v-text-field>
          </v-col>

          <v-col cols="12">
            <v-text-field flat label="メッセージ*" solo></v-text-field>
          </v-col>

          <v-col class="mx-auto mb-3" cols="auto">
            <v-btn color="accent">送信</v-btn>
          </v-col>
        </v-row>
      </v-theme-provider>
    </v-container>
  </v-sheet>
</template>

<script>
export default {

}
</script>

<style>

</style>