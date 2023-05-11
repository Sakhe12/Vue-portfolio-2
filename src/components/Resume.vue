<template lang="">
    <div>
      <h1>UL timeline cards</h1>
<ul>
    <li style="--accent-color:#DDBEA9">
        <div class="date">2023</div>
        <div class="title">Life Choices Academy</div>
        <div class="descr">My main duties as a lecturer assistant was to assist the lecturers with admin as well as to lend a helping hand to the students with coding relating matters as well as being a motivator to them. I am doing this alongside being an intern developer</div>
    </li>
    <li style="--accent-color:#42b983">
        <div class="date">2023</div>
        <div class="title">LC Studio</div>
        <div class="descr"></div>I am currently in an internship  program at LC Studio, a web development agency for Life Choices, where we have been working on real-world projects and we also upskill ourselves further.
    </li>
    <li style="--accent-color:#DDBEA9">
        <div class="date">2022-23</div>
        <div class="title">Life Choices Academy student</div>
        <div class="descr">Amongst the tech skills I was also taught soft skills at this wonderful institution. Soft skills which will help me greatly in life as I have gained the ability to reason properly with people.</div>
    </li>
    <li style="--accent-color:#42b983">
        <div class="date">2020-22</div>
        <div class="title">Mr D Food Flexi Perm Customer Service Agent</div>
        <div class="descr">Resolving order related queries and troubleshooting any app or order issues which may or have disturb the customers purchase journey as well dealing with escalations, which are not limited to driver complaints and restuarants</div>
    </li>
    <li style="--accent-color:#DDBEA9">
        <div class="date">2018-21</div>
        <div class="title">University of The Western Cape</div>
        <div class="descr">I unfortunately was not able to to complete my BA degree due to funding related issues. I was majoring in Political Studies and History</div>
    </li>
    <li style="--accent-color:#42b983">
        <div class="date">2013-17</div>
        <div class="title">Goodwood College</div>
        <div class="descr">I passed with an admission to bachelors pass.</div>
    </li>
</ul>
<div class="credits"><a target="_blank" href="https://www.freepik.com/free-vector/infographic-template-with-yearly-info_1252895.htm">inspired by</a></div>
<div class="container">
  <i class="fa-brands fa-html5 fa-lg"></i>
  <i class="fa-brands fa-css3-alt fa-lg"></i>
  <i class="fa-brands fa-vuejs fa-lg"></i>
  <i class="fa-brands fa-node fa-lg"></i>
  <FontAwesomeIcon icon="fa-brands fa-figma" size="lg" />
  <FontAwesomeIcon icon="fa-brands fa-wordpress" size="lg" />

</div>
    </div>
</template>
<script>
export default {
    // name: "work",
    // data() {
    //     return {
    //       jobs : [
    //       { 
    //         title: "Lecturer Assistant",
    //         company: "Life Choices Academy",
    //         duration: "May 2023",
    //         description: "My main duties as a lecturer assistant was to assist the lecturers with admin as well as to lend a helping hand to the students with coding relating matters as well as being a motivator to them. I am doing this alongside being an intern developer"
    //       },
    //       { 
    //         title: "Intern Developer",
    //         company: "LC Studio",
    //         duration: "March 2023",
    //         description: "I am currently in an internship  program at LC Studio, a web development agency for Life Choices, where we have been working on real-world projects and we also upskill ourselves further."
    //       },
    //       { 
    //         title: "Flexi Perm Customer Service Agent",
    //         company: "Mr D Food",
    //         duration: "March 2020 - September 2023",
    //         description: ""
    //       }
    //       ],
    //       academics: [
    //         {
    //           occupation: "Student",
    //           institution: "Life Choices Academy",
    //           year: "September 2022 - March 2023",
    //           text: "I was studying web development doing both front end and backend development"
    //         },
    //         {
    //           Occupation: "Student",
    //           institution: "University of The Western Cape",
    //           year: "February 2018 - 2020",
    //           text: "I unfortunately was not able to to complete my BA degree due to funding issues"
    //         },
    //         {
    //           Occupation: "Student",
    //           institution: "Goodwood College",
    //           year: "January 2017 - 2017",
    //           text: "I passed my matric with an admission to bachelors degree pass"
    //         },
    //       ]
    //     }
    // }
}
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap");

