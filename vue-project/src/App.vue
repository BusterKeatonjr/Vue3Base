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
  edit(user) {
    user.isEdit = true;
  },
  save(user) {
    user.isEdit = false;
  },
}
}
</script>

<template>
  <!-- <ul>
    <li v-for="user in users" :key="user.id">
<template v-if="!user.isEdit">
  {{ user.name }}
  {{ user.surn }}
  <button @click="edit(user)">
    edit
  </button>
</template>
<template v-else>
  <input v-model="user.name">
  <input v-model="user.surn">
  <button @click="save(user)">
    save
  </button>
</template>
    </li>
  </ul> -->
<table class="user">
<tr v-for="user in users" :key="user.id"> 
<template v-if="!user.isEdit">
  {{ user.name }} {{ user.salary }} {{ user.age }}<button class="button" @click="edit(user)">edit</button>
</template>
<template v-else>
  <input v-model="user.name">
  <input v-model="user.salary">
  <input v-model="user.age">
  <button class="button" @click="save(user)">
      save
  </button>
</template>
</tr>
</table>
</template>

<style scoped>
</style>