<template>
  <div id="computed-basics">
    <p>Has published books:</p>
    <span>{{ publishedBooksMessage }}</span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      author: {
        name: 'John Doe',
        books:[
          'Vue 2 - Advanced Guide',
          'Vue 3 - Basic Guide',
          'Vue 4 - The Mystery'
        ]
      }
    }
  },
  computed: {
    publishedBooksMessage() {
      return this.author.books.length > 0 ? 'Yes' : 'No'
    }
  }
}
</script>
