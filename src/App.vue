<template>
<div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <ListUsers />
</div>
</template>

<script>
import HelloWorld from './components/HelloWorld/HelloWorld.vue'
import ListUsers from './components/ListUsers/ListUsers.vue'

export default {
    name: 'App',
    components: {
        HelloWorld,
        ListUsers
    }
}
</script>
