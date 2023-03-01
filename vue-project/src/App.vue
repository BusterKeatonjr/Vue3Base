<script>
import User from './components/Employee.vue'
export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: 'Jujuba',
          salary: 125000,
          age: 19
        },
        {
          id: 2,
          name: 'Capybara',
          salary: 125000,
          age: 18
        },
        {
          id: 3,
          name: 'Nix',
          salary: 33000,
          age: 0
        },
      ],
    }
  },
  components: {
    User
  }
}
</script>

<template>
<User v-for="user in users" :name="user.name" :salary="user.salary" :age="user.age" :key="user.id" />
</template>


<style scoped>
</style>
