<template>
    <span class="stat">
        <label>{{ label }}</label>
        <input type="text" disabled :value="value" />
    </span>
</template>

<script>
export default {
    props: [ 'label', 'value' ]
}
</script>

<style scoped>
.stat {
    display: block;
    margin-bottom: 4px;
}

.stat label {
    display: inline-block;
    width: 120px;
}

.stat input[type='text'] {
    width: 120px;
    text-align: right;
}
</style>