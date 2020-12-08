<template>
  <user-item
    v-for="user in users"
    :key="user.id"
    :id="user.id"
    :firstName="user.firstName"
    :lastName="user.lastName"
    :age="user.age"
    @delete-user="removeUser"
  ></user-item>
</template>

<script>
import UserItem from "./UserItem.vue";
export default {
  components: { UserItem },
  data() {
    return {
      users: [
        { id: 0, firstName: "Thibaud", lastName: "Dervily", age: 39 },
        { id: 1, firstName: "Marco", lastName: "Polo", age: 34 },
        { id: 2, firstName: "Hubert", lastName: "Dupont", age: 23 },
        { id: 3, firstName: "David", lastName: "Luby", age: 46 },
      ],
    };
  },
  methods: {
    removeUser(id) {
      this.users = this.users.filter((user) => user.id !== id);
    },
  },
};
</script>