<template>
  <div>
    <ul>
      <li v-for="(item,index) in list" :key="index">
        <input type="checkbox" v-model="item.completed">
        {{item.title}}
        <button>delete</button>
      </li>
    </ul>
  </div>
</template>
<script>
import { defineComponent, ref} from 'vue'
export default defineComponent({
  name: 'mainArea',
  setup() {
    let list = ref([
      {
        title: 'eating',
        completed: false
      },
      {
        title: 'sleeping',
        completed: true
      }
    ])
    return {
      list
    }
  },
})
</script>
<style  scoped>
li{
  list-style: none;
}
</style>