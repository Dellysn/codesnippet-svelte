<script>
  let show = false;
  const toggleNav = () => {
    show === true ? (show = false) : (show = true);
  };
</script>

<style>
  nav {
    background-color: rgba(220, 20, 60, 0.829);
    color: #f0f0f0;
    position: relative;
  }
  img {
    width: 100%;
  }
  .navbar-brand {
    width: 115px;
  }
  a.nav-link {
    color: #fff !important;
  }
  .nav-link:hover {
    color: #333 !important;
  }
  .mobile-nav {
    visibility: hidden;
    height: 100vh;
    position: fixed;
    background-color: #06141ffa;
    width: 100%;
    left: 0;
    top: 0%;
    z-index: -999;
  }
  .mobile-nav-menu {
    visibility: hidden;
    margin: 3rem auto;
    max-width: 22rem;
    text-align: center;
    background: #dc143cc0;
    border-radius: 10px;
    padding: 2rem;
  }
  .mobile-nav.show {
    visibility: visible;
    z-index: 999;
  }
  .mobile-nav-menu.show {
    visibility: visible;
    z-index: 999;
  }
  .mobile-nav-menu a.nav-link {
    color: #000;
  }
  .mobile-nav-toggler {
    display: none;
  }
  .close-nav {
    float: right;
    margin: 0.76rem 0.9rem 0 0;
    font-weight: bolder;
    font-family: "Raleway";
    border-radius: 50%;
    text-align: center;
    line-height: 32px;
  }
  @media (max-width: 990px) {
    .navbar-toggler {
      display: none;
    }
    .mobile-nav-toggler {
      display: initial;
      background: transparent;
      color: #fff;
    }
  }
</style>

<nav class="navbar navbar-expand-lg navbar-light">
  <!-- svelte-ignore a11y-missing-attribute -->
  <div class="navbar-brand" href="#"><img src="images/Logo.png" /></div>
  <button class="mobile-nav-toggler" on:click={toggleNav}> &#x2630; </button>
  <button
    class="navbar-toggler"
    type="button"
    data-toggle="collapse"
    data-target="#navbarNav"
    aria-controls="navbarNav"
    aria-expanded="false"
    aria-label="Toggle navigation">
    <span class="navbar-toggler-icon" />
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav ml-auto">
      <li class="nav-item">
        <a class="nav-link active" href="#slide">HOME</a>
      </li>
      <li class="nav-item"><a class="nav-link" href="#about">ABOUT US</a></li>
      <li class="nav-item">
        <a class="nav-link" href="#services">SERVICES</a>
      </li>
      <li class="nav-item"><a class="nav-link" href="#team">OUR TEAM</a></li>
      <li class="nav-item">
        <a class="nav-link" href="#price">PRICE PLANS</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#testimonial">TESTIMONIAL</a>
      </li>
      <li class="nav-item"><a class="nav-link" href="#contact">CONTACT</a></li>
    </ul>
  </div>
  <div class:show class="mobile-nav   navbar-collapse" id="navbarNav">
    <span class="close-nav" on:click={toggleNav}>X</span>
    <ul class:show class="navbar-nav ml-auto mobile-nav-menu show">
      <li class="nav-item">
        <a class="nav-link active" href="#slide">HOME</a>
      </li>
      <li class="nav-item"><a class="nav-link" href="#about">ABOUT US</a></li>
      <li class="nav-item">
        <a class="nav-link" href="#services">SERVICES</a>
      </li>
      <li class="nav-item"><a class="nav-link" href="#team">OUR TEAM</a></li>
      <li class="nav-item">
        <a class="nav-link" href="#price">PRICE PLANS</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#testimonial">TESTIMONIAL</a>
      </li>
      <li class="nav-item"><a class="nav-link" href="#contact">CONTACT</a></li>
    </ul>
  </div>
</nav>
