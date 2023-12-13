<template>
    <div class="container" id="portfolio">
      <h1 class="title" >Portofolio</h1>
      <div class="cards">
        <div class="card">
          <img src="@/assets/img/port-1.png" alt="Card Image" />
          <div class="card-content">
            <h3>My First Project</h3>
            <p>My first personal web using html & css</p>
          </div>
        </div>
        <div class="card">
          <img src="@/assets/img/port-2.png" alt="Card Image" />
          <div class="card-content">
            <h3>Web School</h3>
            <p>Website that explains about the school</p>
          </div>
        </div>
        <div class="card">
          <img src="@/assets/img/port-3.png" alt="Card Image" />
          <div class="card-content">
            <h3>MVC Peminjaman</h3>
            <p>This website is used for management regarding borrowing things</p>
          </div>
        </div>
        <div class="card">
          <img src="@/assets/img/port-4.png" alt="Card Image" />
          <div class="card-content">
            <h3>OOP Rental Motor</h3>
            <p>Used to calculate motorbike rental prices</p>
          </div>
        </div>
        <div class="card">
          <img src="@/assets/img/port-5.png" alt="Card Image" />
          <div class="card-content">
            <h3>OOP Pembelian Bensin</h3>
            <p>Used to calculate the purchase price of gasoline</p>
          </div>
        </div>
        <div class="card">
          <img src="@/assets/img/port-6.png" alt="Card Image" />
          <div class="card-content">
            <h3>Vue Js Bisnis</h3>
            <p>used for business management</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .container {
    margin: 0 auto;
    padding: 20px;
  }

  .title {
    font-size: 2em;
    text-align: center;
    margin-bottom: 20px;
  }

  .cards {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    justify-content: center;
  }

  .card {
    flex: 0 0 calc(33.33% - 16px);
    max-width: calc(33.33% - 16px);
    border: 1px solid #ddd;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }

  .card img {
    width: 100%;
    height: 150px;
    object-fit: cover;
  }

  .card-content {
    padding: 16px;
  }

  .card-content h3 {
    font-size: 1.2em;
    margin-bottom: 8px;
  }

  .card-content p {
    color: #555;
  }

  @media screen and (max-width: 767px) {
    .card {
      flex: 0 0 calc(100% - 16px);
      max-width: calc(100% - 16px);
    }
  }
</style>
