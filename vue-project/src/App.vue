<script>
export default{
data(){
  return{
    users: [
      {
        id: 1,
        name: 'name1',
        salary: 100,
        age: 12,
      },
      {
        id: 2,
        name: 'name2',
        salary: 200,
        age: 12,
      },
      {
        id: 3,
        name: 'name3',
        salary: 300,
        age: 12,
      },
    ],
  }
},
methods: {
  removeUser: function (id) {
    this.users = this.users.filter((user) => {
      return user.id !== id;
    })
  }
}
}
</script>

<template>
<table class="user">
  <tr v-for="user in users" :key="user.id"> {{ user.name }} {{ user.salary }} {{ user.age }} <button class="button" @click="removeUser(users.id)">remove</button>
</tr>
</table>
</template>

<style scoped>
</style>