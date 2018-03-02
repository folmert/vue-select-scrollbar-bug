<template>
  <div id="app">
    <div>
      <ui-button content="open modal" v-b-modal.modalId />
      <b-modal id="modalId" title="Title" ok-title="Close" ok-only hide-header-close>
        Text

        <v-select :close-on-select="false" :options='[

            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},
            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},
            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},
            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},
            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},
            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},
            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},
            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},
            {value: "CA", label: "Canada"}, {value: "UK", label: "United Kingdom"},


            ]' />

      </b-modal>
    </div>
  </div>
</template>

<script>
import Vue from 'vue';
import BootstrapVue from 'bootstrap-vue';
Vue.use(BootstrapVue);

import vSelect from 'vue-select';
import UiButton from './UiButton';

import '../node_modules/bootstrap/dist/css/bootstrap.css';
import 'bootstrap-vue/dist/bootstrap-vue.css';

export default {
  name: 'app',
  components: {UiButton, vSelect},
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

.v-select li {
  width: 100%;

}
</style>
