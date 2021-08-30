<template>
  <div>
    <div class="header">
       <nav role="navigation nav_drawer ">
      <div id="menuToggle" class="nav_drawer">
        <input type="checkbox" class="checkbox nav_drawer"/>
        <span></span>
        <span></span>
        <span></span>

        <!--
    Too bad the menu has to be inside of the button
    but hey, it's pure CSS magic.
    -->
        <ul id="menu" class="nav_drawer_list">
          <a href="#"><li>SIGN IN</li></a>
          <a href="#"><li>JOIN</li></a>
        </ul>
      </div>
    </nav>
      <div class="left_property ">
        <nav class="navbar">
          <div class="menu-toggle" id="mobile-menu">
            <span class="bar"></span>
            <span class="bar"></span>
            <span class="bar"></span>
          </div>
          <ul class="nav">
            <li class="nav-item"><a href="#"><span class="material-icons donut">
donut_small
</span> </a></li>
            <li class="nav-item"><a href="#">SIGN IN</a></li>
            |<li class="nav-item"><a href="#">JOIN</a></li>
          </ul>
        </nav>
      </div>
      <div class="image"></div>
      <div class="right_property">
        <nav class="navbar right_navbar">
           <ul class="nav">
            <li class="nav-item"><a href="#"><p class="right_logo hide"><span  class="material-icons token">
token
</span></p> </a></li>
            <li class="nav-item marvel_unlimited"><a href="#"><p class="right_logo hide">MARVEL UNLIMITED</p><h5 class="subscribe hide">SUBSCRIBE</h5></a></li>
            
            <li class="nav-item"><a href="#"><span class="material-icons">
search
</span></a></li>
          </ul>

        </nav>
        
      </div>
    </div>
    <div class="subheader">
      <div class="Captain_comics">Captain Marvels Comics</div>
    </div>
    <div class="last_header">
      <h6 class="last_header_details">STREAM WHAT IF? EXCLUSIVE ON</h6>
    </div>
  </div>
</template>

<style>
body {
  margin: 0;
  padding: 0;
  height: 100%;
}
.header {
  padding: 1px;
  width: 100%;
  height: 55px;
  background-color: #232323;
  display: flex;
}
.nav_drawer{
  display: none;
}
.left_property {
  color: white;
  font-family: "Avenir Next", "Avenir", sans-serif;
  width: 210px;
  height: 55px;
  background-color: #232323;
  border-right: 1px solid rgb(63, 60, 60);
  border-left: 1px solid rgb(63, 60, 60);
  position: absolute;
  left: 3cm;
}
.donut{
  position: relative;
  bottom: 8px;
}
.token{
  position: relative;
  bottom: 5px;
  color: red;

}
.right_property {
  color: white;
  font-family: "Avenir Next", "Avenir", sans-serif;
  width: 270px;
  height: 55px;
  background-color: #232323;
  border-right: 1px solid rgb(63, 60, 60);
  border-left: 1px solid rgb(63, 60, 60);
  position: absolute;
  right: 3cm;
 
}

.navbar ul {
  list-style: none;
  display: flex;
  color: white;
  padding: 5px 10px;
  line-height: 10px;
}

.nav-item a {
  color: white;
  font-size: 09rem;
  font-weight: 400;
  text-decoration: none;
  transition: color 03s ease-out;
  padding: 5px 10px;
  line-height: 10px;
  font-weight: 600;
  font-size: small;
}
.right_logo{
  position: relative;
  bottom: 22px;
}
.subscribe{
  position: relative;
  bottom: 33px;
}

.marvel_unlimited{
  margin: auto;
  text-align: center;
  border-right: 0px solid rgb(63, 60, 60);
  
}






.marvel {
  color: white;
  text-align: center;
}
.image {
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  margin: auto;
  background-image: url("marvel.png");
  width: 150px;
  height: 55px;
}
.subheader {
  background-color: #232323;
  border-top: 1px solid rgb(63, 60, 60);
  width: 100%;
  height: 45px;
}
.Captain_comics {
  color: white;
  text-align: center;
  margin-top: 13px;
  font-style: initial;
  font-size: medium;
  font-weight: 700;
  font-family: "Avenir Next", "Avenir", sans-serif;
}
.last_header {
  background-color: rgb(0, 0, 2);
  opacity: 0.9;
  border-top: 1px solid rgb(63, 60, 60);
  width: 100%;
  height: 30px;
}
.last_header_details {
  color: white;
  text-align: center;
  margin-top: 7px;
  font-style: initial;
  font-weight: lighter;
  font-family: "Avenir Next", "Avenir", sans-serif;
}

