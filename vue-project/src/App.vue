<script>
import User from './components/User.vue'
export default {
  components: {
    User
  }
}
</script>

<template>
<User :name="['Jujuba', 'Capybara']"/>
</template>


<style scoped>
</style>