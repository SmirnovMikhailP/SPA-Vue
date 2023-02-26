<template>
    <div>
        <div>Colors: {{ obj.color }}</div>
        <div>Numder: {{ obj.number > 10 ? 'more 10' : 'less 10'}}</div>
        <div>Is published: {{ obj.isPublished ? 'Published' : 'Not Published'}}</div>
    </div>
</template>

<script>
import SinglePostComponent from "./SinglePostComponent";

export default {
    name: "SomeComponent",

    data() {
        return {}
    },

    props: [
        'obj'
    ],

    mounted() {
        this.$parent.$parent.parentLog()
    },

    methods: {}

}
</script>

<style scoped>

</style>
