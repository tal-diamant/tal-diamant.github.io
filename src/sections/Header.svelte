<script>
  import menuIcon from '../assets/images/menu-icon.svg';
  let noTranslate = false;
</script>

<div class="wrapper">
  <div class="mobile-menu" class:noTranslate on:click={() => noTranslate = false}>
    <a href="#home">Home</a>
    <a href="#projects">Projects</a>
    <a href="#skills">Skills</a>
    <a href="#contact">Contact</a>
  </div>
  <div class="container">
    <div class="navbar">
      <div>
        <a href="#">
          <img src="/images/favicon.png" alt="" />
        </a>
      </div>
      <div class="menu-toggler" on:click={() => (noTranslate = !noTranslate)}>
        <img src={menuIcon} alt="mobile menu button" />
      </div>
      <div class="links">
        <a href="#home">Home</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
  </div>
</div>

<style>
  .wrapper {
    position: fixed;
    width: 100%;
    height: 2.62rem;
    z-index: 1;
  }

  .container {
    position: relative;
    width: 100%;
    background-color: black;
    padding: 5px 5%;
    z-index: 1;
  }

  .navbar {
    max-width: 1200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: white;
    margin: 0 auto;
  }

  .links {
    display: flex;
    gap: 30px;
    font-size: 1.2rem;
  }

  .menu-toggler {
    display: none;
  }

  .mobile-menu {
    display: none;
  }

  @media (max-width: 500px) {
    .links {
      display: none;
    }

    .menu-toggler {
      display: block;
      cursor: pointer;
    }

    .menu-toggler img {
      width: 30px;
      height: 30px;
    }

    .mobile-menu {
      display: flex;
      flex-direction: column;
      position: absolute;
      background-color: black;
      left: 0;
      top: 2.65rem;
      translate: 0 -110%;
      width: 100%;
      z-index: 1;
      transition: translate 0.25s;
    }

    .mobile-menu a {
      color: #dadada;
      font-size: 1.5rem;
      padding: 5px 10px
    }

    .mobile-menu a:hover {
      color: white;
    }

    .noTranslate {
      translate: 0 0;
    }
  }
</style>
