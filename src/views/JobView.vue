<script setup></script>

<template>
  <main id="main">
    <div id="content-block">
      <section id="apresentation-block">
        <h1 class="apresentation-title">EloJob & DuoJob</h1>
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

  background-color: rgba(0, 0, 0, 0.5);
  margin: 5vh 3vw;
  padding: 3vh 8vw;
  border-radius: 30px;
  border: 2px groove rgb(149, 165, 255);
}
</style>
