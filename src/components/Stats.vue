<template>
    <div class="stats">
        <Stat label="Emotion" :value="emotion" />
        <Stat label="Hunger" :value="hunger" />
        <Stat label="Money" :value="money" />
    </div>
</template>

<script>
import Stat from './Stat.vue';

export default {
    components: { Stat },
    data() {
        return {
            emotion: 'Lonely',
            hunger: 'Not hungry',
            money: '$100'
        }
    }
}
</script>

<style scoped>
.stats {
    background-color: #ffe7e7;
    width: 250px;
    padding: 8px;
    margin: 8px;
    position: fixed;
    top: 0;
    left: 0;
    border-top: 5px solid #fdefef;
    border-left: 5px solid #fdefef;
    border-bottom: 5px solid pink;
    border-right: 5px solid pink;

    text-align: left;
}
</style>