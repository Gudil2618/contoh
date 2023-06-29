<template>
  <div id="app">
    <!-- Navigation-->
    <header>
        <nav class="navbar navbar-expand-lg navbar-light fixed-top" id="mainNav">
            <div class="container px-4 px-lg-5">
              <a class="navbar-brand ms-5" href="#masthead">
                <img src="./assets/starbucks-logo.jpeg" alt="" width="60px"></a>
                <button class="navbar-toggler navbar-toggler-right" data-bs-toggle="collapse" data-bs-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
                    Menu
                    <i class="fas fa-bars"></i>
                </button>     
                <div class="collapse navbar-collapse ms-5" id="navbarResponsive">
                    <ul class="navbar-nav">
                        <li class="nav-item"><a class="nav-link" href="">Menu</a></li>
                        <li class="nav-item ms-5"><a class="nav-link" href="">CoffeHouse</a></li>
                        <li class="nav-item ms-5"><a class="nav-link" href="">Promo</a></li>
                        <li class="nav-item ms-5"><a class="nav-link" href="">About as</a></li>
                    </ul>
                    <div class="search-box">
                      <input class="search-txt" type="text" name="" placeholder="Type to search"/>
                      <a class="search-btn" href="#">
                          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
                            <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
                          </svg>
                      </a>
                  </div>
                </div>
            </div>
        </nav>
    </header>
    <!-- Navigation -->
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
            window.addEventListener("scroll", function()
            {
                var header = document.querySelector("header");
             header.classList.toggle("sticky",window.scrollY  > 0);
            })
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.navbar-nav{
  font-family: Impact, 'Arial Narrow Bold', sans-serif;
}
.search-box{
    position: absolute;
    top: 55%;
    left: 80%;
    transform: translate(-50%,-50%);
    background: #2b6546;
    height: 42px;
    border-radius: 42px;
    padding: 9px;
}
.search-box:hover > .search-txt{
    width: 200px;
    padding: 0 6px;
}
.search-btn{
    color: #fff;
    float: right;
    width: 22px;
    height: 22px;
    border-radius: 50%;
    background: #08ab5400;
    display: flex;
    justify-content: center;
    align-items: center;
}
.search-txt{
    border: none;
    background: none;
    outline: none;
    float: left;
    padding: 0;
    color: white;
    font-size: 15px;
    transition: 0.4s;
    line-height: 25px;
    width: 0px;
}
/* AA */
header{
    display: flex;
    position: fixed;
    align-items: center;
    justify-content: space-between;
    padding: 20px 65px;
    z-index: 1000;
    width: 100%;
    top: 0;
    left: 0;
    height: fit-content;
    transition: 0.6s;
}

header.sticky{
    padding: 5px 100px;
    background: #fff;
    min-height: 70px;
}

header ul{
    display: flex;  
    align-items: center;
    justify-content: center;
}

header ul li{
    list-style: none;
    padding: 0 20px;
    position: relative;
}

header ul li a{
    text-decoration: none;
    font-size: 16px;
    font-weight: 600;
    color: #1a1a1a;
    transition: 0.3s ease;
}

header.sticky ul li a{
    color: #000;
    font-size: 16px;
}

header ul li a:hover, 
#navbar li a.active {
    color: purple;
}

header ul a.active::after {
    content:"";
    width: 30%;
    height: 3px;
    background: purple; 
    position: absolute;
    bottom:-6px;
    left: 20px;
    border-radius: 20%;
}
.sticky-top {
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  z-index: 1020;
}

@media (min-width: 576px) {
  .sticky-sm-top {
    position: -webkit-sticky;
    position: sticky;
    top: 0;
    z-index: 1020;
  }
}
@media (min-width: 768px) {
  .sticky-md-top {
    position: -webkit-sticky;
    position: sticky;
    top: 0;
    z-index: 1020;
  }
}
@media (min-width: 992px) {
  .sticky-lg-top {
    position: -webkit-sticky;
    position: sticky;
    top: 0;
    z-index: 1020;
  }
}
@media (min-width: 1200px) {
  .sticky-xl-top {
    position: -webkit-sticky;
    position: sticky;
    top: 0;
    z-index: 1020;
  }
}
@media (min-width: 1400px) {
  .sticky-xxl-top {
    position: -webkit-sticky;
    position: sticky;
    top: 0;
    z-index: 1020;
  }
}
</style>
