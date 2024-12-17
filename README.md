@import url('https://fonts.googleapis.com/css2?family=ADLaM+Display&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Inknut+Antiqua:wght@300;400;500;600;700;800;900&display=swap');

::-webkit-scrollbar {
  width: 10px;
}

::-webkit-scrollbar-track {
  background-color: #0e1b2b;
}

::-webkit-scrollbar-thumb {
  background-color: #233f80;
  border-radius: 1px;
}
::-webkit-scrollbar-thumb:active {
  background-color: #192f60;
}
::selection {
  background-color: #f7efdd;
  color: white;
}

:root {
  font-family: 'ADLaM Display', system-ui;
  font-weight: 400;
  font-style: normal;
  letter-spacing: 1px;

  /* Darker variants for hover */
  --swiper-navigation-size: 30px !important;
  --swiper-theme-color: #edc048 !important;
}

html {
  scroll-behavior: smooth;
  font-size: 18px;
}

@media (max-width: 1200px) {
  html {
    font-size: 16px;
  }
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  line-height: 1.7;
}

body {
  background: #f7efdd;
  color: var(--text);
  margin: 0;
  padding: 0;
}

img,
button {
  user-select: none;
}

/* Header */
.parent {
  padding: 0 20px;
  margin: 0 auto;
}

@media (min-width: 768px) {
  .parent {
    width: 750px;
  }
}

@media (min-width: 992px) {
  .parent {
    width: 970px;
  }
}

@media (min-width: 1200px) {
  .parent {
    width: 1170px;
  }
}

@media (min-width: 1400px) {
  .parent {
    width: 1370px;
  }
}

/* inputs */
input,
textarea,
select {
  padding: 13px 15px;
  /* border: 2px solid rgb(214, 214, 214); */
  border: 1px solid #ced4da;
  border-radius: 5px;
  transition: var(--transition) border-color;
  margin: 2px;
  font-size: 1rem;
  font-family: inherit;
}

textarea {
  resize: none;
}

input:focus,
textarea:focus,
select:focus {
  outline: none;
  border: 3px solid #233f80;
  margin: 0;
}

.sub-title {
  color: #edc048;
  font-size: 21px;
}

.center {
  text-align: center;
}

.btn {
  outline: none;
  border: 0;
  font-size: 1rem;
  font-family: inherit;
  padding: 7px 20px;
  border-radius: 5px;
  transition: 0.5s background;
  cursor: pointer;
  border-radius: 50px;
}

.btn-primary {
  background: #233f80;
  color: white;
  font-weight: 500;
}

.btn-primary:hover {
  background: #192f60;
}

.btn-navy {
  background: #233f80;
  color: white;
  font-weight: bold;
}

.btn-navy:hover {
  background: #192f60;
}

.btn-nav {
  background: #233f80;
  color: white;
  width: 100%;
}

.btn-landing {
  font-family: inherit;
  font-weight: 400;
  font-size: 24px;
  margin-top: 20px;
  padding: 5px 20px;
}

p {
  font-family: 'Inter';
  font-weight: 600;
}

span.s {
  color: var(--peach);
  font-size: 21px;
  font-weight: bolder;
}

span.b {
  font-weight: 900;
}

h1 {
  font-size: 2.5rem;
  font-weight: 400;
}

h2 {
  font-size: 32px;
  font-weight: 400;
}

h3 {
  font-size: 24px;
  font-weight: 900;
  color: #ffefcb;
  font-family: 'Inter';
  margin: 20px 0;
}

.margin-box {
  margin: 25px 0;
}

a {
  color: white;
}

/* Header */
nav {
  position: fixed;
  background: #4dff0000;
  top: 0;
  z-index: 100;
  left: 50%;
  transform: translate(-50%);
  width: 100%;
  padding: 20px;
}

nav .logo {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 5px 5px 5px 0;
}

nav img {
  width: 50px;
  animation: logo 0.75s ease-in-out;
}

@keyframes logo {
  0% {
    transform: rotate(0deg);
  }

  25% {
    transform: rotate(45deg);
  }

  50% {
    transform: rotate(-45deg);
  }

  100% {
    transform: rotate(0deg);
  }
}

nav .parent {
  display: grid;
  grid-template-columns: auto 1fr auto;
  text-align: center;
  align-items: center;
  width: fit-content;
  min-width: 620px;
  border-radius: 50px;
  background: #7ae500;
}

