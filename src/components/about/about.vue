<template>
  <section class="card" id="about">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
      <div class="text-content">
        <h3>About Me</h3>
        <p>
          Hello, my name is Fadia Azra Kadarisman. I am a hard worker, disciplined and consistent. I am a person who can work in a team, and have experience as a team leader. I have an interest in a career as a back end developer.
        </p>
        <div class="skills">
        <strong><H3>Skills</H3></strong>
        <div class="skill-icons">
          <i class="fa-brands fa-html5" style="color: #ffffff;"></i>
          <i class="fa-brands fa-css3-alt" style="color: #ffffff;"></i>
          <i class="fa-brands fa-php" style="color: #ffffff;"></i>
          <i class="fa-brands fa-laravel" style="color: #ffffff;"></i>
          <i class="fa-brands fa-js" style="color: #ffffff;"></i>
          <i class="fa-solid fa-database" style="color: #ffffff;"></i>
         </div>
        </div>
        <br>
      </div>
      <div class="visual">
          <img src="@/assets/img/yy.jpg" alt="" />
      </div>
    </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Poppins:400,300,500');

section.card {
  font-family: 'Poppins', sans-serif;
  background: #000000;
  border-radius: 0;
  padding: 24px;
  margin: 48px 0;
  display: flex;
  flex-direction: column;
  position: relative;
  box-shadow: 5px 0 0 0 rgba(204, 204, 204, 0.3),
              -5px 0 0 0 rgba(204, 204, 204, 0.3),
              0 5px 0 0 rgba(204, 204, 204, 0.3);
  height: 85vh;
}

section.card .text-content {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin-top: 40px;
}

section.card .text-content h3 {
  margin: 0;
  font-size: 1.5em;
  max-width: 20ch;
  color: #fff;
}

section.card .text-content p {
  margin: 20px 0;
  color: #fff;
}

section.card .text-content a {
  border: 3px solid #f2f2f2;
  color: #ffffff;
  align-self: flex-start;
  text-decoration: none;
  padding: 16px 32px;
  border-radius: 12px;
  transition: 400ms all;
  margin-top: 20px;
}

section.card .text-content a:hover {
  background: #000000;
  color: white;
}

section.card .visual {
  width: 100%;
  height: auto;
  overflow: hidden;
  border-radius: 12px;
  margin-top: 20px;
}

section.card .visual img {
  width: 50%;
  height: auto;
  border-radius: 12px;
  margin-left: 200px;
  margin-top: 20px;
  margin-right: auto;
}

.skills {
  margin-top: 20px;
}

.skills h3 {
  color: #fff;
  font-size: 1.5em;
  margin-bottom: 10px;
}

.skills .skill-icons {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.skills .skill-icons i {
  font-size: 36px;
  margin-right: 20px;
  color: #ffffff;
  transition: color 0.3s ease;
}

.skills .skill-icons i:hover {
  color: #FFD700;
}

@media screen and (min-width: 768px) {
  section.card {
    flex-direction: row;
  }

  section.card .text-content {
    width: calc(60% - 20px);
    margin-left: 20px;
  }

  section.card .visual {
    margin-top: 0;
  }

  .skills .skill-icons {
    margin-top: 0;
  }
}

@media screen and (max-width: 767px) {
  section.card {
    padding: 20px;
    margin: 24px 0;
  }

  section.card .text-content a {
    align-self: flex-start;
    margin-top: 20px;
  }

  section.card .text-content {
    margin-top: 0;
  }

  section.card .visual img {
    margin-left: 0;
  }
}
</style>