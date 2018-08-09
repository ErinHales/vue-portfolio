<template>
  <div class="hello">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.2.0/css/all.css" integrity="sha384-hWVjflwFxL6sNzntih27bfxkr27PmbbK/iSvJ+a4+0owXq79v+lsFkW54bOGbiDQ"
        crossorigin="anonymous">
    <div id="homePage">
        <!-- <img class="homePageImg parallax-window" src="http://i67.tinypic.com/4uymbs.jpg" alt=""> -->
        <div class="homePageImg"></div>
        <div class="nav">
            <h3>Erin</h3>
            <div class="navButtons">
                <img src="http://i65.tinypic.com/2d7widc.jpg" alt="">
                <a href="#" v-scroll-to="{element: '#homePage', duration: 2000}"><h3>home</h3></a>
                <a href="#" v-scroll-to="{element: '#about', duration: 2000}"><h3>about</h3></a>
                <a href="#" v-scroll-to="{element: '#skills', duration: 2000}"><h3>skills</h3></a>
                <a href="#" v-scroll-to="{element: '#projects', duration: 2000}"><h3>projects</h3></a>
                <a href="#" v-scroll-to="{element: '#contact', duration: 2000}"><h3>contact</h3></a>
            </div>
        </div>
        <div id="home">
            <div class="left">
                <div class="right">
                    <div class="center">
                        <h1>Erin Hales</h1>
                        <h3>Web Developer</h3>
                    </div>
                </div>
            </div>
        </div>
        <img class="down" src="http://i64.tinypic.com/1rcb2q.jpg" alt="">
    </div>
    <div id="about">
        <!-- <img src="http://i67.tinypic.com/1o0upf.jpg" alt=""> -->
        <div class="blogs">
            <div>
                <img src="http://i67.tinypic.com/2cekeab.jpg" alt="About Me" />
                <h2>About Me</h2>
            </div>
            <div>
                <img src="http://i65.tinypic.com/t7l7gz.jpg" alt="Web Development" />
                <h2>My Journey
                    <br/> to Web Development</h2>
            </div>
            <div>
                <img src="http://i64.tinypic.com/s5cz1c.jpg" alt="work" />
                <h2>Work Experience</h2>
            </div>
        </div>
        <div id="skills">
            <h2>Skills</h2>
            <div class="skillsContainer">
                <div>
                    <img src="http://i67.tinypic.com/1674j2r.jpg" alt="">
                    <h3>JavaScript</h3>
                </div>
                <div>
                    <img src="http://i67.tinypic.com/15dmatz.jpg" alt="">
                    <h3>HTML</h3>
                </div>
                <div>
                    <img src="http://i67.tinypic.com/1zc1pnc.jpg" alt="">
                    <h3>CSS</h3>
                </div>
                <div>
                    <img src="http://i64.tinypic.com/2myq2c4.jpg" alt="">
                    <h3>React</h3>
                </div>
                <div>
                    <img src="http://i65.tinypic.com/2chm4i9.jpg" alt="">
                    <h3>jQuery</h3>
                </div>
                <div>
                    <img src="http://i66.tinypic.com/2d9xr35.jpg" alt="">
                    <h3>SQL</h3>
                </div>
                <div>
                    <img src="http://i64.tinypic.com/fvcsjs.jpg" alt="">
                    <h3>nodeJS</h3>
                </div>
                <div>
                    <img src="https://vuejsexamples.com/content/images/2017/10/vuejsexamples.png" alt="">
                    <h3>Vue</h3>
                </div>
                <div>
                    <img src="http://i65.tinypic.com/2nro8b8.jpg" alt="">
                    <h3>Angular</h3>
                </div>
            </div>
        </div>
        <h2 id="projectsHeader">Projects</h2>
        <div id="projects">
            <div class="project">
                <img src="http://i65.tinypic.com/1sh5ip.jpg" alt="">
                <p>Ozzy is a parenting application designed to help parents and care providers connect and communicate. It was
                    designed as a personal project during my time at Dev Mountain. It is one of my larger projects and won
                    the award for "Best Overall App".</p>
                <button>Read More
                    <i class="fa fa-angle-double-right"></i>
                </button>
            </div>
            <router-link to="/journey"><div class="project">
                <img src="http://i63.tinypic.com/iqvj49.jpg" alt="">
                <p>This is a calendar application also built during Dev Mountain. It was a very technical piece. Because of
                    the way we measure time, I had to create a lot of algorithms to display the dates correctly and to make
                    events show up in the right spot.</p>
                <button>Read More
                    <i class="fas fa-angle-double-right"></i>
                </button>
            </div></router-link>
            <div class="project">
                <img src="http://i63.tinypic.com/bfnxv4.jpg" alt="">
                <p>This weather app was built as part of the Free Code Camp curriculum. I built it on my own after 2 months
                    of studying code in my free time. It uses the Open Weather API and gives the current weather as well
                    as a three day forecast.</p>
                <button>Read More
                    <i class="fas fa-angle-double-right"></i>
                </button>
            </div>
        </div>
        <form id="contact">
            <input type="text" placeholder="Name">
            <input type="text" placeholder="Email">
            <input type="text" placeholder="Subject">
            <textarea name="" id="" cols="30" rows="10" placeholder="Message"></textarea>
            <div>
                <button>Clear</button>
                <button>Send</button>
            </div>
        </form>
    </div>
  </div>
