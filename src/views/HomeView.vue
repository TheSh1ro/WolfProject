<script>
export default {
  data() {
    return {
      boosters: [
        {
          name: 'Riven',
          winrate: 100,
          jobs: 45,
          id: 1
        },
        {
          name: 'Fiora',
          winrate: 70,
          jobs: 45,
          id: 1
        },
        {
          name: 'Gwen',
          winrate: 60,
          jobs: 45,
          id: 1
        },
        {
          name: 'Jinx',
          winrate: 40,
          jobs: 45,
          id: 1
        },
        {
          name: 'Aphelios',
          winrate: 20,
          jobs: 45,
          id: 1
        }
      ]
    }
  }
}
</script>

<template>
  <main id="main">
    <div id="bannerContainer">
      <div class="bannerContainerTitle">A maior plataforma de ELOJOB do Brasil</div>
    </div>
    <div id="informationContainer">
      <div class="informationContainerVisual">
        <img class="informationContainerIcon" src="../assets/rivens.ico" alt="" />
        <h1 class="informationContainerTitle" style="display: flex">
          <p>Climbing</p>
          <p>Elo</p>
        </h1>
      </div>
      <h1 class="informationContainerAbout">
        Temos os melhores jogadores do servidor para garantir a qualidade do serviço, assim não
        prejudicando seu MMR
      </h1>
      <ul class="informationContainerList">
        <li class="listItem" v-for="booster in boosters" :key="booster.name">
          <img
            class="boosterIcon"
            src="https://cdn.lolalytics.com/generated/champion280px/taliyah.jpg"
            alt="Imagem"
          />
          <p class="boosterName">{{ booster.name }}</p>
          <p class="boosterWinrate">{{ booster.winrate }} WR</p>
        </li>
      </ul>
    </div>
    <div id="servicesContainer"></div>
  </main>
</template>
<style scoped>
#main {
  display: flex;
  flex-direction: column;
  color: #83b5ff;
}
#bannerContainer {
  height: 90vh;

  display: flex;
  justify-content: center;
  align-items: center;
}
#bannerContainer::before {
  content: '';
  background-image: url(https://a-static.besthdwallpaper.com/snowmoon-caitlyn-league-of-legends-lol-wallpaper-3840x2160-103590_54.jpg);
  background-size: cover;
  filter: brightness(70%);
  background-position: center;
  position: absolute;
  height: 100%;
  width: 100%;
}
.bannerContainerTitle {
  font-size: 4rem;
  text-shadow: 0px 0px 10px black;
  color: #a0a0a0;
}
#informationContainer {
  background-color: black;
  min-height: 50vh;
  padding-block: 4vh;

  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 5vh;
}
.informationContainerVisual {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.informationContainerIcon {
  height: 20vh;
}
.informationContainerTitle > p:first-child {
  font-weight: bolder;
  color: #c869ff;
  border-bottom: 2px solid;
}
.informationContainerTitle > p:last-child {
  font-weight: bolder;
  color: #83b5ff;
  border-bottom: 2px solid;
}
.informationContainerAbout {
  text-align: center;
  font-size: 1.5rem;
  padding-inline: 10vw;
}
.informationContainerList {
  display: flex;
  flex-direction: row;
}
.listItem {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.boosterIcon {
  width: 120px;
  margin-inline: 5px;
}
.boosterName {
  color: #a0a0a0;
  font-weight: bold;
}
.boosterWinrate {
  color: #83b5ff;
  font-weight: bold;
}
</style>
