<template>
    <nav>
      <div class="logo" style="display: flex; align-items: center;">
        <span class="logo-name">アズラ</span>
      </div>
      <div class="hamburger" @click="toggleNav">
        <div class="line1"></div>
        <div class="line2"></div>
        <div class="line3"></div>
      </div>
      <ul class="nav-links" :class="{ open: isNavOpen }" @click="closeNav">
        <li><router-link to="/" @click="scrollToElement('home')">Home</router-link></li>
        <li><router-link to="/about" @click="scrollToElement('about')">About</router-link></li>
        <li><router-link to="/portfolio" @click="scrollToElement('portfolio')">Portfolio</router-link></li>
        <li><router-link to="/contact" @click="scrollToElement('contact')">Contact</router-link></li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    mounted() {
            this.hamburger = document.querySelector(".hamburger");
            this.navLinks = document.querySelector(".nav-links");
            this.links = document.querySelectorAll(".nav-links li");

            this.hamburger.addEventListener('click', () => {
                this.navLinks.classList.toggle("open");
                this.links.forEach(link => {
                    link.classList.toggle("fade");
                });

                this.hamburger.classList.toggle("toggle");
            });
        },
    data() {
      return {
        isNavOpen: true,
      };
    },
    methods: {
      toggleNav() {
        this.isNavOpen = !this.isNavOpen;
      },
      closeNav() {
        this.isNavOpen = false;
      },
      scrollToElement(elementId) {
        const element = document.getElementById(elementId);
        if (element) {
          element.scrollIntoView({
            behavior: 'smooth',
          });
        }
      },
    },
  };
  </script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Noto+Serif+JP:wght@200&family=Poppins:wght@600&display=swap');
    .logo-name {
      display: inline-block;
      white-space: nowrap;
      color: #000000;
      font-size: 26px;
      font-weight: bold;
      margin-left: 20px;
      font-family: 'Noto Serif JP', serif;
    }
    * {
        margin: 0;
        padding: 0;
        color: #000406;
        font-family: sans-serif;
        letter-spacing: 1px;
        font-weight: 300;
    }

    body {
        overflow-x: hidden;
    }

    nav {
        height: 4.5rem;
        width: 100vw;
        background-color: #fcfcfc;
        box-shadow: 0 3px 20px rgba(0, 0, 0, 0.2);
        display: flex;
        position: fixed;
        z-index: 10;
    }

    .logo {
        padding: 1vh 1vw;
        text-align: center;
    }

    .logo img {
        height: 5rem;
        width: 5rem;
    }

    .nav-links {
        display: flex;
        list-style: none;
        width: 88vw;
        padding: 0 0.7vw;
        justify-content: right;
        align-items: center;
        text-transform: uppercase;
        margin-right: 40px;
    }

    .nav-links li a {
        text-decoration: none;
        margin: 20px;
    }

    .nav-links li a:hover {
        color: #000000;
        border-bottom: 2px solid #484747;
        
    }

    .nav-links li {
        position: relative;
    }

    .nav-links li a:hover::before {
        width: 80%;
    }

    .hamburger div {
        width: 30px;
        height: 3px;
        background: #000000;
        margin: 5px;
        transition: all 0.3s ease;
    }

    .hamburger {
        display: none;
    }

    @media screen and (max-width: 800px) {
        nav {
            position: fixed;
            z-index: 3;
        }

        .hamburger {
            display: block;
            position: absolute;
            cursor: pointer;
            right: 5%;
            top: 50%;
            transform: translate(-5%, -50%);
            z-index: 2;
            transition: all 0.7s ease;
        }

        .nav-links {
            position: fixed;
            background: #ffffff;
            height: 100vh;
            width: 100%;
            flex-direction: column;
            clip-path: circle(50px at 90% -20%);
            -webkit-clip-path: circle(50px at 90% -10%);
            transition: all 1s ease-out;
            pointer-events: none;
        }

        .nav-links.open {
            clip-path: circle(1000px at 90% -10%);
            -webkit-clip-path: circle(1000px at 90% -10%);
            pointer-events: all;
        }

        .nav-links li {
            opacity: 0;
        }

        .nav-links li:nth-child(1) {
            transition: all 0.5s ease 0.2s;
        }

        .nav-links li:nth-child(2) {
            transition: all 0.5s ease 0.4s;
        }

        .nav-links li:nth-child(3) {
            transition: all 0.5s ease 0.6s;
        }

        .nav-links li:nth-child(4) {
            transition: all 0.5s ease 0.7s;
        }

        .nav-links li:nth-child(5) {
            transition: all 0.5s ease 0.8s;
        }

        .nav-links li:nth-child(6) {
            transition: all 0.5s ease 0.9s;
            margin: 0;
        }

        .nav-links li:nth-child(7) {
            transition: all 0.5s ease 1s;
            margin: 0;
        }

        li.fade {
            opacity: 1;
        }
    }

    .toggle .line1 {
        transform: rotate(-45deg) translate(-5px, 6px);
    }

    .toggle .line2 {
        transition: all 0.7s ease;
        width: 0;
    }

    .toggle .line3 {
        transform: rotate(45deg) translate(-5px, -6px);
    }
</style>
