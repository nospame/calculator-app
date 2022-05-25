<script>

export default {
  name: 'HomeView',
  data: function () {
    return {
      entry: '',
      result: ''
    }
  },
  methods: {
    calculate: function () {
      this.result = this.entry.split(/\D/)
    },
    multiply: () => {

    },
    divide: () => {

    },
    add: () => {

    },
    subtract: () => {

    }
  }
}
</script>

<template>
  <div class="home">
    <p>{{ result }}</p>
    <input v-model="entry" type="text">
    <br />
    <button class="uk-button uk-button-default">1</button>
    <button class="uk-button uk-button-default">2</button>
    <button class="uk-button uk-button-default">3</button>
    <br />
    <button class="uk-button uk-button-default">4</button>
    <button class="uk-button uk-button-default">5</button>
    <button class="uk-button uk-button-default">6</button>
    <br />
    <button class="uk-button uk-button-default">7</button>
    <button class="uk-button uk-button-default">8</button>
    <button class="uk-button uk-button-default">9</button>
    <br />
    <button class="uk-button uk-button-default">0</button>
    <button v-on:click="calculate()" class="uk-button uk-button-default">Enter</button>
  </div>
</template>

