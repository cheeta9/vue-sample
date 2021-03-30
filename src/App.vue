<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3.0 + Vite" />
  <AttributeBinding />
  <EventHandling />
  <TwoWayBinding />
  <ConditionalRendering />
  <ListRendering />
  <TodoList />
  <ComputedBasics />
  <WatchExample />
  <ClassStyle />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import AttributeBinding from './components/AttributeBinding.vue'
import EventHandling from './components/EventHandling.vue'
import TwoWayBinding from './components/TwoWayBinding.vue'
import ConditionalRendering from './components/ConditionalRendering.vue'
import ListRendering from './components/ListRendering.vue'
import TodoList from './components/TodoList.vue'
import ComputedBasics from './components/ComputedBasics.vue'
import WatchExample from './components/WatchExample.vue'
import ClassStyle from './components/ClassStyle.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    AttributeBinding,
    EventHandling,
    TwoWayBinding,
    ConditionalRendering,
    ListRendering,
    TodoList,
    ComputedBasics,
    WatchExample,
    ClassStyle
  }
}
</script>
