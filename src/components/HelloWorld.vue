<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>
  <div>auto increament count is: {{ auto_count }}</div>
  <p>Edit <code>components/HelloWorld.vue</code> to test hot module replacement.</p>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      count: 0,
      auto_count: 0
    }
  },
  mounted() {
    setInterval(() => {
      this.auto_count++
    }, 1000)
  }
}
</script>
