<template>
  <section id="hero">
    <v-row no-gutters>
      <v-img
        :min-height="'calc(100vh - ' + $vuetify.application.top + 'px)'"
        src="https://images.unsplash.com/photo-1503694978374-8a2fa686963a?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MXwxfDB8MXxhbGx8fHx8fHx8fA&ixlib=rb-1.2.1&q=80&w=1080&utm_source=unsplash_source&utm_medium=referral&utm_campaign=api-credit">
        <v-theme-provider dark>
          <v-container fill-height>
            <v-row>
              <v-col class="text-center white--text">
                <p :class="[$vuetify.breakpoint.smAndDown ? 'display-1' : 'display-2']" class="font-weight-light">WELCOME TO</p>
                <p
                  :class="[$vuetify.breakpoint.smAndDown ? 'display-2': 'display-3']"
                  class="font-weight-bold">大盛印刷株式会社</p>
                  <v-btn class="align-self-end" fab outlined>
                    <nuxt-link v-scroll-to="'#about-me'" to tag="div">
                      <v-icon>
                        mdi-chevron-double-down
                      </v-icon>
                    </nuxt-link>
                  </v-btn>
              </v-col>
            </v-row>
          </v-container>
        </v-theme-provider>
      </v-img>
    </v-row>
  </section>
</template>

<script>
export default {

}
</script>

<style>

</style>