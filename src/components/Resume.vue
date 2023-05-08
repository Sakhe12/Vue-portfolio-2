<template lang="">
    <div>
      <div class="timeline">
  <div class="container left">
    <div class="content">
      <h3>2023</h3>
      <h4>Life Choices Academy Lecturer Assistant</h4>
      <p>My main duties as a lecturer assistant was to assist the lecturers with admin as well as to lend a helping hand to the students with coding relating matters as well as being a motivator to them. I am doing this alongside being an intern developer</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h3>2023</h3>
      <h4>LC Studio Intern Developer</h4>
      <p>I am currently in an internship  program at LC Studio, a web development agency for Life Choices, where we have been working on real-world projects and we also upskill ourselves further.</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h3>2022-23</h3>
      <h4>Life Choices Academy student</h4>
      <p>Amongst the tech skills I was also taught soft skills at this wonderful institution. Soft skills which will help me greatly in life as I have gained the ability to reason properly with people.</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h3>2020-22</h3>
      <h4>Mr D Food Flexi Perm Customer Service Agent</h4>
      <p>Resolving order related queries and troubleshooting any app or order issues which may or have disturb the customers purchase journey as well dealing with escalations, which are not limited to driver complaints and restuarants</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h3>2018-2021</h3>
      <h4>University of The Western Cape</h4>
      <p>I unfortunately was not able to to complete my BA degree due to funding related issues. I was majoring in Political Studies and History</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h3>2013-2017</h3>
      <h4>Goodwood College</h4>
      <p>I passed my matric with an admission to bachelors degree pass</p>
    </div>
  </div>
</div>
    </div>
</template>
<script>
export default {
    name: "work",
    data() {
        return {
          jobs : [
          { 
            title: "Lecturer Assistant",
            company: "Life Choices Academy",
            duration: "May 2023",
            description: "My main duties as a lecturer assistant was to assist the lecturers with admin as well as to lend a helping hand to the students with coding relating matters as well as being a motivator to them. I am doing this alongside being an intern developer"
          },
          { 
            title: "Intern Developer",
            company: "LC Studio",
            duration: "March 2023",
            description: "I am currently in an internship  program at LC Studio, a web development agency for Life Choices, where we have been working on real-world projects and we also upskill ourselves further."
          },
          { 
            title: "Flexi Perm Customer Service Agent",
            company: "Mr D Food",
            duration: "March 2020 - September 2023",
            description: ""
          }
          ],
          academics: [
            {
              occupation: "Student",
              institution: "Life Choices Academy",
              year: "September 2022 - March 2023",
              text: "I was studying web development doing both front end and backend development"
            },
            {
              Occupation: "Student",
              institution: "University of The Western Cape",
              year: "February 2018 - 2020",
              text: "I unfortunately was not able to to complete my BA degree due to funding issues"
            },
            {
              Occupation: "Student",
              institution: "Goodwood College",
              year: "January 2017 - 2017",
              text: "I passed my matric with an admission to bachelors degree pass"
            },
          ]
        }
    }
}
</script>
<style scoped>
    * {
  box-sizing: border-box;
}

body {
  background-color: #474e5d;
  font-family: Helvetica, sans-serif;
}

/* The actual timeline (the vertical ruler) */
.timeline {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
}

/* The actual timeline (the vertical ruler) */
.timeline::after {
  content: '';
  position: absolute;
  width: 6px;
  background-color: #000000;
  top: 0;
  bottom: 4.1%;
  left: 50%;
  margin-left: -3px;
}

/* Container around content */
.container {
  padding: 10px 40px;
  position: relative;
  padding-bottom: 7%;
  background-color: inherit;
  width: 50%;
}

/* The circles on the timeline */
.container::after {
  content: '';
  position: absolute;
  width: 25px;
  height: 25px;
  right: -17px;
  background-color: #D9D9D9;
  border: 4px solid #DDBEA9;
  top: 15px;
  border-radius: 50%;
  z-index: 1;
}

/* Place the container to the left */
.left {
  right: 25.5%;
}

/* Place the container to the right */
.right {
  left: 25.5%;
}

/* Add arrows to the left container (pointing right) */
.left::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  right: 30px;
  border: medium solid white;
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent white;
}

/* Add arrows to the right container (pointing left) */
.right::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  left: 30px;
  border: medium solid #DDBEA9;
  border-width: 10px 10px 10px 0;
  border-color: transparent #DDBEA9 transparent transparent;
}

/* Fix the circle for containers on the right side */
.right::after {
  left: -16px;
}

/* The actual content */
.content {
  padding: 20px 30px;
  background-color: #DDBEA9;
  opacity: 90%;
  position: relative;
  border-radius: 6px;
  box-shadow: 0px 0px 15px #f181bd;
}

/* Media queries - Responsive timeline on screens less than 600px wide */
@media screen and (max-width: 600px) {
  /* Place the timelime to the left */
  .timeline::after {
  left: 31px;
  }
  
  /* Full-width containers */
  .container {
  width: 100%;
  padding-left: 70px;
  padding-right: 25px;
  }
  
  /* Make sure that all arrows are pointing leftwards */
  .container::before {
  left: 60px;
  border: medium solid white;
  border-width: 10px 10px 10px 0;
  border-color: transparent white transparent transparent;
  }

  /* Make sure all circles are at the same spot */
  .left::after, .right::after {
  left: 15px;
  }
  
  /* Make all right containers behave like the left ones */
  .right {
  left: 0%;
  }
  .left {
    right: 0%;
  }
}
</style>