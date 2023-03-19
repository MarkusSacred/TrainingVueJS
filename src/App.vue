<script>
import Headers from './components/Header.vue'
import Tasks from './components/Tasks.vue'

export default{
  name: 'App',
  components:{
    Headers,
    Tasks
  },
  data(){
    return {
      listOfTask: []
    }
  },created(){
      this.listOfTask = [
        {
          id: '1',
          text: 'This is a sampling 1',
          day: 'March',
          reminder: true,
      
        },
        {
          id: '2',
          text: 'This is a sampling 2',
          day: 'April',
          reminder: true,
      
        },
        {
          id: '3',
          text: 'This is a sampling 3',
          day: 'May',
          reminder: true,
      
        },


      ]
  }
}

</script>

<template>
    <div class="container">
        <Headers title="Ticketing System"/>
        <Tasks :listOfTask="listOfTask"/>
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap');
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: 'Poppins', sans-serif;
}
.container {
  max-width: auto;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid steelblue;
  padding: 30px;
  border-radius: 5px;
}
.btn {
  display: inline-block;
  
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}
.btn:focus {
  outline: none;
}
.btn:active {
  transform: scale(0.98);
}
.btn-block {
  display: block;
  width: 100%;
}
</style>