</template>

<script>
import Vue from 'vue';
import VueScrollTo from 'vue-scrollto';
// import router from '../Router.vue';
Vue.use(VueScrollTo);
// import Icon from 'vue-awesome/components/Icon';

export default {
  name: "Home",
  // components: Icon,
  mounted () {
    // let scrollpos = window.scrollY;
    // const header = document.querySelector("nav");
    // // const header_height = header.offsetHeight;

    // const add_class_on_scroll = () => header.classList.add("showNav");
    // const remove_class_on_scroll = () => header.classList.remove("showNav");

    // window.addEventListener('scroll', function() {
    //   scrollpos = window.scrollY;
    //   if (scrollpos >= 200) {
    //     add_class_on_scroll();
    //   } else {
    //     remove_class_on_scroll();
    //   }
    // });
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* light green/gray = B8D8D8
medium green/gray = 7A9E9F
dark green/gray = 4F6367
cream = EEF5DB
coral = FE5F55 
right coral = F4B196
dark blue = 076982*/

/* http://meyerweb.com/eric/tools/css/reset/ 
  v2.0 | 20110126
  License: none (public domain)
*/
/* * {
  margin:0;
  padding: 0;
  box-sizing: border-box;
} */

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}
body {
  line-height: 1;
  width: 100vw;
}
ol,
ul {
  list-style: none;
}
blockquote,
q {
  quotes: none;
}
blockquote:before,
blockquote:after,
q:before,
q:after {
  content: "";
  content: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}

button {
  outline: none;
  cursor: pointer;
}

input {
  outline: none;
}

@import url("https://fonts.googleapis.com/css?family=Josefin+Sans");

body {
  scroll-y: hidden;
}

p {
  text-indent: 30px;
  margin-bottom: 20px;
}

.homePageImg {
  height: 100%;
  margin: 0px;
  padding: 0px;
  position: fixed;
  width: 100vw;
  background-image: url("http://i67.tinypic.com/4uymbs.jpg");
  background-size: cover;
  z-index: -2;
}

.nav {
  position: fixed;
  top: 0px;
  color: white;
  font-family: "Josephin Sans", sans-serif;
  font-size: 30px;
  display: flex;
  justify-content: space-between;
  width: 100vw;
  background-color: rgba(244, 177, 150, 0);
  z-index: 1;
}

.showNav {
  --ease: all 1000ms ease;
  /* background-color: white; */
  transition: var(--ease);
  background-color: rgba(244, 177, 150, 1);
}

.nav > h3,
.navButtons h3 {
  display: inline-block;
  padding: 15px;
}

.navButtons h3 {
  cursor: pointer;
  transition: transform 0.3s linear;
  color: white;
}

.navButtons {
  padding-right: 30px;
}

#home {
  position: absolute;
  top: 35vh;
  width: 30%;
  left: 35%;
}

#home .left {
  border: 2px solid #044252;
  position: relative;
  top: -10px;
  left: -10px;
  width: 100%;
  height: 100%;
}

#home .right {
  width: 100%;
  height: 100%;
  top: 29%;
  left: 39%;
  border: 2px solid #044252;
  position: relative;
  top: 10px;
  left: 10px;
}
#home .center {
  margin: 40px;
}

#home h1 {
  font-size: 6vw;
  text-align: center;
}

