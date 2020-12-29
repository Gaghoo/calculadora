<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/calc">Calculadora</router-link>
    </div>
    <div class="main">
      <router-view/>
    </div>
  </div>
</template>

<style>
*{
  box-sizing: border-box;
  padding: 0;
  margin: 0%;
}
#app {
  font-family: 'Times New Roman', Times, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  background: linear-gradient(to right, #f0f2f0, #000c40);

}

.main{
  display: flex;
  flex-direction: column;
  height: calc(100vh - 60px);
  justify-content: center;
  align-items: center;
}

#nav {
  height: 60px;
  background: #000a4062;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
}

#nav a {
  padding: 10px;
  font-weight: bold;
  color: #afd1f3;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
