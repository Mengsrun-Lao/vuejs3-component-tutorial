<template>
    <h2>hello {{name}} and super-hero {{ heroName }}</h2>
</template>

<script>
export default{

    name:'Greeting-word',
    props: ['name','heroName']

}
</script>