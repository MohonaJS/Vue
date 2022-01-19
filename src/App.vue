<template>
  <div id="app">
    <div>
      <form action="" @submit="handleformsubmit">
        <div><label for="">Your Name: </label>
          <input type="text"></div>
        <button type="submit">Submit form </button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
  }, 
  data(){return{  
    name: ''
  }},
  methods:{  
    handleformsubmit(e){  
      e.preventDefault();
      
    }
  }
}
</script>

<style>

</style>
