<template>
  <div class="TabList">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "Login",
  props: {
    msg: String
  },
  data: {
    userLogin: ""
  },
  methods: {
    validateUserlogin() {
      let vm = this;
      if (vm.userLogin === null) alert("Preencha o nome de usuário");
      return;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
