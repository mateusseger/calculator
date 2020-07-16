<template>
    <div class="display">
        {{ value }}
    </div>
</template>

<script>
export default {
    props: ['value']
}
</script>

<style>
.display {
    grid-column: span 4;
    background-color: #0009;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    font-size: 2em;
    color: #fff;
    padding: 15px;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    overflow: hidden;
    font-weight: bold;
}
</style>