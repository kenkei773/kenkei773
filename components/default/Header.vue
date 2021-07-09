<template>
<div>
  <v-app-bar app color="white" height="60">
    <v-app-bar-nav-icon
      clipped
      @click="drawer = true"
      class="d-flex d-sm-none"
    />
      <v-avatar class="mr-3" color="grey lighten-3" size="40">
        <v-img contain max-height="70%" src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png">
        </v-img>
      </v-avatar>
      <nuxt-link  v-scroll-to="'#hero'" to tag="div" class="link">
      <v-toolbar-title class="font-weight-black title">
        大盛印刷
      </v-toolbar-title>
      </nuxt-link>

    <v-spacer></v-spacer>

    <nav class="d-none d-sm-flex">
      <ul>
        <li>
          <nuxt-link to="/" tag="div" class="link">Top</nuxt-link>
        </li>
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

      <v-navigation-drawer
        v-model="drawer"
        fixed
        temporary
        right
        width="150"
        src="https://source.unsplash.com/P8VMwYFY-Es"
        height="300"
      >
  <v-list
    nav
    dense
  >
    <v-list-item-group>
      <v-list-item>
        <v-list-item-icon>
            <v-icon>mdi-account</v-icon>
        </v-list-item-icon>
          <v-list-item-title>
            <nuxt-link v-scroll-to="'#about-me'" to tag="div" class="link">About Me</nuxt-link></v-list-item-title>
      </v-list-item>
      <v-list-item>
        <v-list-item-icon>
            <v-icon>mdi-folder</v-icon>
        </v-list-item-icon>
          <v-list-item-title>
            <nuxt-link v-scroll-to="'#features'" to tag="div" class="link">制作</nuxt-link></v-list-item-title>
      </v-list-item>
      <v-list-item>
        <v-list-item-icon>
            <v-icon>mdi-folder-zip</v-icon>
        </v-list-item-icon>
          <v-list-item-title>
            <nuxt-link v-scroll-to="'#features'" to tag="div" class="link">CTP</nuxt-link></v-list-item-title>
      </v-list-item>
      <v-list-item>
        <v-list-item-icon>
            <v-icon>mdi-animation</v-icon>
        </v-list-item-icon>
          <v-list-item-title>
            <nuxt-link v-scroll-to="'#features'" to tag="div" class="link">印刷</nuxt-link></v-list-item-title>
      </v-list-item>
      <v-list-item>
        <v-list-item-icon>
            <v-icon>mdi-blogger</v-icon>
        </v-list-item-icon>
          <v-list-item-title>
            <nuxt-link v-scroll-to="'#blog'" to tag="div" class="link">BLOG</nuxt-link></v-list-item-title>
      </v-list-item>
      <v-list-item>
        <v-list-item-icon>
            <v-icon>mdi-email</v-icon>
        </v-list-item-icon>
          <v-list-item-title>
            <nuxt-link v-scroll-to="'#contact'" to tag="div" class="link">CONTACT</nuxt-link></v-list-item-title>
      </v-list-item>
    </v-list-item-group>
  </v-list>
  </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false
    }
  }
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

