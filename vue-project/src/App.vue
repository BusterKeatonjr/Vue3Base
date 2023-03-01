<script>
import User from './components/User.vue'
export default {
  data() {
    return {
      name: 'Jujuba',
      salary: '125000',
      age: '19',
    }
  },
  components: {
    User
  }
}
</script>

<template>
<User :name="name" :salary="salary" :age="age"/>
</template>


<style scoped>
</style>