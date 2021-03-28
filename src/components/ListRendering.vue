<template>
  <div id="list-rendering">
    <ol>
      <li v-for="(todo, key) in todos" :key="key">
        {{ todo.text + ' / key is: ' + key }}
      </li>
    </ol>
  </div>
</template>

<script>
export default {
  data() {
    return {
      todos: [
        { text: 'Learn JavaScript' },
        { text: 'Learn Vue' },
        { text: 'Build sometihng awesome' }
      ]
    }
  }
}
</script>