*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  --color: rgba(30, 30, 30);
  --bgColor: rgba(245, 245, 245);
  min-height: 100vh;
  display: grid;
  align-content: center;
  gap: 2rem;
  padding: 2rem;
  font-family: "Poppins", sans-serif;
  color: var(--color);
  background: var(--bgColor);
}

h1 {
  text-align: center;
}

ul {
  --col-gap: 2rem;
  --row-gap: 2rem;
  --line-w: 0.25rem;
  display: grid;
  grid-template-columns: var(--line-w) 1fr;
  grid-auto-columns: max-content;
  column-gap: var(--col-gap);
  list-style: none;
  width: min(60rem, 90%);
  margin-inline: auto;
}

/* line */
ul::before {
  content: "";
  grid-column: 1;
  grid-row: 1 / span 20;
  background: rgb(225, 225, 225);
  border-radius: calc(var(--line-w) / 2);
}

/* columns*/

/* row gaps */
ul li:not(:last-child) {
  margin-bottom: var(--row-gap);
}

/* card */
ul li {
  grid-column: 2;
  --inlineP: 1.5rem;
  margin-inline: var(--inlineP);
  grid-row: span 2;
  display: grid;
  grid-template-rows: min-content min-content min-content;
}

/* date */
ul li .date {
  --dateH: 3rem;
  height: var(--dateH);
  margin-inline: calc(var(--inlineP) * -1);

  text-align: center;
  background-color: var(--accent-color);

  color: white;
  font-size: 1.25rem;
  font-weight: 700;

  display: grid;
  place-content: center;
  position: relative;

  border-radius: calc(var(--dateH) / 2) 0 0 calc(var(--dateH) / 2);
}

/* date flap */
ul li .date::before {
  content: "";
  width: var(--inlineP);
  aspect-ratio: 1;
  background: var(--accent-color);
  background-image: linear-gradient(rgba(0, 0, 0, 0.2) 100%, transparent);
  position: absolute;
  top: 100%;

  clip-path: polygon(0 0, 100% 0, 0 100%);
  right: 0;
}

/* circle */
ul li .date::after {
  content: "";
  position: absolute;
  width: 2rem;
  aspect-ratio: 1;
  background: var(--bgColor);
  border: 0.3rem solid var(--accent-color);
  border-radius: 50%;
  top: 50%;

  transform: translate(50%, -50%);
  right: calc(100% + var(--col-gap) + var(--line-w) / 2);
}

/* title descr */
ul li .title,
ul li .descr {
  background: var(--bgColor);
  position: relative;
  padding-inline: 1.5rem;
}
ul li .title {
  overflow: hidden;
  padding-block-start: 1.5rem;
  padding-block-end: 1rem;
  font-weight: 500;
}
ul li .descr {
  padding-block-end: 1.5rem;
  font-weight: 300;
}

/* shadows */
ul li .title::before,
ul li .descr::before {
  content: "";
  position: absolute;
  width: 90%;
  height: 0.5rem;
  background: rgba(0, 0, 0, 0.5);
  left: 50%;
  border-radius: 50%;
  filter: blur(4px);
  transform: translate(-50%, 50%);
}
ul li .title::before {
  bottom: calc(100% + 0.125rem);
}

ul li .descr::before {
  z-index: -1;
  bottom: 0.25rem;
}

@media (min-width: 40rem) {
  ul {
    grid-template-columns: 1fr var(--line-w) 1fr;
  }
  ul::before {
    grid-column: 2;
  }
  ul li:nth-child(odd) {
    grid-column: 1;
  }
  ul li:nth-child(even) {
    grid-column: 3;
  }

  /* start second card */
  ul li:nth-child(2) {
    grid-row: 2/4;
  }

  ul li:nth-child(odd) .date::before {
    clip-path: polygon(0 0, 100% 0, 100% 100%);
    left: 0;
  }

  ul li:nth-child(odd) .date::after {
    transform: translate(-50%, -50%);
    left: calc(100% + var(--col-gap) + var(--line-w) / 2);
  }
  ul li:nth-child(odd) .date {
    border-radius: 0 calc(var(--dateH) / 2) calc(var(--dateH) / 2) 0;
  }
}

.credits {
  margin-top: 1rem;
  text-align: right;
}
.credits a {
  color: var(--color);
}

</style>