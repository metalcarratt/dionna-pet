<template>
  <div id="app">
    <Title />
    <img src="Diona.PNG" />
    <Stats />
    <PhoneIcon @click.native="usingPhone = true" />
    <Phone v-if="usingPhone" @close="usingPhone = false" />
  </div>
</template>

<script>
import Title from '@/components/Title.vue';
import Stats from '@/components/Stats.vue';
import PhoneIcon from '@/components/PhoneIcon.vue';
import Phone from '@/components/phone/Phone.vue';

export default {
  name: 'App',
  components: { Title, Stats, PhoneIcon, Phone },
  data() {
    return {
      usingPhone: false
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

img {
  height: 600px;
}
</style>
