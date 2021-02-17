<template>
  <main>
    <div class="background">
      <app-masthead/>
    </div>
    <div class="headings">
          <h1 class="title">
      smashing fuck
    </h1>
    <div v-for=""></div>
    <p>Pleas eat</p>
    </div>
    <div class="links"><p>Got follow Maller</p></div>
    <div class="nextpage">Projects</div>
    
  </main>
</template>

<script>
import AppMasthead from'~/components/AppMasthead.vue'

export default {
  components: {
    AppMasthead
  }
}
</script>

<style>
main { 
  width: 100vw;
  height: calc(100vh - 100px);
  display: grid; 
  grid-template-columns: 100px repeat(4, 1fr); 
  grid-template-rows: repeat(3, 1fr) 50px 100px; 
  grid-column-gap: 0px;
  grid-row-gap: 0px; 
}
.background { grid-area: 1 / 3 / 5 / 6; } 
.headings { grid-area: 2 / 2 / 3 / 6; } 
.links { grid-area: 5 / 1 / 6 / 5; padding: 30px;} 
.nextpage { grid-area: 4 / 5 / 6 / 6; background: #eee; color: black; padding: 30px } 
</style>
