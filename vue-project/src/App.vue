<script>
export default {
  data() {
    return {
      obj: {
        done: true,
        selected: false,
      },
    };
  },
  methods: {},
};
</script>
<template>
  <p :class="obj">text</p>
</template>