/* Portrait for s5 s4 ans note 3 */
@media screen and (device-width: 320px) and (device-height: 640px) and (-webkit-device-pixel-ratio: 3) and (orientation: portrait) {
  .nav-item a {
    display: none;
  }
  .right_property{
     display: none;
  }
}
/* ----------- Galaxy S6 ----------- */

/* Portrait and Landscape */
@media screen and (device-width: 360px) and (device-height: 640px) and (-webkit-device-pixel-ratio: 4) {
  .nav-item a {
    display: none;
  }
  .left_property {
    display: none;
  }
  .right_property{
     display: none;
  }
}


/* ----------- iPhone 5, 5S, 5C and 5SE ----------- */

/* Portrait and Landscape */
@media only screen 
  and (min-device-width: 320px) 
  and (max-device-width: 568px)
  and (-webkit-min-device-pixel-ratio: 2) {
    .nav-item a {
    display: none;
  }
  .left_property {
    display: none;
  }
  .right_property{
     display: none;
  }

   body {
    margin: 0;
    padding: 0;

    /* make it look decent enough */
    background: #232323;
    color: #cdcdcd;
    font-family: "Avenir Next", "Avenir", sans-serif;
  }

  #menuToggle {
    display: block;
    position: relative;
    top: 20px;
    left: 30px;

    z-index: 1;

    -webkit-user-select: none;
    user-select: none;
  }

  #menuToggle a {
    text-decoration: none;
    color: #232323;

    transition: color 0.3s ease;
  }


  #menuToggle input {
    display: block;
    width: 40px;
    height: 32px;
    position: absolute;
    top: -7px;
    left: -5px;

    cursor: pointer;

    opacity: 0; /* hide this */
    z-index: 2; /* and place it over the hamburger */

    -webkit-touch-callout: none;
  }

  /*
 * Just a quick hamburger
 */
  #menuToggle span {
    display: block;
    width: 33px;
    height: 4px;
    margin-bottom: 5px;
    position: relative;

    background: #cdcdcd;
    border-radius: 3px;

    z-index: 1;

    transform-origin: 4px 0px;

    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1),
      background 0.5s cubic-bezier(0.77, 0.2, 0.05, 1), opacity 0.55s ease;
  }

  #menuToggle span:first-child {
    transform-origin: 0% 0%;
  }

  #menuToggle span:nth-last-child(2) {
    transform-origin: 0% 100%;
  }

  /* 
 * Transform all the slices of hamburger
 * into a crossmark.
 */
  #menuToggle input:checked ~ span {
    opacity: 1;
    transform: rotate(45deg) translate(-2px, -1px);
    background: #cdcdcd;
  }

  /*
 * But let's hide the middle one.
 */
  #menuToggle input:checked ~ span:nth-last-child(3) {
    opacity: 0;
    transform: rotate(0deg) scale(0.2, 0.2);
  }

  /*
 * Ohyeah and the last one should go the other direction
 */
  #menuToggle input:checked ~ span:nth-last-child(2) {
    transform: rotate(-45deg) translate(0, -1px);
     color: white;
  }

  /*
 * Make this absolute positioned
 * at the top left of the screen
 */
  #menu {
    position: absolute;
    width: 100vw;
    margin: -100px 0px 0 -50px;
    padding: 100px;
    padding-top: 125px;

    background: #232323;
    list-style-type: none;
    -webkit-font-smoothing: antialiased;
    /* to stop flickering of text in safari */

    transform-origin: 0% 0%;
    transform: translate(-100%, 0);

    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1);
  }

  #menu li {
    padding: 10px;
    font-size: 25px;
    font-weight: bolder;
    color: white;
    position: relative;
    right: 2px;

  }

  /*
 * And let's slide it in from the left
 */
  #menuToggle input:checked ~ ul {
    transform: none;
  }

  .last_header {
  background-color: rgb(32, 30, 30);
  opacity: 0.9;
  border-top: 1px solid rgb(63, 60, 60);
  width: 100%;
  height: 30px;
}
.last_header_details {
  color: white;
  text-align: center;
  margin-top: 7px;
  font-style: initial;
  font-weight: lighter;
  font-family: "Avenir Next", "Avenir", sans-serif;
}
}





