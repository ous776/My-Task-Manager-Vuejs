<template>
    <header>
      <h1>{{title}}</h1>  
      <Button @show-addtask="$emit('show-add')" :text="showAtask ? 'Close' : 'Add Task'" :color="showAtask ? 'red' : 'green'"/>
    </header>
</template>


<script>
 /* eslint-disable */

 import Button from './Button'
export default {

    name: 'Header',
    props: {
        title: String,
        showAtask: Boolean,
    },

    components: {
        Button
    }
}
</script>

<style scoped>
header {
    display:flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>