#home h3 {
  font-size: 4vw;
  text-align: center;
  padding: 10px;
}

.navButtons > h3:active {
  border-bottom: 4px solid #f4b196;
}

.navButtons > h3:hover {
  transform: scale(1.07);
}

.navButtons img {
  display: none;
  height: 50px;
  margin: 10px;
}

.down {
  position: absolute;
  margin-left: calc(50vw - 25px);
  width: 50px;
  top: 87vh;
  text-align: center;
  animation: bounce 2s infinite;
}

#about {
  background-color: rgba(255, 255, 255, 0.5);
  position: absolute;
  top: 100vh;
}

.blogs {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin-top: 100px;
  margin-bottom: 100px;
  width: 99vw;
}

.blogs > div {
  width: 300px;
  height: 300px;
  font-size: 30px;
  background-color: #076982;
  color: white;
  padding: 50px;
  text-align: center;
  transition: transform 0.5s linear;
  margin: 100px;
}

.blogs > div:hover {
  cursor: pointer;
  transform: scale(1.07);
}

.blogs img {
  width: 200px;
  margin-bottom: 20px;
}

#skills {
  background-color: #f4b196;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.skillsContainer {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  width: 1200px;
}

#skills div {
  padding: 60px;
  text-align: center;
}

#skills h3 {
  font-size: 30px;
  margin: 20px;
  /* text-shadow: 2px 2px rgba(0,0,0,0.5); */
}

#skills h2 {
  font-size: 40px;
  padding: 20px;
  padding-top: 90px;
  text-align: center;
}

#skills img {
  width: 50px;
}

#projects {
  background-color: transparent;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  padding-top: 100px;
}

.project {
  /* background-color: #076982; */
  background-color: rgba(255, 255, 255, 0.5);
  /* color: white; */
  color: #044252;
  margin: 50px;
  padding: 20px;
  width: 400px;
  font-size: 20px;
  text-align: center;
}

.project button {
  background-color: #044252;
  color: white;
  font-size: 20px;
  border: none;
  padding: 10px;
}

.project p {
  margin-top: 10px;
}

.project img {
  width: 80%;
}

form {
  background-color: rgba(255, 255, 255, 0.5);
  width: 80%;
  margin-left: 10%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-bottom: 100px;
  margin-top: 100px;
}

form input {
  width: 60%;
  background-color: transparent;
  border: none;
  border-bottom: 3px solid gray;
  margin: 20px;
  font-size: 50px;
}

textarea {
  width: 60%;
  background-color: transparent;
  font-size: 30px;
}

form button {
  background-color: #044252;
  color: white;
  border: none;
  font-size: 30px;
  padding: 20px;
  margin: 20px;
}

#projectsHeader {
  font-size: 40px;
  text-align: center;
  margin-top: 100px;
}

@keyframes bounce {
  70% {
    transform: translateY(20px);
  }
  100% {
    transform: translateY(0px);
  }
}

@media (max-width: 1300px) {
  .blogs div {
    width: 200px;
    height: 200px;
    margin: 100px 50px 100px 50px;
  }
  .blogs img {
    width: 100px;
  }
  #home {
    width: 40%;
    left: 30%;
  }
}

@media (max-width: 1200px) {
  .skillsContainer {
    width: 100vw;
  }
  #skills {
    width: 100vw;
  }
  #home {
    width: 50%;
    left: 25%;
  }
  .content {
    width: 80%;
  }
}

@media (max-width: 1000px) {
  #home h1 {
    font-size: 8;
  }
  #home h2 {
    font-size: 6;
  }
  form input {
    width: 80%;
  }
  textarea {
    width: 80%;
  }
}

@media (max-width: 800px) {
  #skills h3 {
    margin: 10px;
  }
  form {
    width: 100%;
    margin-left: 0px;
    margin-bottom: 0px;
  }
  textarea {
    height: 300px;
  }
  form input {
    font-size: 30px;
  }
  .navButtons h3 {
    display: none;
  }
  .navButtons img {
    display: block;
  }
  .content {
    width: 90%;
  }
}

@media (max-width: 540px) {
  #home {
    width: 80%;
    left: 10%;
    top: calc(50vh - 100px);
  }
  #home h1 {
    font-size: 10vw;
  }
  #home h2 {
    font-size: 8vw;
  }
  .skillsContainer {
    flex-direction: column;
  }
  .project {
    width: 300px;
  }
}
</style>
