<template>
  <div>
    <header>
      <input type="text" v-model="value">
    </header>
  </div>
</template>
<script>
import { defineComponent, ref} from 'vue'
export default defineComponent({
  name: 'navHeader',
  setup() {
    let value = ref('')
    return {
      value
    }
  },
})
</script>