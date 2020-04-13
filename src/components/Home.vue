<template>
    <div class="vh-100 w-100" :style="cssProps">
        <b-container class="h-75 d-flex">
            <b-jumbotron class="my-auto w-100" header="Climb Tracker" lead="A new way to track your progression as a climber!">
                <b-img :src="require('@/assets/bouldering-icon.png')"></b-img>
                <hr>
                <b-button variant="primary" href="#">Start Your Track Now</b-button>
            </b-jumbotron>
        </b-container>
    </div>
</template>
<script>
export default {
  name: 'home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      cssProps: {
        backgroundImage: `url(${require('@/assets/background.jpg')})`
      }
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.jumbotron {
    opacity: 0.9;
}
</style>
