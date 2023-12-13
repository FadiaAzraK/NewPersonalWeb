<template>
    <div class="container">
        <div class="head" id="home">
            <div class="profile">
                <img src="@/assets/img/lusyu-removebg-preview.png" alt="Your Name" class="profile-image">
                <div class="profle-text">
                    <h1><span class="hello">Hello, </span> i'm Fadia Azra Kadarisman</h1>
                    <p class="typing-text">
                       Welcome To my personal website. Let's get to know me !
                    </p>
                    <!-- <div class="social-icons">
                        <a href="#" target="_blank">
                            <font-awesome-icon :icon="['fab', 'github']" />
                        </a>
                        <a href="#" target="_blank">
                            <i class="fab fa-linkedin"></i>
                        </a>
                        <a href="#" target="_blank">
                            <i class="fab fa-instagram"></i>
                        </a>
                    </div> -->
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

    .container {
        padding: 16px 0;
    }
    .head {
        position: relative;
        text-align: center;
        padding: 12px;
        margin-bottom: 6px;
        height: 500px;
        width: 100%;
        color: white;
    }
    .head:before {
        content: " ";
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 50%;
        background-color: black;
        transform: skew(0deg, 6deg);
        z-index: -1;
    }
    .head:after {
        content: " ";
        position: absolute;
        top: 0;
        right: 0;
        height: 100%;
        width: 50%;
        background-color: black;
        transform: skew(0deg, -6deg);
        z-index: -1;
    }
    .profile {
        position: relative;
        margin-top: 10%;
    }

    .profile-image {
        background-color: black;
        position: absolute;
        align-items: center;
        top: 75px;
        left: 50%;
        transform: translate(-50%, -50%);
        border-radius: 50px 50px 0 50px;
        width: 200px; 
        height: 250px;
        object-fit: cover;
    }

    .profile-text {
        color: white;
        margin-top: 20px;
    }

    h1, p {
        bottom: -130px;
        position: relative;
        color:white;
        margin: 0;
    }
    .hello {
        color: #FFD700; 
        font-size: 35px; 
        font-weight: bold; 
    }
    .typing-text {
        color: white;
        margin: 0;
        overflow: hidden;
        white-space: nowrap;
        animation: typing 2s steps(10) forwards;
        border-right: 2px solid white;
        display: inline-block;
    }
    @keyframes typing {
        from {
            width: 0;
        }
        to {
            width: 50%;
            border-color: transparent;
        }
    }

    @media (max-width: 768px) {
  .profile {
    margin-top: 100px;
  }

  .profile-image {
    width: 150px;
    height: 180px;
    top: 100%;
  }
  h1, p {
        bottom: -200px;
        position: relative;
        color:white;
        margin: 0;
    }

  h1 {
    font-size: 24px;
  }

  p {
    font-size: 16px;
  }
  .typing-text {
        color: white;
        margin-left: 20px;
        overflow: hidden;
        white-space: nowrap;
        animation: typing 2s steps(5) forwards;
        border-right: 2px solid white;
        display: inline-block;
        width: 50%;
    }
    @keyframes typing {
        from {
            width: 0;
        }
        to {
            width: 80%;
            border-color: transparent;
        }
    }
}

</style>