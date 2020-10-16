<template>
<div class="users container">
    <h3>List Users</h3>
    <table class="content-table container">
        <thead>
            <tr>
                <th>Id</th>
                <th>Name</th>
                <th>User Name</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="user in users" v-bind:key="user.id" active-class="active">
                <th>{{user.id}}</th>
                <th>{{user.name}}</th>
                <th>{{user.username}}</th>
            </tr>
        </tbody>
    </table>
</div>
</template>

<script>
import axios from 'axios';
export default {
    name: 'ListUsers',
    data() {
        return {
            users: []
        }
    },
    mounted() {
        axios.get('https://jsonplaceholder.typicode.com/users').then((res) => {
            this.users = res.data;
        });
    }
}
</script>

<style lang="scss">
@import './style.scss';
</style>
