<template>
    <div>
        <h2>Component F</h2>
        <h3>THis is the value passed from acestor form : {{ username }}</h3>
    </div>
</template>

<script>
    export default {
        name:'component-F',
        inject:[
            'username'
        ]
    }
    
</script>

 