<template>
    <div class="component">
        <h3>You may view the User Details here</h3>
        <p>Many Details</p>
        <p>User Name: {{ myName }}</p>
        <p>Reversed User Name: {{ switchName() }}</p>
    </div>
</template>

<script>
    export default {
        props: {
            myName: {
                type: String,
                default: 'Nathan'
            }
        },
        methods: {
            switchName() {
                return this.myName.split("").reverse().join("")
            }
        }
    }
</script>

<style scoped>
    div {
        background-color: lightcoral;
    }
</style>
