<template>
  <div id="app">
    <section class="hero is-primary is-bold is-fullheight">
      <!-- Hero head: wiil stick at the top -->
      <div class="hero-head">
        <nav class="navbar">
          <div class="container">
            <div class="navbar-brand">
              <a class="navbar-item">
                VueJs To-Do List
              </a>
            </div>
          </div>
        </nav>
      </div>

      <!-- Hero content: wiil be in the middle -->
      <div class="hero-body">
        <div class="container has-text-centered">
          <div class="row">
            <div class="columns">
              <div class="column is-half is-offset-one-quarter">
                <todo-card></todo-card>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Hero footer: wiil stick at the bottom -->
      <div class="hero-foot">
        <div class="container">
          <div class="content has-text-centered">
            <p>
              <strong>VueJs To-Do List</strong> by <a href="http://github.com/guifrribeiro">Guilherme Ferreira</a>
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import TodoCard from './components/TodoCard'

export default {
  name: 'app',
  components: {
    TodoCard
  },
  data () {
    return {
      msg: 'Welcome to My To-Do List'
    }
  }
}
</script>

<style>
</style>
