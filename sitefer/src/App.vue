<template>
  <div id="app">
    <b-sidebar 
    visible="true" 
    noCloseOnBackdrop="true"
    noCloseOnEsc="true"
    noCloseOnRouteChange="true">
      <nav class="mb-3">
        <b-nav vertical>
          <b-nav-item>
            <router-link to="/">Home</router-link>
          </b-nav-item>
          <b-nav-item>
            <router-link to="/about">About</router-link>
          </b-nav-item>
        </b-nav>
      </nav>
    </b-sidebar>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

button.close.text-dark {
  visibility: hidden;
}
</style>
