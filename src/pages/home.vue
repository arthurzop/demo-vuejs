<script setup lang="jsx">
</script>

<template>
  <header>
    <h1 class="headerTitle">SOS</h1>
    <div id="menu">
      <nav class="headerNav">
        <a href="#album" class="navItem">Álbum</a>
        <a href="#tracklist" class="navItem">Tracklist</a>
        <a href="#artista" class="navItem">Artista</a>

        <a href="#detalhes" class="navItem">Detalhes</a>
      </nav>
    </div>
  </header>
  <main>
    <div class="albumContainer">
      <div class="albumTop">
        <div class="spotifyContainer">
          <h1 class="spotifyTitle">SOS</h1>
          <h2 class="spotifySubtitle">Sza</h2>
          <div id="divider"></div>
          <div class="spotifyInfo">
            <div class="spotifyText">
              <b>Gênero: </b>R&B, Soul <br />
              <b>Ano de Lançamento: </b> 2022
            </div>
            <p class="spotifyTime">1h06min</p>
          </div>
        </div>
        <div class="leftContainer">
          <div class="descricaoContainer">
            <div class="descricaoSubContainer">
              <h4 class="descricaoText">Gênero:</h4>
              <h5 class="descricaoSubText">R&B, Soul, Hip Hop</h5>
              <h4 class="descricaoText">Ano de Lançamento:</h4>
              <h5 class="descricaoSubText">2022</h5>
            </div>
            <div class="descricaoSubContainer">
              <h4 class="descricaoText">Artista:</h4>
              <h5 class="descricaoSubText">SZA</h5>
              <h4 class="descricaoText">Duração:</h4>
              <h5 class="descricaoSubText">23 Faixas, 1h06min</h5>
            </div>
          </div>
          <div class="infoContainer">
            <div class="divider"></div>
            <div class="infoSubContainer">
              <div class="infoText">
                <b>SOS</b> é o segundo álbum de estúdio da cantora e compositora
                estadunidense SZA. Lançado em 9 de dezembro de 2022 através da
                Top Dawg Entertainment e RCA Records. Serve como continuação do
                álbum anterior de SZA, Ctrl.
              </div>
            </div>
          </div>
        </div>
        <div class="tracklistContainer" id="tracklist">
          <h1 class="tracklistTitle">TrackList</h1>
          <div class="tracklistText">
            1. SOS <br />
            2. Kill Bill <br />
            3. Seek & Destroy <br />
            4. Low <br />
            5. Love Language <br />
            6. Blind <br />
            7. Used (ft. Don Toliver) <br />
            8. Snooze <br />
            9. Notice Me <br />
            10. Gone Girl <br />
            11. Smoking on my Ex Pack <br />
            12. Ghost in the Machine <br />
            (ft. Phoebe Bridgers) <br />
            13. F2F <br />
            14. Nobody Gets Me <br />
            15. Conceited <br />
            16. Too Late <br />
            17. Far <br />
            18. Shirt <br />
            19. Open Arms (ft. Travis Scott) <br />
            20. I Hate U <br />
            21. Good Days <br />
            22. Forgiveless (ft. Ol' Dirty Bastards)
          </div>
        </div>
      </div>
    </div>
    <div class="fullDivider"></div>
    <div class="artistContainer">
      <div class="artistText">
        <h1 class="artistTitle" id="artista">sza</h1>
        <p class="artistSubText">
          <b>Solána Rowe,</b> mais conhecida como SZA é uma cantora, compositora
          e produtora que representa boa parte do que identifica a música negra
          atual.
        </p>
        <p class="artistSubText">
          São colagens assumidas de sons, gêneros e diferentes conceitos
          sonoros, eixo que a norte-americana representa na sonoridade vasta que
          se derrama ao longo de toda a obra.
        </p>
      </div>
    </div>
  </main>
  <footer id="detalhes">
    <a href="https://github.com/arthurzop">
    </a>
    <div class="footerSub">
      <nav class="footerNav">
        <a
          href="https://pt.wikipedia.org/wiki/SZA"
          target="_blank"
          class="navItem"
          >About</a
        >
        <a
          href="https://www.youtube.com/channel/UCO5IQ70V7l-XpHW40HwaGsw"
          target="_blank"
          class="navItem"
          >Music</a
        >
        <a href="https://www.instagram.com/sza/" target="_blank" class="navItem"
          >Social</a
        >
      </nav>
    </div>
  </footer>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Tourney:wght@700&family=Urbanist:wght@300;400;500;600&family=Yuji+Syuku&display=swap");

/* font-family: 'Tourney', sans-serif;
font-family: 'Urbanist', sans-serif;
font-family: 'Yuji Syuku', serif; */

:root {
  /* color var */
  --darkGreen: #002029;
  --richBlack: #00303d;
  --midnightGreen: #004052;
  --prussian-blue: #0b3047;
  --header: rgba(0, 64, 82, 0.5);
  --white: #fff;

  /* font-weight */
  --light: 300;
  --regular: 400;
  --medium: 500;
  --semibold: 600;
  --bold: 800;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  color: var(--white);
  text-decoration: none;

  scroll-behavior: smooth;
  transition: 0.5s;
}

body {
  width: 100%;
  height: 100%;
  background-color: var(--darkGreen);
  display: flex;
  flex-direction: column;
  justify-content: space-between;

  background-image: url(../assets/background.png);
  background-repeat: no-repeat;
  background-size: cover;

  scroll-behavior: smooth !important;
}

header {
  width: 100%;
  height: 15vh;
  display: flex;
  align-items: center;
  justify-content: space-between;

  padding: 3vh 5vw;

  position: fixed;
  z-index: 1;

  background-color: var(--header);
  box-shadow: rgba(0, 0, 0, 0.2) 0px 8px 24px;
}

.headerTitle {
  font-family: "Tourney", sans-serif;
  font-weight: var(--bold);
  font-size: 6em;
}

.menuImg{
  display: none;
}


.headerNav {
  display: flex;
  gap: 3vw;
}

.navItem {
  font-size: 2em;
  font-weight: var(--semibold);
  font-family: "Urbanist", sans-serif;
}

main {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 15vh 0 5vh;
}

.albumContainer {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  padding: 5vh 5vw 5vh 2.5vw;
}

.spotifyContainer{
  display: none;
}

.albumTop {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
}

.descricaoContainer {
  display: flex;
  width: 100%;
  justify-content: space-around;
  padding-bottom: 18vh;
}

.descricaoSubContainer {
  display: flex;
  flex-direction: column;
  gap: 2.5vh;
  font-family: "Urbanist", sans-serif;
}

.descricaoText {
  font-size: 2.2em;
  font-weight: var(--semibold);
}

.descricaoSubText {
  font-size: 2em;
  font-weight: var(--regular);
}

.tracklistContainer {
  display: flex;
  flex-direction: column;
  margin-top: 7vh;
  gap: 3vh;
  font-family: "Yuji Syuku", serif;
}

.tracklistTitle {
  font-size: 3em;
}

.tracklistText {
  font-size: 2em;
}

#albumMobile {
  display: none;
}

