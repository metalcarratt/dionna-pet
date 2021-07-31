<template>
    <div class="phone">
        <img src="phone.png" />
        <p>Use phone</p>
    </div>
</template>

<style scoped>
.phone {
    background-color: #ffe7e7;
    width: 250px;
    padding: 8px;
    margin: 8px;
    position: fixed;
    top: 120px;
    left: 0;
    border-top: 5px solid #fdefef;
    border-left: 5px solid #fdefef;
    border-bottom: 5px solid pink;
    border-right: 5px solid pink;

    text-align: left;
}

.phone:hover {
    cursor: pointer;
}

img {
    height: 60px;
    vertical-align: middle;
}
p {
    display: inline-block;
    vertical-align: middle;
    font-size: 20px;
    margin-left: 8px;
}
</style>