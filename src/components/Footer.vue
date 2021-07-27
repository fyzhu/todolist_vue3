<template>
  <div>
    <footer>
      <div>
        {{isCompleted}}/ {{all}}
      </div>
      <button v-if="isCompleted>0" @click="handleClear">clear</button>
    </footer>
  </div>
</template>
<script>
import { defineComponent, ref} from 'vue'
export default defineComponent({
  name: 'navFooter',
  setup() {
    let isCompleted = ref(1)
    let all = ref(3)
    let handleClear = () => {
      console.log('handleClear');
    }
    return {
      isCompleted,
      all,
      handleClear
    }
  },
})
</script>