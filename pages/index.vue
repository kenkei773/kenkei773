<template>
  <div>
    <!-- top -->
    <Top />
    <!-- about -->
    <About />
    <!-- features -->
    <Features />
    <!-- stats -->
    <Stats />
    <!-- blog -->
    <Blog />
    <!-- contact -->
    <Contact />
  </div>
</template>

<script>
import Top from '~/components/index/Top.vue'
import About from '~/components/index/About.vue'
import Features from '~/components/index/Features.vue'
import Stats from '~/components/index/Stats.vue'
import Blog from '~/components/index/Blog.vue'
import Contact from '~/components/index/Contact.vue'

export default {
  components: {
    Top,
    About,
    Features,
    Stats,
    Blog,
    Contact
  }
}
</script>