/* ----------- iPhone 6, 6S, 7 and 8 ----------- */

/* Portrait and Landscape */
@media only screen and (min-device-width: 375px) and (max-device-width: 667px) and (-webkit-min-device-pixel-ratio: 2) {
  .nav-item a {
    display: none;
  }
  .left_property {
    display: none;
  }
  .hide{
  display: none;
}


   body {
    margin: 0;
    padding: 0;

    /* make it look decent enough */
    background: #232323;
    color: #cdcdcd;
    font-family: "Avenir Next", "Avenir", sans-serif;
  }

  #menuToggle {
    display: block;
    position: relative;
    top: 20px;
    left: 30px;

    z-index: 1;

    -webkit-user-select: none;
    user-select: none;
  }

  #menuToggle a {
    text-decoration: none;
    color: #232323;

    transition: color 0.3s ease;
  }


  #menuToggle input {
    display: block;
    width: 40px;
    height: 32px;
    position: absolute;
    top: -7px;
    left: -5px;

    cursor: pointer;

    opacity: 0; /* hide this */
    z-index: 2; /* and place it over the hamburger */

    -webkit-touch-callout: none;
  }

  /*
 * Just a quick hamburger
 */
  #menuToggle span {
    display: block;
    width: 33px;
    height: 4px;
    margin-bottom: 5px;
    position: relative;

    background: #cdcdcd;
    border-radius: 3px;

    z-index: 1;

    transform-origin: 4px 0px;

    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1),
      background 0.5s cubic-bezier(0.77, 0.2, 0.05, 1), opacity 0.55s ease;
  }

  #menuToggle span:first-child {
    transform-origin: 0% 0%;
  }

  #menuToggle span:nth-last-child(2) {
    transform-origin: 0% 100%;
  }

  /* 
 * Transform all the slices of hamburger
 * into a crossmark.
 */
  #menuToggle input:checked ~ span {
    opacity: 1;
    transform: rotate(45deg) translate(-2px, -1px);
    background: #cdcdcd;
  }

  /*
 * But let's hide the middle one.
 */
  #menuToggle input:checked ~ span:nth-last-child(3) {
    opacity: 0;
    transform: rotate(0deg) scale(0.2, 0.2);
  }

  /*
 * Ohyeah and the last one should go the other direction
 */
  #menuToggle input:checked ~ span:nth-last-child(2) {
    transform: rotate(-45deg) translate(0, -1px);
     color: white;
  }

  /*
 * Make this absolute positioned
 * at the top left of the screen
 */
  #menu {
    position: absolute;
    width: 100vw;
    margin: -100px 0px 0 -50px;
    padding: 100px;
    padding-top: 125px;

    background: #232323;
    list-style-type: none;
    -webkit-font-smoothing: antialiased;
    /* to stop flickering of text in safari */

    transform-origin: 0% 0%;
    transform: translate(-100%, 0);

    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1);
  }

  #menu li {
    padding: 10px;
    font-size: 25px;
    font-weight: bolder;
    color: white;
    position: relative;
    right: 2px;

  }

  /*
 * And let's slide it in from the left
 */
  #menuToggle input:checked ~ ul {
    transform: none;
  }

  .last_header {
  background-color: rgb(32, 30, 30);
  opacity: 0.9;
  border-top: 1px solid rgb(63, 60, 60);
  width: 100%;
  height: 30px;
}
.last_header_details {
  color: white;
  text-align: center;
  margin-top: 7px;
  font-style: initial;
  font-weight: lighter;
  font-family: "Avenir Next", "Avenir", sans-serif;
}
}

/* ----------- iPhone 6+, 7+ and 8+ ----------- */

