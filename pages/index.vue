<template>
  <div>
    <banner/>
    <about/>
    <team/>
    <work/>
    <services/>
  </div> 
</template>

<script>
import Banner from '~/components/Banner.vue'
import About from '~/components/About.vue'
import Team from '~/components/Team.vue'
import Work from '~/components/Work.vue'
import Services from '~/components/Services.vue'

export default {
  components: {
    banner: Banner,
    about: About,
    team: Team,
    work: Work,
    services: Services
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quattrocento Sans', sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
