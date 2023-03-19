<template>
    <div :key="CTask.id" v-for="CTask in listOfTask">
      <ListOfTask :gettingTask="CTask"/>
    </div >
</template>

<script>

//List of task
import ListOfTask from './ListTask.vue'
    export default{

        name: 'Tasks',
        props:{

            listOfTask: Array
        },
        components:{
            ListOfTask
        }
    }

</script>