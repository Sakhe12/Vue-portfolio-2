<template lang="">
    <div>
        <div class="container-fluid test">
            <div class="row gap-5 mx-5 d-sm-flex justify-content-center">
                    <div v-for="humans in testimonials" :key="humans" class="card" style="width: 18rem;">
                        <img :src="humans.image" class="card-img-top" alt="...">
                        <div class="card-body">
                          <h5 class="card-title">{{humans.name}}</h5>
                          <p class="card-text">{{humans.text}}</p>
                        </div>
                      </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "humans",
    data() {
        return {
            testimonials : [
                {
                    image : "https://i.postimg.cc/QdCvRYV6/Joel-Profile.jpg",
                    name : "Joel Mukanya",
                    text : "Sakhe is a very creative, and a well-behaved student. He does enjoy working with his classmates and works well on his project. He has gained knowledge of web development, including Bootstrap 5. I will be very delighted to see him get hired as a developer."
                },
                {
                    image : "https://i.postimg.cc/ncQHXr0n/DSC-3597.jpg",
                    name : "Deno Rautenbach",
                    text : "Sakhe is a born leader. Political in his approach, firm in his execution. I believe his capabilities have been circumcised and that with the right methodology, can reach their peak. Yet for now, he's a dependable source of knowledge to anyone that needs an explanation simplified into plain words, the way of learning should be implemented."
                },
                {
                    image : "https://i.postimg.cc/HW00f9Wp/C11-Sibabalwe-Mafestire-1.jpg",
                    name : "Sibabalwe Mafestire",
                    text : "Sakhe is a go getter, dedicated and committed to his work, open minded and always looks forward to growth and developing his skills. Time oriented, and successfully completes his work before deadlines and is a very good team player."
                },
                {
                    image : "https://i.postimg.cc/9MxgMX7y/candice-2022.jpg",
                    name : "Candice Anon",
                    text : "Sakhe is always ready to engage with any activity, not afraid to give his opinion and he is very outspoken. Change is what drives him. Key qualities that describe Sakhe is passion, education and growth. Shows great leaderships skills"
                },
                {
                    image : "https://i.postimg.cc/c4LqwjFX/DSC-3517.jpg",
                    name : "Lindokuhle Mgoqi",
                    text : "Sakhe has an amazing amount of willingness and he never leaves a task incomplete, He is also a social butterfly and works well with others."
                },
                {
                    image : "https://i.postimg.cc/wMgwy3VW/C11-Brandon-Swinton-1.jpg",
                    name : "Brandon Swinton",
                    text : "Sakhe Mzolisa is hard working guy who completes every project and reaches every goal that he sets for himself. He is a selfless peer who go out of his way to assist others if they are having trouble with something. He is friendly and respectful which makes him perfect for the work-environment.",
                }
            ]
        }
    },
}
</script>
<style scoped >
.card {
    background-color: #DDBEA9;
    opacity: 70%;
    margin-top: 5%;
    padding-top: 2%;
    transform-origin: 50% 50;
    animation: scaledown ,5s linear;
    animation-fill-mode: forwards;
}
.card:hover {
    transform-origin: 50% 50;
    animation: down 5s linear;
    animation-fill-mode: forwards;
    z-index: 100;
}
@keyframes down {
    100%{
        transform: scale(1);
    }
    0%{transform: scale(1.2);
    }
}
@keyframes down {
    100%{
        transform: scale(1);
        box-shadow: var(--shadow);
    }
    0%{transform: scale(1.2);
    }
}
.test {
    padding-bottom: 3rem;
}
</style>