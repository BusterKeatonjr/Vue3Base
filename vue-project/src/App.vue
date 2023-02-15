<script>
export default {
  data() {
    return {
      data: {
      user1: '100$',
      user2: '200$',
      user3: '300$',
      }
    }
  },
  methods: {
    }
}
</script>
<template>
  <ul>
    <li v-for="value in data">{{ value }}</li>
  </ul>
  <ul>
    <li v-for="(value, key) in data">{{ key }} - {{ value }}</li>
  </ul>
  <ul>
    <li v-for="(value, key, index) in data">{{ key }} - {{ value }} - {{ index }}</li>
  </ul>
  <ul>
    <li v-for="(value, key, index) in data">{{ key }} - {{ value }} - {{ index + 1 }}</li>
  </ul>
</template>
