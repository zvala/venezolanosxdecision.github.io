<template>
  <section v-if="show">
    <div class="container">
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Provident
        itaque repudiandae eaque blanditiis aut odit ab natus corporis id
        dolorum sapiente fugit, cupiditate doloremque ratione, in sint non ad
        ipsam!
      </p>
      <button @click="dismiss" class="">aceptar</button>
    </div>
  </section>
</template>

<script>
export default {
  name: "CookieConsent",
  data() {
    return {
      show: undefined,
    };
  },
  computed: {
    cookie() {
      return this.getCookie();
    },
  },
  beforeMount() {
    this.show = this.cookie;
  },
  methods: {
    dismiss() {
      this.show = false;
      this.setCookie();
    },
    getCookie() {
      return localStorage.getItem("cookie") === null;
    },
    setCookie() {
      localStorage.setItem("cookie", "venezolanos por decision");
    },
  },
};
</script>

<style scoped>
section {
  position: fixed;
  background-color: #fff;
  box-shadow: 0 1px 6px 0 rgb(54 64 67 / 80%);
  width: 100%;
  bottom: 0;
}

section .container {
  display: flex;
  gap: 16px;
}

button {
}
</style>
