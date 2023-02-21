<script>
export default {
  data() {
    return {
      obj: {
        hidden: true,
      },
    };
  },
  methods: {
    setDone: function () {
      this.obj.hidden = !this.obj.hidden;
    },
  },
};
</script>
<template>
  <button @click="this.obj.hidden = false">hide </button>
  <button @click="this.obj.hidden = true">hide </button>
  <button @click="setDone">{{ obj.hidden ? "show" : "hide" }} </button><br />
  <p>&nbsp;&nbsp;&nbsp;&nbsp;</p>
  <p :class="obj"></p>
</template>
<style>
p.hidden {
  display: none;
}
</style>