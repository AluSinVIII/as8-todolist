
<template>
  <div id="app">
     <section class="hero is-warning is-bold is-fullheight">
      <div class="hero-body">
        <div class="container has-text-centered">
          <h1 class="title">{{msg}}</h1>
        </div>
      </div>
      <ToDoCard></ToDoCard>

      <div class="hero-foot">
        <div class="container">
          <div class="content has-text-centered pb-5">
            <p>
              <strong>Atelier Mars 2021</strong>
            </p>
            <p>
              Découvrez comment styliser simplement votre ToDo list avec 
              <a class="has-text-primary" href="https://bulma.io/">
                <strong>Bulma</strong>
              </a> 
            </p>
          </div> 
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import ToDoCard from './components/ToDoCard.vue'
export default {
  name: 'app',
  components: {
    ToDoCard
    
  },
  data () {
    return {
      msg: 'Test'
    }
  }
}
</script>

<style>
</style>