/* Portrait and Landscape */
@media only screen and (min-device-width: 414px) and (max-device-width: 736px) and (-webkit-min-device-pixel-ratio: 3) {
  .nav-item a {
    display: none;
  }
  .left_property {
    display: none;
  }
 

}
/* ----------- iPhone X ----------- */

/* Portrait and Landscape */
@media only screen and (min-device-width: 375px) and (max-device-width: 812px) and (-webkit-min-device-pixel-ratio: 3) {
  .nav-item a {
    display: none;
  }
  .Captain_comics {
  color: white;
  text-align: center;
  margin-top: 13px;
  font-style: initial;
  font-size: medium;
  font-weight: 700;
  font-family: "Avenir Next", "Avenir", sans-serif;
}
.last_header {
  background-color: rgb(32, 30, 30);
  opacity: 0.9;
  border-top: 1px solid rgb(63, 60, 60);
  width: 100%;
  height: 30px;
}
.last_header_details {
  color: white;
  text-align: center;
  margin-top: 7px;
  font-style: initial;
  font-weight: lighter;
  font-family: "Avenir Next", "Avenir", sans-serif;
}
 .left_property {
   display: none;
  }
  .right_property {
  color: white;
  font-family: "Avenir Next", "Avenir", sans-serif;
  width: 270px;
  height: 55px;
  background-color: #232323;
  border-right: 1px solid rgb(63, 60, 60);
  border-left: 1px solid rgb(63, 60, 60);
  position: absolute;
  right: 0.5cm;
 
}
.hide{
  display: none;
}

.navbar ul {
  list-style: none;
  display: flex;
  color: white;
  padding: 5px 10px;
  line-height: 10px;
}

.nav-item a {
  color: white;
  font-size: 09rem;
  font-weight: 400;
  text-decoration: none;
  transition: color 03s ease-out;
  padding: 5px 10px;
  line-height: 10px;
  font-weight: 600;
  font-size: small;
}
.right_logo{
  position: relative;
  bottom: 22px;
}
.subscribe{
  position: relative;
  bottom: 33px;
}

.marvel_unlimited{
  margin: auto;
  text-align: center;
  border-right: 0px solid rgb(63, 60, 60);
  
}
 

  .navbar ul {
    list-style: none;
    display: flex;
    color: white;
    padding: 5px 10px;
    line-height: 10px;
  }

  .nav-item a {
    color: white;
    font-size: 09rem;
    font-weight: 400;
    text-decoration: none;
    transition: color 03s ease-out;
    padding: 5px 10px;
    line-height: 10px;
    font-weight: 600;
    font-size: small;

  }

.nav_drawer_list a{
  font-size: x-small;
}
  body {
    margin: 0;
    padding: 0;

    /* make it look decent enough */
    background: #232323;
    color: #cdcdcd;
    font-family: "Avenir Next", "Avenir", sans-serif;
  }

  #menuToggle {
    display: block;
    position: relative;
    top: 20px;
    left: 30px;

    z-index: 1;

    -webkit-user-select: none;
    user-select: none;
  }

  #menuToggle a {
    text-decoration: none;
    color: #232323;

    transition: color 0.3s ease;
  }


  #menuToggle input {
    display: block;
    width: 40px;
    height: 32px;
    position: absolute;
    top: -7px;
    left: -5px;

    cursor: pointer;

    opacity: 0; /* hide this */
    z-index: 2; /* and place it over the hamburger */

    -webkit-touch-callout: none;
  }

  /*
 * Just a quick hamburger
 */
  #menuToggle span {
    display: block;
    width: 33px;
    height: 4px;
    margin-bottom: 5px;
    position: relative;

    background: #cdcdcd;
    border-radius: 3px;

    z-index: 1;

    transform-origin: 4px 0px;

    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1),
      background 0.5s cubic-bezier(0.77, 0.2, 0.05, 1), opacity 0.55s ease;
  }

  #menuToggle span:first-child {
    transform-origin: 0% 0%;
  }

  #menuToggle span:nth-last-child(2) {
    transform-origin: 0% 100%;
  }

  /* 
 * Transform all the slices of hamburger
 * into a crossmark.
 */
  #menuToggle input:checked ~ span {
    opacity: 1;
    transform: rotate(45deg) translate(-2px, -1px);
    background: #cdcdcd;
  }

  /*
 * But let's hide the middle one.
 */
  #menuToggle input:checked ~ span:nth-last-child(3) {
    opacity: 0;
    transform: rotate(0deg) scale(0.2, 0.2);
  }

  /*
 * Ohyeah and the last one should go the other direction
 */
  #menuToggle input:checked ~ span:nth-last-child(2) {
    transform: rotate(-45deg) translate(0, -1px);
     color: white;
  }

  /*
 * Make this absolute positioned
 * at the top left of the screen
 */
  #menu {
    position: absolute;
    width: 100vw;
    margin: -100px 0px 0 -50px;
    padding: 100px;
    padding-top: 125px;

    background: #232323;
    list-style-type: none;
    -webkit-font-smoothing: antialiased;
    /* to stop flickering of text in safari */

    transform-origin: 0% 0%;
    transform: translate(-100%, 0);

    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1);
  }

  #menu li {
    padding: 10px;
    font-size: 25px;
    font-weight: bolder;
    color: white;
    position: relative;
    right: 2px;

  }

  /*
 * And let's slide it in from the left
 */
  #menuToggle input:checked ~ ul {
    transform: none;
  }

  /* ----------- Google Pixel XL ----------- */

  /* Portrait and Landscape */
  @media screen and (device-width: 360px) and (device-height: 640px) and (-webkit-device-pixel-ratio: 4) {
    .nav-item a {
      display: none;
    }
    .left_property {
      display: none;
    }
  }
}


