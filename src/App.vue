<template>
    <div id="app" class="section">
        <div class="container sidebar">
            <Sidebar/>
        </div>
        <div class="container columns landing-page">
            <Home/>
        </div>
        <footer>
            <p>Copyright © 2020 Avokado Health - Keto & Low-carb Meal Planner</p>
        </footer>
    </div>
</template>

<script>
import Home from './components/Home.vue';
import Sidebar from './components/Sidebar.vue';

export default {
  name: 'App',
  components: {
    Home, Sidebar
  }
}
</script>

<style>
    #app {
        padding-bottom: 0.5rem;
    }
    footer p {
        font-size: 0.75rem;
        text-align: right;
    }
</style>
