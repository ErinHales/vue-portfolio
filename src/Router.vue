<template>

</template>

<script src="https://unpkg.com/vue/dist/vue.js"></script>
<script src="https://unpkg.com/vue-router/dist/vue-router.js"></script>

<script>
// import Home from './components/Home';
// import About from './components/About';
// import Work from './components/Work';
// import Journey from './components/Journey';
const Home = require('./components/Home');
const About = require('./components/About');
const Work = require('./components/Work');
const Journey = require('./components/Journey');

const routes = [
    { path: '/home', component: Home },
    { path: '/about', component: About },
    { path: '/work', component: Work },
    { path: '/journey', component: Journey }
]
const router = new VueRouter({
    routes
})

const app = new Vue({
    router
}).$mount('#app')
</script>