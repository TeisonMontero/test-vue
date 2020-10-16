<template>
<div class="hello">
    <h3>My aplication with vueJS</h3>
</div>
</template>

<script>
export default {
    name: 'HelloWorld',
    props: {
        msg: String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style lang="scss" scoped>
@import './style.scss';
</style>
