<template>
    <div class="container">
      <h1 class="title" id="contact">Contact Me</h1>
      <div class="social-icons">
        <div class="ig">
          <a href="instagram.com/fdiaazr_" target="_blank" rel="noopener noreferrer">
            <i class="fab fa-instagram" style="color: #000000;"></i>
            <span>@fdiaazr_</span>
          </a>
        </div>
        <div class="github">
          <a href="https://github.com/FadiaAzraK" target="_blank" rel="noopener noreferrer">
            <i class="fab fa-github" style="color: #000000;"></i>
            <span>FadiaAzraK</span>
          </a>
        </div>
        <div class="linkedin">
          <a href="www.linkedin.com/in/fadia-azra-kadarisman-7099052a4" target="_blank" rel="noopener noreferrer">
            <i class="fab fa-linkedin" style="color: #000000;"></i>
            <span>Fadia Azra Kadarisman</span>
          </a>
        </div>
        <div class="email">
          <a href="mailto:fadiaazra50@gmail.com" target="_blank" rel="noopener noreferrer">
            <i class="fas fa-envelope" style="color: #000000;"></i>
            <span>fadiaazra50@gmail.com</span>
          </a>
        </div>
      </div>
    </div>

  </template>
  
  <style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
  
  * {
    font-family: 'Poppins', sans-serif;
  }
  
  .container {
    margin: 0 auto;
    padding: 20px;
    text-align: center;
    margin-top: 30px;
  }
  
  .title {
    font-size: 2em;
    margin-bottom: 20px;
  }
  
  .social-icons {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
  }
  
  .icon {
    flex: 1 1 calc(50% - 20px);
    margin: 10px;
    text-align: center;
  }
  
  .social-icons a {
    color: #555;
    font-size: 2em;
    text-decoration: none;
    display: flex;
    flex-direction: column;
    align-items: center;
    transition: color 0.3s ease;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 10px;
  }
  
  .social-icons a:hover {
    color: #007bff;
    cursor: pointer;
  }
  
  @media screen and (max-width: 767px) {
    .icon {
      flex: 1 1 calc(100% - 20px);
    }
  }
</style>