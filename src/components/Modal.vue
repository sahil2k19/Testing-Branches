<template>
    <div class="backdrop">
        <div class="modal">
            <h1>{{ header }}</h1>
            bro dont change the main 
            <p>{{ text }}</p>
        </div>
    </div>
</template>

<script>
    export default{
        props:['header', 'text', 'theme'],
    }
</script>

<style>

</style>