<template>
  <div id="app" >
    <todo-add></todo-add>
    <hr><hr>
    <todo-show></todo-show>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import todo from './components/todo.vue'
import addTodo from './components/Add.vue'

export default {
  components:{
    'todo-show':todo,
    'todo-add': addTodo
  },
  name: 'app',
  data () {
    return {

    }
  }
}
</script>

<style>

</style>
