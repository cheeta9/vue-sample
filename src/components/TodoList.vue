<template>
  <div>
    <ol>
      <TodoItem
        v-for="item in groceryList"
        v-bind:todo="item"
        v-bind:key="item.id"
      />
    </ol>
  </div>
</template>

<script>
import TodoItem from './TodoItem.vue'

export default {
  data() {
    return {
      groceryList: [
        { id: 0, text: 'Vegetables' },
        { id: 1, text: 'Cheese' },
        { id: 2, text: 'Whatever else humans are supposesd eat' }
      ]
    }
  },
  components: {
    TodoItem
  }
}
</script>