/* ----------- iPad Pro 12.9" ----------- */

/* Portrait and Landscape */
@media only screen 
  and (min-device-width: 1024px) 
  and (max-device-width: 1366px)
  and (-webkit-min-device-pixel-ratio: 2) {
    .left_property {
    color: white;
    font-family: "Avenir Next", "Avenir", sans-serif;
    width: 210px;
    height: 55px;
    background-color: #232323;
    border-right: 1px solid rgb(63, 60, 60);
    border-left: 1px solid rgb(63, 60, 60);
    position: absolute;
    left: 1cm;
  }
  .right_property {
  color: white;
  font-family: "Avenir Next", "Avenir", sans-serif;
  width: 270px;
  height: 55px;
  background-color: #232323;
  border-right: 1px solid rgb(63, 60, 60);
  border-left: 1px solid rgb(63, 60, 60);
  position: absolute;
  right: 0.1cm;
 
}

.navbar ul {
  list-style: none;
  display: flex;
  color: white;
  padding: 5px 10px;
  line-height: 10px;
}

.nav-item a {
  color: white;
  font-size: 09rem;
  font-weight: 400;
  text-decoration: none;
  transition: color 03s ease-out;
  padding: 5px 10px;
  line-height: 10px;
  font-weight: 600;
  font-size: small;
}
.right_logo{
  position: relative;
  bottom: 22px;
}
.subscribe{
  position: relative;
  bottom: 33px;
}

.marvel_unlimited{
  margin: auto;
  text-align: center;
  border-right: 0px solid rgb(63, 60, 60);
  
}
 

  .navbar ul {
    list-style: none;
    display: flex;
    color: white;
    padding: 5px 10px;
    line-height: 10px;
  }

  .nav-item a {
    color: white;
    font-size: 09rem;
    font-weight: 400;
    text-decoration: none;
    transition: color 03s ease-out;
    padding: 5px 10px;
    line-height: 10px;
    font-weight: 600;
    font-size: small;

  }

}

/* ----------- iPad 3, 4 and Pro 9.7" ----------- */

