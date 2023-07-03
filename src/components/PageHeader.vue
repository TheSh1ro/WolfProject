<script>
export default {
  data() {
    return {
      userExpanded: false
    }
  },
  methods: {
    userExpand() {
      if (!this.userExpanded) {
        this.userExpanded = true
      }
    },
    userHidden() {
      this.userExpanded = false
    }
  }
}
</script>
<template>
  <header id="header">
    <RouterLink class="logo" to="/">
      <img class="logo-icon" src="../assets/rivens.png" alt="" />
      <p class="logo-text">Climbing</p>
      <p class="logo-text">Elo</p>
    </RouterLink>
    <div class="navbar">
      <RouterLink class="navbar-button" to="/elojob">Serviços</RouterLink>
      <RouterLink class="navbar-button" to="/account">Contas</RouterLink>
      <RouterLink class="navbar-button" to="/login">Aulas</RouterLink>
    </div>
    <div
      class="user"
      :class="{ expanded: this.userExpanded }"
      @click="userExpand()"
      @mouseleave="userHidden()"
    >
      <div class="user-login">
        <input v-show="userExpanded" type="text" placeholder="Usuário" />
        <input v-show="userExpanded" type="text" placeholder="Senha" />
      </div>
      <img
        v-show="!userExpanded"
        class="user-picture"
        src="https://cdn.pixabay.com/photo/2017/07/18/23/23/user-2517433_640.png"
        alt=""
      />
    </div>
  </header>
</template>

<style scoped>
#header {
  height: 10vh;

  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  font-size: 1.5rem;
  background-color: black;
  font-size: 2rem;
  position: relative;
  color: var(--blue);
}
.logo {
  display: flex;
  align-items: center;
  cursor: pointer;
  height: 100%;
  padding-block: 1rem;
}
.logo-icon {
  height: 100%;
}
@media (max-width: 600px) {
  .logo > p {
    display: none;
  }
}
.logo-text:first-of-type {
  color: var(--purple);
}
.logo-text:last-of-type {
  color: var(--blue);
}

.navbar {
  display: flex;
  gap: 1rem;
}
.navbar-button {
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--blue);
}
.navbar-button:hover {
  color: var(--purple);
}

.user {
  display: flex;
  height: 100%;
}
.user-picture {
  height: 100%;
  border-top-left-radius: 30px;
  border-bottom-left-radius: 30px;
  filter: hue-rotate(100deg);
}
.user:hover {
  color: var(--blue);
}
.user.expanded {
  color: red;
}
</style>
