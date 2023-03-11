<template>
    <div class="backdrop">
        <div class="modal">
            <h1>{{ header }}</h1>
            this is branch 2 code
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