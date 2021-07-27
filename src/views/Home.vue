<template>
  <div class="home">
    <Header></Header>
    <Main></Main>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'
import Footer from '@/components/Footer.vue'

import {defineComponent, ref, reactive, toRefs} from 'vue'
export default defineComponent({
  name: 'Home',
  components: {
    Header,
    Main,
    Footer
  },
  setup() {
    let num = ref(0)
    let data = reactive({
      name: 'zyf',
      arr: [1,2,3]
    })
    return {
      num,
      ...toRefs(data)
    }
  }
})
</script>
