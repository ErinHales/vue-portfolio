<template>
<div class="journey">
    <div class="circle">
        <img src="http://i65.tinypic.com/t7l7gz.jpg" alt="Web Development" />
    </div>
    <div class="content">
        <p>I never expected to be a web developer. It's not that I had any bias against it, but rather that it was never
                    an option. I simply didn't know about it. It wasn't until 2017 that I had a discussion with an old friend
                    who is now a web developer. This encouraged me to look into the field. What I found was that I loved
                    it! It satisfied my itch for problem solving and also design. I found that hours spent in front of the
                    computer passed quickly.</p>
        <p>When I decided to go to Dev Mountain (a three month intensive program), I knew that it was going to be a
                    really hard thing, so I spent months preparing. Every day when I got home from work, I would spend 3-4
                    hours going through courses on Free Code Camp and building small projects. I learned that I was good
                    at coding and quick at catching on to new topics.</p>
        <p>Dev Mountain was an amazing experience, and it helped me realize that I can do hard things. And now that it's behind me, I am eager to start the next phase of my career as a web developer.</p>
    </div>
    <button class="back">Back</button>
</div>
</template>

<script src="https://unpkg.com/vue/dist/vue.js"></script>
<script src="https://unpkg.com/vue-router/dist/vue-router.js"></script>

<script>
export default {
    name: "Journey",
    mounted() {
        console.log("Journey component mounted successfully");
    }
}
</script>

<style>
.journey,
.aboutMePage,
.workPage {
    width: 100vw;
    height: 100vh;
    color: white;
    font-size: 25px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #076982;
}

.circle {
    border-radius: 50%;
    background-color: rgba(255,255,255,0.2);
    padding: 40px;
    margin-bottom: 50px;
}

.circle img {
    width: 100px;
}

.content {
    width: 60%;
}

.back {
    background-color: #044252;
    border-radius: 30px;
    border: none;
    margin: 20px;
    font-size: 30px;
    color: white;
    padding: 10px;
}
</style>