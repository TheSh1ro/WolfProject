<script setup></script>

<template>
  <main id="main">
    <div id="welcome-block">
      <h1 class="welcome-slogan">A maior plataforma de ELOJOB do Brasil</h1>
    </div>
    <div id="boosters-block">
      <div class="boosters-block-logo">
        <img class="riven-icon" src="../assets/rivens.png" alt="" />
        <div class="logo-text">
          <p class="logo-half1">Climbing</p>
          <p class="logo-half2">Elo</p>
        </div>
      </div>
      <h1 class="boosters-text">
        Temos os melhores jogadores do servidor para garantir a qualidade do serviço, assim não
        prejudicando seu MMR
      </h1>
      <ul class="boosters-list">
        <li class="booster-item">
          <img
            class="booster-icon"
            src="https://cdn.lolalytics.com/generated/champion280px/taliyah.jpg"
            alt=""
          />
          <p class="booster-description">Warley Path</p>
          <p>65% WR</p>
        </li>
        <li class="booster-item">
          <img
            class="booster-icon"
            src="https://cdn.lolalytics.com/generated/champion280px/riven.jpg"
            alt=""
          />
          <p class="booster-description">Aram player</p>
          <p>76% WR</p>
        </li>
        <li class="booster-item">
          <img
            class="booster-icon"
            src="https://cdn.lolalytics.com/generated/champion280px/fiora.jpg"
            alt=""
          />
          <p class="booster-description">Felipinho</p>
          <p>0% WR</p>
        </li>
        <li class="booster-item">
          <img
            class="booster-icon"
            src="https://cdn.lolalytics.com/generated/champion280px/draven.jpg"
            alt=""
          />
          <p class="booster-description">Gwen manca</p>
          <p>87% WR</p>
        </li>
      </ul>
    </div>
  </main>
</template>
<style scoped>
#main {
  min-height: 90vh;
  display: flex;
  flex-direction: column;
}
#welcome-block {
  height: 90vh;
  background-image: url(https://a-static.besthdwallpaper.com/snowmoon-caitlyn-league-of-legends-lol-wallpaper-3840x2160-103590_54.jpg);
  background-size: cover;
  filter: opacity(50%);

  display: flex;
  justify-content: center;
  align-items: center;
}
#boosters-block {
  display: flex;
  flex-direction: column;
  background-color: black;
}
.boosters-block-logo {
  display: flex;
  flex-direction: column;
}
.logo-text {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  font-size: 2rem;
  padding-bottom: 3vh;
}
.riven-icon {
  align-self: center;
  height: 20vh;
}
.logo-half1 {
  font-weight: bolder;
  color: #c869ff;
  border-bottom: 2px solid;
}
.logo-half2 {
  font-weight: bolder;
  color: #83b5ff;
  border-bottom: 2px solid;
}
.welcome-slogan {
  color: white;
  text-shadow: 0px 0px 10px black;
  text-align: center;
  font-size: 4rem;
  padding-inline: 5vw;
}
.boosters-text {
  text-align: center;
  font-size: 1.5rem;
  padding-inline: 10vw;
}
.boosters-list {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 10px;
  padding: 5vh;
}
.booster-item {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.booster-icon {
  width: 100px;
}
.booster-description {
}
</style>
