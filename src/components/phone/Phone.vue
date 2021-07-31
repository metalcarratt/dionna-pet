<template>
    <div class="bigPhone">
        <span class="speaker" />
        <span class="screen" />
        <span class="button" @click="$emit('close')">Off</span>
    </div>
</template>

<style scoped>
.bigPhone {
    background-color: #e6a2ec;
    width: 400px;
    height: 600px;
    position: fixed;
    z-index: 10;
    top: 40px;
    left: calc(50% - 200px);

    border: 2px solid purple;
    border-radius: 32px;
}

.speaker {
    display: block;
    width: 200px;
    height: 20px;
    background-color: #420e3f;
    margin-left: calc(50% - 100px);
    margin-top: 8px;
    border-radius: 8px;
    border: 1px solid black;
}

.screen {
    display: block;
    width: 380px;
    height: 500px;
    background-color: #ffe7fe;
    margin-left: calc(50% - 190px);
    margin-top: 8px;
    border-radius: 16px;
    border: 1px solid black;
}

.button {
    display: block;
    width: 100px;
    height: 40px;
    background-color: #420e3f;
    margin-left: calc(50% - 50px);
    margin-top: 8px;
    border-radius: 16px;
    border: 1px solid black;
    padding-top: 8px;
    box-sizing: border-box;
    color: #420e3f;
}

.button:hover {
    cursor: pointer;
    background-color: #7a1974;
}
</style>