<template>
    <div class="home">
        <section id="about" class="container">
            <div>
             <div class="row">
                <div class="col-sm-6">
                    <h4 id="heading" class="display-4 text-liter">Hi I am <span class="">Sakhe Mzolisa</span>, an Intern Developer as well as an aspiring UX Designer & AWS Cloud Practioner.</h4>
                    <button type="button" class="btn btn-primary">
                        <a href="./Sakhe's Resume.pdf" download class="text" target="_blank"><i class="bi bi-linkedin"></i><strong>Download Cv</strong></a>
                    </button>
                </div>
                <div class="col">
                  <img class="img" src="../assets/img1.png" alt="Image">
                </div>
             </div>
            </div>
            
        </section>
    </div>
</template>
<script>
// import jsPDF from "jspdf";
export default {
    // methods: {
    //     generatePdf() {
    //         var doc = new jsPDF();
    //         doc.text(100, 100, "Hello World!");
    //         doc.save("../assets/");
    //     }
    // }
}
</script>
<style scoped>    
img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
span {
    color: #DDBEA9;
 }
 button {
    background-color: #DDBEA9;
    margin-top: 20%;
    margin-right: 50%;
    width: 30%;
}
min-height {
    min-height: 100vh;
}
a  {
    text-decoration: none;
    color: #80836C;
}

     #heading {
        /* width: 100%;
        height: 100%; */
        top: 15%;
        position: relative;
        animation: example 8s infinite;
    }
    @keyframes example {
        from {left:0% ;}
        to {left: 5%;}
     }
     @media (max-width: 768px) {
        button {
            width: 50%;
            margin: auto;
            margin-top: 0%;
        }
        img {
            width: 100%;
            padding-top: 25%;
            height: 100%;
            padding-bottom: 10%;
            margin-bottom: 5%;
            object-fit: cover;
        }
        #heading {
            width: 90%;
            height: 100%;
            top: 10%;
            position: relative;
            animation: example 8s infinite;
        }
     }
    

</style> 