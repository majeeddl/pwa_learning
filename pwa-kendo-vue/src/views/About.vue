<template>
    <div class="about">
        <h1>This is an about page</h1>
        <div>{{data}}</div>
    </div>
</template>


<script>
  export default {
    data() {
      return {
        data: 0
      };
    },
    created() {
      let storage = window.localStorage;
      // storage.setItem("key", "value");
      this.data = storage.getItem("key");
    },
    computed: {}
  };
</script>

