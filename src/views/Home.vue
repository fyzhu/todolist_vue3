<template>
  <div class="home">
    <Header></Header>
    <Main></Main>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'
import Footer from '@/components/Footer.vue'

import {defineComponent} from 'vue'
export default defineComponent({
  name: 'Home',
  components: {
    HelloWorld,
    Header,
    Main,
    Footer
  }
})
</script>
