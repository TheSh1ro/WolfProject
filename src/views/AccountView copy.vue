<script setup></script>

<template>
  <main id="main">
    <div id="content-block">
      <section id="apresentation-block">
        <h1 class="apresentation-title">Contas de League of Legends</h1>
        <h2 class="apresentation-description">Entrega rápida e confiável</h2>
      </section>
      <section id="account-block">
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
        <div class="card">
          <p class="account-elo">Desafiante</p>
          <p class="account-level">Level 35</p>
          <img
            class="account-icon"
            src="https://support-leagueoflegends.riotgames.com/hc/article_attachments/4415894930323/Challenger_Emblem_2022.png"
            alt=""
          />
          <p class="account-essence">3679 EA | 44 Campeões</p>
          <p class="account-look">Ver skins</p>
        </div>
      </section>
    </div>
  </main>
</template>
<style scoped>
#main {
  min-height: 90vh;

  display: flex;
  flex-direction: column;

  background-size: 100%;
  filter: opacity(80%);
  background-image: url(../assets/background.jpg);
}

#content-block {
  display: flex;
  flex-direction: column;
  gap: 10vh;

  background-color: rgba(0, 0, 0, 0.5);
  margin: 5vh 3vw;
  padding: 3vh 8vw;
  border-radius: 30px;
  border: 2px groove rgb(149, 165, 255);
}

#apresentation-block {
  grid-area: 1 / 1 / 1 / 4;
  height: fit-content;
  margin-top: 5vh;

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: rgb(243, 194, 255);
}
.apresentation-title {
  font-size: 4rem;
  text-shadow: 3px 3px 15px black;
  text-align: center;
}
@media only screen and (max-width: 1100px) {
  .apresentation-title {
    font-size: 2rem;
  }
}
.apresentation-description {
  color: rgb(184, 194, 255);
  font-style: oblique;
}

#account-block {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(4, 1fr);
  justify-content: center;
  gap: 5vw 5vw;
}
.card {
  height: 300px;
  width: 250px;
  color: white;

  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: space-around;
  background-color: rgba(0, 195, 255, 0.2);
  border-radius: 0px 0px 15px 15px;
  border: 2px solid white;
}
.card:hover {
  border: 2px groove rgb(234, 149, 255);
  margin-top: -1px;
}
.account-elo {
  font-size: 1.4rem;
  font-weight: bolder;
  border-bottom: 2px solid black;
  align-self: center;
  color: rgb(196, 196, 196);
}
.account-icon {
  width: 70%;
  align-self: center;
  margin-top: -40px;
}
.account-level {
  font-size: 1.2rem;
}
.account-look {
  background-color: rgba(0, 0, 0, 0.6);
  width: fit-content;
  align-self: center;
  padding: 2px 35px;
}
.account-look:hover {
  cursor: pointer;
  background-color: black;
}
</style>
