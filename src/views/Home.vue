<template>
  <div class="Home">
    <h1 class="text-2xl font-bold">TRAcKify</h1>

    <button @click="showMessage">button</button>
    <p v-if="message">{{ message }}</p>
  </div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            message: null,
        };
    },
    methods:{
        showMessage(){
            this.message = "This is a message from the Trackify component";
        },
    },
};
</script>
