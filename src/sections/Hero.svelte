<script>
  import arrowDown from '../assets/images/arrow-down.svg';
</script>

<div id="home" class="container">
  <div class="hero">
    <div class="content">
      <h1 class="desktop-title">Web Developer | Game Developer</h1>
      <h1 class="mobile-title">Web Developer<br />Game Developer</h1>
      <h4>Turning ideas into reality.</h4>
    </div>
    <a href="#projects" class="arrow"
      ><img class="arrow-down" src={arrowDown} alt="arrow down" /></a
    >
  </div>
</div>

<style>
  .container {
    background-image: url(/images/desert.jpg);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    width: 100%;
    height: 100vh;
  }

  .hero {
    height: 100%;
    background-color: #0007;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
  }

  .content {
    text-align: center;
    color: white;
    padding: 0 20px;
  }

  h1 {
    font-size: clamp(3rem, 4.5vw, 4rem);
  }

  h4 {
    margin-top: 2rem;
    color: #d9d9d9;
    font-size: 1.3rem;
  }

  .arrow {
    position: absolute;
    bottom: 20px;
  }

  .mobile-title {
    display: none;
  }

  @media (max-width: 1000px) {
    .desktop-title {
      display: none;
    }

    .mobile-title {
      display: block;
      font-size: 3rem;
    }
  }

  @media (max-width: 415px) {
    .mobile-title {
        font-size: 2.2rem;
    }
  }
</style>
