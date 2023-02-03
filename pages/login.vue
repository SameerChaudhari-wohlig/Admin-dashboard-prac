<template>
  <body class="text-center">
    <main class="form-signin w-100 m-auto d-flex justify-content-center mt-4">
      <form>
        <img
          class="mb-4"
          src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHwAAAB8CAMAAACcwCSMAAAAaVBMVEX///8A3IKA7sD8/v34/vvy/fiE7sLk+/GK78Wh8tCR8MiX8cvt/Paa8c0E3IQ145wY347C9+HQ+Ojc+u3L+OWu9Nd17LtD5aPm+/Io4Za69t075J9o6rWp89S99t7O+OdU56tt67dY6K2XIl5CAAADSklEQVRoge2Z3XLiMAxGKwMhBAjht1CgpX3/h9yhWSI7tiwrznpvfK4zcyZB+fxFvL1lMplMJpPJZDKZsZkeFpWqFofpf3DvStVS7pO7PxWyTeyeK515WnllyKuk7q0ySfngZ0VPXszSyY+qzzGZe265E87c0iFfJnJ/OdxKHZK4p6VTXiaJ2Q+nW6mPBO4V4Vbq/O/lC1K+ti/enzZ1fVVjHT170q3Urn/xsYZf6s9R3JPKIy8n5sUHeFGP8i70Q93EvMFV08mhWcW7rVA3KQzFDTRu8XI71E3u2rU7MLAGQoor1E20iN+Y8k2sfM3K8VdfQI9FnNsd6jqYsdOmL2+i8pcIdZ2v7uJT3w1wipFToY7gubqvbXkdEXR0qHfguL3bboD34XI61F9glzq63ACDy5Yv1FuwRdrTFjdz3lBvwf6s3G6AYpjcH+pPqu5YmTum7e/MDTrzmVB/grP8oNwAjyFyLtSVwgDb0m6AAd82fKir7kCbXHzyy8TnceJq6iZYHyufG0D8URkQ6t0Nnclpa5HOnCjUf/xuca3gQx2L64FzA4j6XECo46P0TlvLRSKXhPqadwM4Cj6FJNRnRKibNMGrhIBQxx/xO8QN8B0qDwj17tod720JrLKiUL+Gyq9hcj7UsavfQ90Ad4+yQxLqVIVwEVQr+FDHpk5WCBeKd0tC3VVYaWp2fRUQ6ji3ngrh4sHJJaH+KXMDMAsDSaj7K4QLplZIQr2QugFKnzsg1LsXhqsQLny1QhTqbIVw8UPL+VDH70JvYaUha0VAqHevqnzaWshaIQn15TA3ALGr5kMdV08rQaibEBsySajfeAuFs8pKQj24Qrhw1ApRqG94BY1jQyYJdWvnJcPakElCPayw0li1gg91/C507Lxk9DZkfKjjsi9q2n7pbcgkoR5cWGmMDRl/4xhMxM5Lhr4h44MV+1fktLU0kqeOb0fka/ZCe93YG8d8GeEXf6L96my64UfmKE/deO7sSh8vHcety9kKg7VzYInoowX8lOswWPyi461FX8ly5yluEektq4TaqBTMoaYV7qAdDEfv/+edf+K1Beo6+t5r6y+A6Xbt82tnwfl0ifDXm2KEPzozmUwmk8lkMplMIv4AfJYxuP9cIS8AAAAASUVORK5CYII="
          alt=""
          width="72"
          height="57"
        />
        <h1 class="h3 mb-3 fw-normal">Please log in</h1>

        <div class="form-floating">
          <input
            type="email"
            class="form-control"
            id="floatingInput"
            placeholder="name@example.com"
          />
          <label for="floatingInput">Email address</label>
        </div>
        <div class="form-floating">
          <input
            type="password"
            class="form-control"
            id="floatingPassword"
            placeholder="Password"
          />
          <label for="floatingPassword">Password</label>
        </div>

        <div class="checkbox mb-3">
          <label>
            <input type="checkbox" value="remember-me" /> Remember me
          </label>
        </div>
        <button
          @click.prevent="submit"
          class="w-100 btn btn-lg btn-primary"
          type="submit"
        >
          Log in
        </button>
      </form>
    </main>
  </body>
</template>

<script>
import { ref, onMounted } from "vue";
import { useRouter } from "vue-router";

export default {
  setup() {
    const email = ref("");
    const password = ref("");
    const router = useRouter();

    async function submit() {
      await fetch("http://localhost:3000/api/login", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        credentials: "include",
        body: JSON.stringify({
          email: email,
          password: password,
        }),
      });

      console.log(router);
      router.push({ path: "/dashboard" });
    }

    return {
      email,
      password,
      submit,
    };
  },
};
</script>
