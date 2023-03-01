<script>
import User from './components/Employee.vue'
export default {
  data() {
    return {
      
    }
  },
  components: {
    User
  },
  methods: {
    jujuba() {
      alert('Roblox');
    },
    capybara(){
      alert('CEPU')
    }
  }
}
</script>

<template>
<User @show="jujuba" @show1="capybara" />
</template>


<style scoped>
</style>