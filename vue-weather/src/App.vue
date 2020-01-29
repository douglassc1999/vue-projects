<template>
  <!-- Stop in minute 12 -->
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" class="search-bar" placeholder="Buscar...">
        <div class="weather-wrap">
          <div class="location-box">
            <div class="location">Natal, RN</div>
            <div class="date">Tuesday 28 January 2020</div>
          </div>

          <div class="weather-box">
            <div class="temp">9 °C</div>
            <div class="weather">Rain</div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>

export default {
  name: 'app',
  data() {
    return {
      api_key: 'ca2d4d9dbacef82920a670b94fb3cb2c'
    }
  }
}

</script>

<style>
* {
   margin: 0;
   padding: 0;
   box-sizing: border-box;
}

body {
  font-family: 'montserrat', sans-serif;

}

#app {
  background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}

main {
  min-height: 100vh;
  padding: 25px;

  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.75));
}

.search-box {
  width: 100%;
  margin-bottom: 30px;
}

.search-box .search-bar {
  display: block;
  width: 100%;
  padding: 15px;

  color: #313131;
  font-size: 20px;

  appearance: none;
  border: none;
  outline: none;
  background: none;

  box-shadow: 0px 0px 8px rgba(0, 0, 0, 0.25);
  background-color: rgba(255, 255, 255, 0.5);
  border-radius: 0px 16px 0px 16px;
  transition: 0.4s; 
}

.search-box .search-bar:focus {
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.75);
  background-color: rgba(255, 255, 255, 0.75);
  border-radius: 16px 0px 16px 0px;
}
</style>
