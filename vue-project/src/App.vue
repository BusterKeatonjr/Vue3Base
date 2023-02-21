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
  <p :class="{active: true, valid: false,}"></p>
</template>
<style>
.active {
  border: 5px solid red;
}
.valid {
  color: green;
}
</style>
