<template>
  <header id="header">
    <RouterLink class="logo-area" to="/">
      <img class="logo-icon" src="../assets/rivens.png" alt="" />
      <p class="logo-half1">Climbing</p>
      <p class="logo-half2">Elo</p>
    </RouterLink>
    <div class="navbar">
      <RouterLink class="navbar-button" to="/account">Contas</RouterLink>
      <RouterLink class="navbar-button" to="/elojob">EloJob</RouterLink>
      <RouterLink class="navbar-button" to="/login">Coach</RouterLink>
    </div>
    <div class="user">
      <RouterLink to="/login">Login</RouterLink>
    </div>
  </header>
</template>

<style scoped>
#header {
  height: 10vh;
  padding-inline: 1.5vw;

  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  font-size: 1.5rem;
  border-bottom: 1px solid #83b5ff;
  background-color: black;
  color: #83b5ff;
}
.logo-area {
  display: flex;
  align-items: center;
  font-size: 1.5rem;
  cursor: pointer;
}
.logo-icon {
  height: 8vh;
}
@media (max-width: 600px) {
  .logo-area {
    visibility: hidden;
    width: 0px;
  }
}
.logo-half1 {
  color: #c869ff;
  border-bottom: 1px solid;
}
.logo-half2 {
  color: #83b5ff;
  border-bottom: 1px solid;
}
.navbar {
  display: flex;
  gap: 15px;
}
.navbar-button {
  border-radius: 4px;
  border-bottom: 2px solid white;
  padding-inline: 3px;
}
.navbar-button:hover {
  border-bottom: 2px solid #c869ff;
  color: #c869ff;
}
.user:hover {
  color: #83b5ff;
}
</style>