.albumImage {
  width: 550px;
  height: 550px;
}

.albumImage:hover {
  transform: scale(1.05);
  transition: 0.8s;
}

.leftContainer {
  display: flex;
  flex-direction: column;
  width: 70%;
  align-items: center;
}

.menuSvg{
  display: none;
}

.divider {
  width: 100%;
  border: 1px var(--white) solid;
  margin: 5vh 0;
}

.infoContainer {
  width: 80%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.infoSubContainer {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.infoText {
  width: 100%;
  text-align: left;
  font-family: "Urbanist", sans-serif;
  background-color: var(--prussian-blue);
  font-size: 2.5em;
  font-weight: var(--light);
  padding: 4vh 2vh;
  border-bottom-left-radius: 10px;
  border-bottom-right-radius: 10px;
}

.albumArtistImage {
  width: 100%;
}

.artistImg{
  width: 550px;
  height: 350px;
}

/* -------------------------- */

.artistContainer {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-around;
  margin-top: 35vh;
  padding: 3vh 3vw;
  gap: 5vw;
}

.artistText {
  width: 80%;
  display: flex;
  flex-direction: column;
  gap: 3vh;
  font-weight: var(--light);
}

.artistInfoContainer {
  width: 100%;
  display: flex;
  flex-direction: column;
}

.artistTitle {
  font-size: 5em;
  font-family: "Yuji Syuku", serif;
  text-transform: uppercase;
  margin-inline-start: 3vw;
}

.artistSubText {
  font-family: "Urbanist", sans-serif;
  font-size: 2em;
}

.artistImg{
  width: 950px;
  height: 550px;
}

/* -------------------------- */

footer {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 3vh;
  background-color: var(--midnightGreen);
}

.footerSub {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Urbanist", sans-serif;
}

.githubIcon{
  height: 50px;
}

.footerNav{
  display: flex;
  gap: 5vw;
}

/* ----------------------- */

@media (max-width: 1080px) {

  header {
    align-items: center;
    justify-content: space-between;
  }

  .headerNav {
    display: flex;
    flex-direction: column;
    background-color: var(--header);
    padding: 4vh;
    position: absolute;
    right: 0;
    top: 15vh;
  }

  #menu{
    display: none;
  }

  .menuSvg{
    display: block;
    position: absolute;
    right: 0;
    margin: 5vw;
    height: 50px;
    width: 50px;
    color: var(--white);
  }

  .spotifyContainer{
    width: 80%;
    display: flex;
    flex-direction: column;
    font-family: 'Urbanist', sans-serif;
    margin-bottom: 5vh;
  }

  .spotifyTitle{
    font-size: 3em;
    font-weight: var(--bold);
  }

  .spotifySubtitle{
    font-size: 2em;
    font-weight: var(--medium);
  }

  .spotifyInfo{
    display: flex;
    justify-content: space-between;
  }

  .spotifyText{
    display: flex;
    flex-direction: column;
    gap: 2vh;
    font-size: 1.8em;
  }

  #divider{
    margin: 1.5vh 0
  }

  .fullDivider{
    width: 70%;
    border: solid 1px var(--white);
    margin: 2vh 0 1vh;
  }

  .albumTop {
    flex-direction: column;
    align-items: center;
    margin: 0;
  }

  .leftContainer {
    width: 100%;
  }

  .descricaoContainer {
    display: none;
  }

  .descricaoSubContainer {
    gap: 5vh;
  }

  #albumMobile {
    display: block;
    width: 80%;
    height: auto;
  }

  #albumWeb {
    display: none;
  }

  .tracklistContainer {
    text-align: center;
  }

  .artistContainer{
    flex-direction: column;
    text-align: center;
    margin: 2vh;
  }

  .artistImg{
    width: 550px;
    height: 350px;
  }

  
}
</style>
