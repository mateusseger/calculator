<template>
    <button
        :class="{ double, triple, operation }"
        @click="$emit('onClick', label)">
        {{ label }}
    </button>
</template>

<script>
export default {
    props: {
        label: {
            type: String
        },
        double: {
            type: Boolean
        },
        triple: {
            type: Boolean
        },
        operation: {
            type: Boolean
        }
    }
}
</script>

<style>
button {
    border: none;
    border-top: 1px solid #3336;
    border-right: 1px solid #3336;
    background-color: #6661;
    font-size: 1.2em;
    font-weight: bold;
    transition: all 0.1s ease-out;	
}
button:active {
    background-color: #6663;
}
button.double {
    grid-column: span 2;
}
button.triple {
    grid-column: span 3;
}
button.operation {
    background: #fa8231;
    color: #fff;
    border-right: none;
}
button.operation:active {
    background: #fa8231cc;
}
</style>