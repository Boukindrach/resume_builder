<template>
  <main class="container">
      <div id="resume" class="d-flex">
        <div class="left-col">
          <h4 class="section-headline">
            About me
          </h4>
          <div>
            I am a 10x software engieer
          </div>
          <h4 class="section-headline">
            Contact
          </h4>
          <ul>
            <li>+2126959465</li>
            <li>contact@gmail.com</li>
            <li>Morocco-agadir</li>
          </ul>
          <h4 class="section-headline">
            Skills
          </h4>
          <ul>
            <li>Python</li>
            <li>Pandas</li>
            <li>SQL</li>
            <li>R</li>
            <li>Machine Learning</li>
          </ul>
          <h4 class="section-headline">
            Certifications
          </h4>
          <ul>
            <li>Natural Language Processing with Python (Coursera)</li>
            <li>Recommendation Systems with TensorFlow on GCP (Google)</li>
          </ul>
        </div>
        <div class="right-col">
          <div class="personal-name">
            Jhon stones
          </div>
          <div class="personal-title">
            Software developer
          </div>
          <h4 class="section-headline">
            Experience
          </h4>
          <div>Senior software engieer</div>
          <div>Blackrocket Inc., London, 2023 - Present</div>
          <h4 class="section-headline">
            Education
          </h4>
          <div>Bachelor of Science in Computer Science</div>
          <div>Evergreen State University, Springdale, 2018-2022</div>
          <ul>
            <li>Relevant coursework in database management, algorithms, and programming languages.</li>
            <li>Senior project: 'Development of a Recommender System for Movie Ratings.'</li>
          </ul>
        </div>
      </div>
  </main>
</template>

<style scoped>
  #resume {
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    height: 297mm;
    width: 210mm;
  }
  .left-col {
    background-color: var(--background-color-left);
    color: var(--text-color-left);
    border-right: 1px solid var(--highlight-color-left);
    width: 30%;
    padding: 30px;
  }

  .right-col {
    background-color: var(--background-color-right);
    color: var(--text-color-right);
    width: 70%;
    padding: 30px;
  }

  .section-headline {
    font-size: 20px;
    font-weight: var(--headline-weight);
    margin-bottom: 15px;
    margin-top: 0;
  }

  .right-col .section-headline {
    color: var(--highlight-color-right);
  }

  .left-col .section-headline {
    border-bottom: 1px solid var(--highlight-color-left);
    padding-bottom: 5px;
    margin-right: -30px;
    padding-right: 10px;
    color: var(--highlight-color-left);
  }

  .resume-section {
    margin-bottom: 30px;
  }

  .personal-name {
    font-weight: 300;
    color: var(--highlight-color-right);
    font-size: 28px;
    border-bottom: 1px solid var(--highlight-color-right);
    margin: 0;
    margin-left: -30px;
    padding-left: 30px;
    padding-bottom: 15px;
  }

  .personal-title {
    border-bottom: 1px solid var(--highlight-color-right);
    margin: 0 0 20px -30px;
    padding: 15px 0 15px 30px;
    font-weight: 300;
    font-size: 20px;
  }

  #resume ul {
    padding-inline-start: 16px;
    margin-block-end: 0px;
    margin-block-start: 5px;
  }
</style>
