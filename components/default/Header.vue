<template>
  <v-app-bar app color="white" height="60">
    <v-avatar class="mr-3" color="grey lighten-3" size="40">
      <v-img contain max-height="70%" src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png">
      </v-img>
    </v-avatar>
    <v-toolbar-title class="font-weight-black title">
      大盛印刷
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <nav>
      <ul>
        <li>
          <nuxt-link v-scroll-to="'#about-me'" to tag="div" class="link">About Me</nuxt-link>
        </li>
        <li>
          <nuxt-link v-scroll-to="'#features'" to tag="div" class="link">制作</nuxt-link>
        </li>
        <li>
          <nuxt-link v-scroll-to="'#features'" to tag="div" class="link">CTP</nuxt-link>
        </li>
        <li>
          <nuxt-link v-scroll-to="'#features'" to tag="div" class="link">印刷</nuxt-link>
        </li>
        <li>
          <nuxt-link v-scroll-to="'#blog'" to tag="div" class="link">BLOG</nuxt-link>
        </li>
        <li>
          <nuxt-link v-scroll-to="'#contact'" to tag="div" class="link">CONTACT</nuxt-link>
        </li>
      </ul>
    </nav>

  </v-app-bar>
</template>

<script>
export default {

}
</script>

<style scoped>
  nav {
    color:black;
  }
  ul {
    text-decoration: none;
    display: flex;
  }
  li {
    list-style: none;
    text-decoration: none;
    margin-left: 20px;
    font-size: 14px;
  }
  .link {
    cursor: pointer;
  }
</style>

