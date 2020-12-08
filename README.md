# vue3-component-cli-exercise

## Exercise N°5


1. Create a `UserItem.vue` component which represents a user item list element. 
It will take some props (`id`, `firstName`, `lastName`, `age`). 
It will output a `user-delete` event with user id.
Add a `delete` button which will trigger the delete event.


2. Create a `UserList.vue` component which will display a user list. 
Define a data object `{users: []}`, with a hard-coded value list.
Listen the `user-delete` event and update `users` array.

3. Use `UserList.vue` in `App.vue`.


## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
