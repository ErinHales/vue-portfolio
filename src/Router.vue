<template>

</template>

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
    { path: '/home', name: "Home", component: Home },
    { path: '/about', name: "About", component: About },
    { path: '/work', name: "Work", component: Work },
    { path: '/journey', name: "Journey", component: Journey }
]
const router = new VueRouter({
    routes
})

const app = new Vue({
    router
}).$mount('#app')
</script>