nav .links {
  margin-right: 10px;
  color: #ffffff;
}

nav a {
  color: var(--text);
  text-decoration: none;
  padding: 10px 10px;
  position: relative;
  transition: 0.2s;
}

nav a:hover {
  background: #ffffffde;
  border-radius: 50px;
  color: black;
}

.parent .logo .linkimg {
  padding: 0;
  transition: 4s;
}

.parent .logo .linkimg:hover {
  background: transparent;
  border-radius: 0;
  scale: 1.05;
  rotate: 1440deg;
}

nav .btn {
  padding: 10px 20px;
  border-radius: 50px;
}

/* long-term-relationship */

.long-term-relationship .content {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  padding: 10px 0px 0px 30px;
}

.long-term-relationship .text-section h6 {
  font-size: 16px;
  letter-spacing: 2px;
  color: #333;
  position: relative;
  margin-bottom: 20px;
  padding-top: 75px;
}

.long-term-relationship .text-section h6::before {
  content: '';
  position: absolute;
  top: 50%;
  left: -40px;
  width: 30px;
  height: 2px;
  background-color: #ffdd00;
  transform: translateY(-50%);
}

.long-term-relationship .text-section h1 {
  font-size: 48px;
  line-height: 1.2;
  font-weight: bold;
  color: #333;
}

.long-term-relationship .image-section img {
  max-width: 450px;
  height: auto;
  padding-left: 50px;
}

/* Adjust layout for smaller screens */
@media (max-width: 768px) {
  .long-term-relationship .content {
    flex-direction: column;
    text-align: center;
  }

  .long-term-relationship .image-section img {
    margin-top: 20px;
  }
}

/* Footer of about */

.long-term-relationship .footer-of-about {
  background-color: #000016;
  color: #fff;
  display: flex;
  justify-content: space-between;
  padding: 1% 10% 1% 10%;
}

.long-term-relationship .footer-of-about-title {
  font-size: 1.3em;
  font-weight: 600;
  padding-top: 1px;
}

/* Sections */
section {
  padding-top: 100px;
}

section .sec .parent {
  display: block;
}

section .sec .title {
  margin-top: 20px;
  padding-bottom: 14px;
}

section .sec p {
  padding-bottom: 40px;
}

section .lr {
  display: flex;
  align-items: center;
}

section .lr .right {
  flex: 1;
}

section {
  min-height: 100vh;
}

section .parent {
  padding: 20px;
}

section .parent.grid {
  display: grid;
  grid-template-columns: 4fr 3fr;
  align-items: center;
  min-height: 100vh;
}

@media (max-width: 1200px) {
  section .parent.grid {
    grid-template-columns: auto;
    grid-template-rows: 1fr 1fr;
    margin-top: 50px;
  }

  section .parent.grid .right {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}

/* Feedback */
.swiper {
  padding: 20px 0;
}

.swiper-slide {
  width: 370px !important;
  padding: 0 -20px;
}

.swiper-button-next,
.swiper-button-prev {
  font-weight: bold;
}

.swiper-button-next:hover,
.swiper-button-prev:hover {
  color: #b88e45;
}

.card-container {
  display: flex;
  justify-content: center;
  gap: 2rem;
}

.card {
  width: 300px;
  height: 400px;
  padding: 1rem;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
  text-align: center;
  transition: 0.2s;
}

.card:hover {
  scale: 1.01;
}

.card img {
  width: auto;
  height: 150px;
  margin-top: 2rem;
  margin-bottom: 1rem;
}
.Evidence-based-Learning h2,
.Conservation h2,
.Conservation-Filmmaking-Program h2 {
  text-align: center;
  margin-bottom: 20px;
}
.card h3 {
  font-size: 1.2rem;
  color: #333;
}

.reviews {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 2rem;
}

.review {
  width: 200px;
  text-align: center;
  font-size: 0.9rem;
  color: #777;
}

/* footer */

.footer {
  background-color: #000016;
  color: #fff;
  padding: 1em;
  display: flex;
  justify-content: space-between;
}

.footer-title {
  font-size: 1.3em;
  font-weight: 600;
  padding-top: 1px;
}

.footer-title span a {
  text-decoration: none;
  color: #3a6cf4;
  font-size: 1.2em;
}

.footer-title span a:hover {
  color: red;
}

.footer-title .social-icons a {
  font-size: 1.3em;
  padding: 0 12px 0 0;
}
