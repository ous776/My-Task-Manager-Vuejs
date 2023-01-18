<template>
    <button @click="onClick()" :style="{ background: color}" class="btn">{{text}}</button>
</template>

<script>
/* eslint-disable */
export default{
name: 'Button',
props: {
    text: String,
    color: String
},

methods: {
    onClick() {
        this.$emit('show-addtask')
    }
}

}

</script>