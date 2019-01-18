<template lang="html">
  <div class="container">
    <h1>Add To Do List</h1>
    <div class="row">
      <div class="col-md-6">
        <hr>
        <b-card>
          <p>Title:</p>
          <b-form-input type="text"></b-form-input>
          <p>Body</p>
          <b-form-input type="text"></b-form-input>
          <b-button @click="addToList">Submit</b-button>
        </b-card>
      </div>

      <div class="col-md-6">
        <b-card v-for="list in lists" :title="list.title">
          <p>{{list.body}}</p>
        </b-card>
      </div>

    </div>
  </div>
</template>

<script>
  export default {
    data(){
      return{
        title:'',
        body:'',
        lists: [
          {title:'One',body:'Yes I am'},
          {title:'VUe Js',body: 'Is easy'}
        ]
      }
    },

    methods :{
      addToList: function () {
        alert("You have clicked me");

      }
    }
  }
</script>

<style lang="css" scoped>
</style>