/* Portrait and Landscape */
@media only screen and (min-device-width: 768px) and (max-device-width: 1024px) and (-webkit-min-device-pixel-ratio: 2) {
  .left_property {
   display: none;
  }
  .right_property {
  color: white;
  font-family: "Avenir Next", "Avenir", sans-serif;
  width: 270px;
  height: 55px;
  background-color: #232323;
  border-right: 1px solid rgb(63, 60, 60);
  border-left: 1px solid rgb(63, 60, 60);
  position: absolute;
  right: 0.5cm;
 
}
.hide{
  display: none;
}

.navbar ul {
  list-style: none;
  display: flex;
  color: white;
  padding: 5px 10px;
  line-height: 10px;
}

.nav-item a {
  color: white;
  font-size: 09rem;
  font-weight: 400;
  text-decoration: none;
  transition: color 03s ease-out;
  padding: 5px 10px;
  line-height: 10px;
  font-weight: 600;
  font-size: small;
}
.right_logo{
  position: relative;
  bottom: 22px;
}
.subscribe{
  position: relative;
  bottom: 33px;
}

.marvel_unlimited{
  margin: auto;
  text-align: center;
  border-right: 0px solid rgb(63, 60, 60);
  
}
 

  .navbar ul {
    list-style: none;
    display: flex;
    color: white;
    padding: 5px 10px;
    line-height: 10px;
  }

  .nav-item a {
    color: white;
    font-size: 09rem;
    font-weight: 400;
    text-decoration: none;
    transition: color 03s ease-out;
    padding: 5px 10px;
    line-height: 10px;
    font-weight: 600;
    font-size: small;

  }
  
.nav_drawer_list a{
  font-size: x-small;
}
  body {
    margin: 0;
    padding: 0;

    /* make it look decent enough */
    background: #232323;
    color: #cdcdcd;
    font-family: "Avenir Next", "Avenir", sans-serif;
  }

  #menuToggle {
    display: block;
    position: relative;
    top: 20px;
    left: 30px;

    z-index: 1;

    -webkit-user-select: none;
    user-select: none;
  }

  #menuToggle a {
    text-decoration: none;
    color: #232323;

    transition: color 0.3s ease;
  }


  #menuToggle input {
    display: block;
    width: 40px;
    height: 32px;
    position: absolute;
    top: -7px;
    left: -5px;

    cursor: pointer;

    opacity: 0; /* hide this */
    z-index: 2; /* and place it over the hamburger */

    -webkit-touch-callout: none;
  }

  /*
 * Just a quick hamburger
 */
  #menuToggle span {
    display: block;
    width: 33px;
    height: 4px;
    margin-bottom: 5px;
    position: relative;

    background: #cdcdcd;
    border-radius: 3px;

    z-index: 1;

    transform-origin: 4px 0px;

    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1),
      background 0.5s cubic-bezier(0.77, 0.2, 0.05, 1), opacity 0.55s ease;
  }

  #menuToggle span:first-child {
    transform-origin: 0% 0%;
  }

  #menuToggle span:nth-last-child(2) {
    transform-origin: 0% 100%;
  }

  /* 
 * Transform all the slices of hamburger
 * into a crossmark.
 */
  #menuToggle input:checked ~ span {
    opacity: 1;
    transform: rotate(45deg) translate(-2px, -1px);
    background: #cdcdcd;
  }

  /*
 * But let's hide the middle one.
 */
  #menuToggle input:checked ~ span:nth-last-child(3) {
    opacity: 0;
    transform: rotate(0deg) scale(0.2, 0.2);
  }

  /*
 * Ohyeah and the last one should go the other direction
 */
  #menuToggle input:checked ~ span:nth-last-child(2) {
    transform: rotate(-45deg) translate(0, -1px);
     color: white;
  }

  /*
 * Make this absolute positioned
 * at the top left of the screen
 */
  #menu {
    position: absolute;
    width: 100vw;
    margin: -100px 0px 0 -50px;
    padding: 100px;
    padding-top: 125px;

    background: #232323;
    list-style-type: none;
    -webkit-font-smoothing: antialiased;
    /* to stop flickering of text in safari */

    transform-origin: 0% 0%;
    transform: translate(-100%, 0);

    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1);
  }

  #menu li {
    padding: 10px;
    font-size: 25px;
    font-weight: bolder;
    color: white;
    position: relative;
    right: 2px;

  }

  /*
 * And let's slide it in from the left
 */
  #menuToggle input:checked ~ ul {
    transform: none;
  }

}
</style>

<script>
export default {
  name: "Home",
};
</script>
