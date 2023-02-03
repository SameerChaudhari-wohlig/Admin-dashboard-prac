<template>
  <div class="d-flex justify-content-center mt-5">
    <form class="form-group col-3">
      <label class="form-label">
        Name:
        <input class="form-control" v-model="name" type="name" />
      </label>
      <br />
      <label class="form-label">
        Email:
        <input class="form-control" v-model="email" type="email" />
      </label>
      <br />
      <label class="form-label">
        Password:
        <input class="form-control" v-model="password" type="password" />
      </label>
      <br />
      <button class="btn btn-primary" @click.prevent="submit">Submit</button>
    </form>
  </div>
</template>

<script>
import { ref, onMounted } from "vue";
import { useRouter } from "vue-router";

export default {
  setup() {
    const name = ref("");
    const email = ref("");
    const password = ref("");
    const router = useRouter();

    async function submit() {
      await fetch("http://localhost:3000/api/register", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({
          name: name,
          email: email,
          password: password,
        }),
      });

      console.log(router);
      router.push({ path: "/login" });
    }

    return {
      name,
      email,
      password,
      submit,
    };
  },
};
</script>
