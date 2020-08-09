<template>
  <div>{{ count }} {{ object.foo }}</div>
</template>

<script>
import { ref, reactive } from 'vue'

export default {
  setup () {
    const count = ref({ foo: 'bar' })
    const object = reactive({ foo: 'bar' })
    console.log(count)
    console.log(object)
    // expose to template
    return {
      count,
      object
    }
  }
}
</script>
