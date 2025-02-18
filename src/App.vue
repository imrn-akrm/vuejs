<template>
<img alt="Vue logo" src="./assets/logo.png">
  <HelloImran msg="hello imran"  />
  <HomeComponent />
  <EventComponent />
  <TwoWayBinding />
  <GetInputValue />
  <CheckBoxes />
  <Ifelse />
  <Toggle />
  <ForLoop />
</template>

<script>
import HelloImran from './components/hello-imran.vue'
import HomeComponent from './components/Home.vue'
import EventComponent from './components/events.vue'
import TwoWayBinding from './components/twoWayBinding.vue'
import GetInputValue from './components/getInputValue.vue';
import CheckBoxes from './components/checkBoxes.vue';
import Ifelse from './components/ifelse.vue';
import Toggle from './components/toggle.vue';
import ForLoop from './components/forloop.vue';


export default {
  name: 'App',
  components: {
    HelloImran,
    HomeComponent,
    EventComponent,
    TwoWayBinding,
    GetInputValue,
    CheckBoxes,
    Ifelse,
    Toggle,
    ForLoop
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
</style>
