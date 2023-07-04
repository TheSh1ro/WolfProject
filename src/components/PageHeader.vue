<script>
export default {
  data() {
    return {
      userExpanded: false,
      inputLogin: null,
      inputPassword: null,
      user: {
        login: null,
        password: null,
        logged: false
      }
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
      this.inputLogin = null
      this.inputPassword = null
    },
    submit(event) {
      if (event.code == 'Enter' && this.inputLogin && this.inputPassword) {
        this.user.login = this.inputLogin
        this.user.password = this.inputPassword
        this.user.logged = true
      }
    }
  },
  onMounted () {
    
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
    <div
      class="user"
      :class="{ expanded: this.userExpanded }"
      @click="userExpand()"
      @mouseleave="userHidden()"
    >
      <img class="user-picture" src="https://cdn.onlinewebfonts.com/svg/img_454474.png" alt="" />
      <div class="login-inputs" @keypress="submit" v-show="!user.logged">
        <input class="login-input" type="text" placeholder="Usuário" v-model="inputLogin" />
        <input class="login-input" type="text" placeholder="Senha" v-model="inputPassword" />
      </div>
      <div class="user-name" v-show="user.logged">
        <p>{{ user.login }}</p>
      </div>
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

.user {
  display: flex;
  align-items: center;

  height: 10vh;
  width: 10vh;
  border-bottom-left-radius: 20px;
  border-top-left-radius: 20px;
  padding: 1vh;
  gap: 10px;

  background: radial-gradient(circle, rgba(200, 105, 255, 1) 0%, rgba(131, 181, 255, 1) 100%);
  color: black;
  transition: 0.3s ease;
  position: relative;
  overflow: hidden;
}
.user-picture {
  left: 0px;
  height: 100%;
  filter: invert();
}

.user.expanded {
  width: 40vh;
}
.login-inputs {
  display: flex;
  flex-direction: column;
  align-content: center;
  gap: 10px;
}
.login-input {
  border: none;
  border-radius: 15px;
  padding: 4px;
  font-weight: bolder;
  text-align: center;
}
.user-name {
  flex: 1;
}
</style>
