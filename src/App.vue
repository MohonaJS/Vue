<template>
  <div id="app">
   <form action="" @submit.prevent="addTask">
     <h1>To-Do app</h1>
     <p>Find all the task in one place</p>
     <input type="text" placeholder="Add a task" v-model="gettodo"> 
     <button > Submit </button>
   </form>
   <ol>
     <li v-for="(todo, index) in todos" :key="index">
        {{todo.text}}
     </li>
   </ol>

  </div>
</template>

<script>
export default {
  name: 'App',
  data(){ 
    return { 
      gettodo: '',
      todos: [
        {  text: 'Buy eggs', done:true},
        {  text: 'Buy oil', done:false},
        {  text: 'Buy alu', done:false}
      ]
  }},
  methods: {  
    addTask(){  
     console.log(this.todos);
    }
  }
}
</script>

<style>
  button, input {
    margin: 5px;
    padding: 5px;
   
    color: black;
  }
</style>
