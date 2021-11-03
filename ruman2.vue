<template>
    <div>
        <h1>hello</h1>
        <h2>{{name}}</h2>
        <button>click me</button>
        <table>
            <tr>
                <td>name</td>
            </tr>
            <tr v-for="user in users" :key="user.id" >
                <td>{{user.name}}</td>
            </tr>
        </table>
    </div>
</template>

<script>
    export default {
        name:'ruman2',
        data() {
            return {
                users: [
                    {name:'punjab'},
                    {name:'sindh'},
                    {name:'kpk'},
                    {name:'balochistan'}
                ]
            }
        },
    }
</script>
