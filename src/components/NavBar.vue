<script setup lang="ts">
defineProps<{
  msg: string;
}>();
</script>

<template>
  <div class="navBar">
    <img
      alt="Vue logo"
      class="logo"
      src="../assets/logo.svg"
      width="125"
      height="125"
    />
    <h3>About us</h3>
    <h3>Services</h3>
    <h3>Use cases</h3>
    <h3>Pricing</h3>
    <h3>Blog</h3>
    <Button>Request a quote</Button>
    <img
      alt="Vue logo"
      class="menu"
      src="../assets/menu-icon.svg"
      width="125"
      height="125"
    />
  </div>
</template>

<style scoped>
h3 {
  font-size: 1.2rem;
}

.logo {
  background-color: #fff;
  height: 68px;
}

.menu {
  width: 24px;
  height: 16px;
  display: none;
}

/* Navbar styles */
.navBar {
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: space-around;
  padding-left: 2em;
  padding-right: 2em;
  margin-top: 1em;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background-color: #fff;
  height: 68px;
  width: 100%;
}

/* Navbar h3 styles */
.navBar h3 {
  font-weight: 400;
  color: #000;
}

.navBar h3:hover {
  color: #00bfa6;
  cursor: pointer;
}

/* Navbar button styles */
.navBar Button {
  width: 231px;
  height: 68px;
  border-radius: 14px;
  background: none;
  font-weight: 400;
  color: #000;
  font-size: 1.2rem;
  cursor: pointer;
}

/* Media queries */
@media (max-width: 800px) {
  .navBar h3,
  button {
    display: none;
  }

  .menu {
    display: flex;
  }

  .navBar {
    justify-content: space-between;
  }
}
</style>
