<template>
  <div>
    <button @click="handleClick">CLICK ME</button>
    <select name="dropdown" id="dropdown">
      <option value="1">Option 1</option>
      <option value="2">Option 2</option>
    </select>
    <input type="text" v-model="inputVal">
    <div v-if="inputVal">{{inputVal}}</div>
    <div v-if="hasBeenClicked">
      You clicked
    </div>
    <div v-else>
      You have not clicked
    </div>
  </div>
</template>
<script>
export default {
  name: 'kitchenSink',
  data() {
    return {
      hasBeenClicked: false,
      dropdown: null,
      inputVal: null,
    };
  },
  methods: {
    handleClick() {
      this.hasBeenClicked = !this.hasBeenClicked;
    },
  },
};
</script>
