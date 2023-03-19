<template>
  <header>
    <h1>{{ title}}</h1>
    <Button @click="AddClick() " color="green" title="Add Task"/>
    <!--<Button  @click="UpdateClick() " color="orange" title="Update Task"/>
    <Button  @click="DeleteClick() " color="red" title="Delete Task"/>-->
  </header>
</template>

<script>
import Button from './Button.vue'

export default {
    name: 'Header',
    props:{
        title: String,

    },
    components: {
        Button

    },
    methods:{
        AddClick(){
            console.log("Nagana add pwede na matulog")
        },
        UpdateClick(){
            console.log("Nagana update pwede na matulog")
        },DeleteClick(){
            console.log("Nagana delete pwede na matulog")
        }
    },
}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

</style>