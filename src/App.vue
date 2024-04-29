<template>
  <AppForm>

      <template v-slot:help>
        <p>{{help}}</p>
      </template>
      <template  v-slot:fields class="fields">
        <input type="text" placeholder="email">
        <input type="text" placeholder="username">
        <input type="password" placeholder="password">

      </template>
      <template v-slot:buttons class="buttons">
        <button type="submit">submit</button>

      </template>
<p>dummy text</p>
  </AppForm>
  <br/>
  <AppForm>
    <template v-slot:help>
      <p>contact.</p>
    </template>
    <template  v-slot:fields class="fields">
      <input type="text" placeholder="name">
      <input type="text" placeholder="message">

    </template>
    <template v-slot:buttons class="buttons">
      <button type="submit">submit</button>

    </template>

  </AppForm>

</template>

<script>

import AppForm from "./components/Form.vue"
import Form from "@/components/Form.vue";

export default {
  name: "App",
  components: {
    Form,
    AppForm,
  },
  data(){
    return{
      help: 'this is some help text!'
    }
  }
}
</script>



