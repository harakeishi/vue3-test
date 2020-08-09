<template>
  <div></div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    const count = ref(0)
    console.log(count.value) // 0

    count.value++
    console.log(count.value) // 1

    // expose to template
    return {
    }
  }
}
</script>
