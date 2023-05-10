<template lang="">
    <div>
        <div class="container-fluid tasks">
            <div class="row gap-5 mx-4 d-sm-flex justify-content-center">
                <h2 class="display-2"><strong>Projects</strong></h2>
                <div v-for="work in projects" :key="work" class="card cards" style="width: 18rem;">
                    <img :src="work.img" class="card-img-top pic" alt="...">
                    <div class="card-body">
                      <h5 class="card-title">{{work.task}}</h5>
                      <div class="icons">
                          <a :href="work.weblink" target="_blank" class="btn btn-danger">Browser</a>
                          <a :href="work.github" target="_blank" class="btn btn-dark">Github</a>
                      </div>
                    </div>
                  </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name : "work",
    data() {
        return {
          projects : [
            {
                img : "https://i.postimg.cc/pd6641V5/calculator.gif",
                task : "Calculator",
                weblink : "https://winxcalculator.netlify.app/",
                github : "https://github.com/Sakhe12/calculator.git"
            },
            {
                img : "https://i.postimg.cc/tgcxL816/atm.gif",
                task : "Footyhub",
                weblink : "https://footyhub-823968.netlify.app/",
                github : "https://github.com/Sakhe12/jsfinalproject"
            },
            {
                img : "https://i.postimg.cc/PrfmcgK6/wireframe.gif",
                task : "Portfolio",
                weblink : "https://sakhe.netlify.app/",
                github : "https://github.com/Sakhe12/Portfolio.git"
            },
            {
                img : "https://i.postimg.cc/RF77LNHt/browser.gif",
                task : "Vue-end of Module",
                weblink : "https://vuejs-finalproject-ba333.web.app/",
                github : "https://github.com/Sakhe12/vuejs-finalproject.git"

            },
            {
                img : "https://i.postimg.cc/0QNfP7XC/idea.gif",
                task : "Footyhub(mock)",
                weblink : "https://astonishing-hamster-68f43f.netlify.app/",
                github : "https://github.com/Sakhe12/bootstrap-challenge.git"

            },
            {
                img : "https://i.postimg.cc/hvxqg2rk/resize.gif",
                task : "Project",
                weblink : "https://lifechoices1.netlify.app/",
                github : "https://github.com/Sakhe12/life-choices.git"
            },
            {
                img : "https://i.postimg.cc/hvxqg2rk/resize.gif",
                task : "Capstone",
                weblink : "https://isipho-bb5e9.web.app/",
                github : "https://github.com/Sakhe12/Isipho-Capstone-project.git"
            },
          ]  
        }
    },
}
</script>
<style scoped>
.tasks {
    min-height: 100vh;
    padding-bottom: 3rem;
}

.cards {
    background-color: #DDBEA9;
    opacity: 70%;
    padding-top: 2%;
}

</style>