<template lang="">
    <div>
        <div class="container">
            <div class="row">
                <div class="col-sm-6 touch">
                    <h1><strong>Let Us get in touch</strong></h1>
                    <p class="text-muted"><i class="bi bi-geo-alt-fill"></i>24 New Rest, Gugulethu,</p>
                    <p class="text-muted"><i class="bi bi-phone"></i>083 282 8451</p>
                    <p class="text-muted"><i class="bi bi-envelope-fill"></i>sakhemzolisa@gmail.com</p>
                    <div class="icons gap-3">
                        <a href="https://www.linkedin.com/in/sakhe-mzolisa-507588230/" target="_blank"><i class="bi bi-linkedin"></i></a>
                        <a href="https://github.com/Sakhe12" target="_blank"><i class="bi bi-github"></i> </a>
                        <a href="https://twitter.com/MzolisaSakhe" target="_blank"><i class="bi bi-twitter"></i></a>
                    </div>
                </div>
                <div class="col Contact">
                    <h2 class="display-2">Contact</h2>
            <form
            action="https://formspree.io/f/mlevoeqb"
            method="post"
            >
                <div class="mb-3 text-center">
                    <label for="exampleInput
                    tName" class="form-label"></label>
                    <input type="text" class="form-control" id="exampleInputName1" placeholder="Enter your name" name="fullname" aria-describedby="nameHelp" required>
                  </div>
                  <div class="mb-3 text-center">
                    <label for="exampleInputSurname
                    tName" class="form-label"></label>
                    <input type="text" class="form-control" id="exampleInputSurname1" placeholder="Enter your surname" name="Surname" aria-describedby="surnameHelp" required>
                  </div>
                <div class="mb-3 text-center">
                  <label for="exampleInputEmail1" class="form-label"></label>
                  <input type="email" class="form-control" id="exampleInputEmail1" placeholder="you@mail.com" name="Email" aria-describedby="emailHelp" required>
                  <div id="emailHelp" class="form-text">This is confidential information </div>
                </div>
                <div class="mb-3 text-center">
                  <label for="exampleInputmessage1" class="form-label"></label>
                  <!-- <textarea name="" id="" cols="30" rows="10"></textarea> -->
                  <input type="text" class="form-control" id="exampleInputmessage1" placeholder="text..." name="message" required>
                  <div id="messagedHelp" class="form-text"></div>
                </div>
                <button type="submit" class="btn btn-success">Submit</button>
              </form>

                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    input {
        background-color: #DDBEA9;
        opacity: 70%;
        border-radius: 5px #DDBEA9;
    }
    h2 {
        color: black;
    }
    button { 
        background-color: #DDBEA9;
    }
    .Contact {
        padding-top: 5%;
    }
    .touch {
        padding-top: 15%;
        color: black;
    }
    .icons a {
  display: inline-block;
  padding: 10px;
  font-size: 1.5rem;
  color: #333;
  transition: all 0.3s ease;
}

.icons a:hover {
  color: #fff;
  text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 30px #fff, 0 0 40px #33ff33, 0 0 70px #33ff33, 0 0 80px #33ff33, 0 0 100px #33ff33;
}

    a {
        color: black;
    }
    .icons {
        display: flex;
        align-items: center;
        justify-content: center;
      }
    p { 
        padding-top: 5%;
    }
</style>