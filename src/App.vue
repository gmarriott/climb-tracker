<template>
  <div id="app">
    <b-navbar toggleable="sm" type="light" variant="light">
    <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>

    <b-navbar-brand>Climb Tracker</b-navbar-brand>
      <b-navbar-nav>
        <b-nav-text class="pr-4">Track your climbing progression!</b-nav-text>
         <b-nav-item><router-link to="/">Home <font-awesome-icon :icon="['fa', 'mountain']"/></router-link></b-nav-item>
        <b-nav-item><router-link to="/time-entries">Time Entries <font-awesome-icon :icon="['far', 'clock']"/></router-link></b-nav-item>
      </b-navbar-nav>
  </b-navbar>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
