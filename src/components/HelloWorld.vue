<template>
  <div>
    <h1>HelloWorld Component</h1>
    <button v-on:click="onClick()">Click</button>
    <div>{{clicked}}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      clicked: false
    }
  },
  methods : {
    onClick() {
      this.clicked = true;
    }
  },
  created () {
    console.log('created')
  },
  mounted() {
    console.log('mounted');
  },
  updated() {
    console.log('updated');
  },
  unmounted() {
    console.log('unmounted');
  },
  errorCaptured() {
    console.log('errorCaptured');
  },
  renderTracked() {
    console.log('renderTracked');
  },
  renderTriggered() {
    console.log('renderTriggered');
  },
  activated() {
    console.log('activated');
  },
  deactivated() {
    console.log('deactivated');
  }
}
</script>
