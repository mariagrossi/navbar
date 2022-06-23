<template>
  <div class="home">
    <navbar msg="" />
  </div>
</template>

<script>
// @ is an alias to /src
import navbar from "@/components/navbar.vue";

export default {
  name: "Home",
  components: {
    navbar
  }
};
</script>
