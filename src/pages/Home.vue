<template>
  <div class="home">
    <div class="container">
      <div class="profile-container">
        <img src="../assets/profile.jpg" alt="Profile Picture - Claudio Castro">
        <h1>Cláudio Luiz Castro</h1>
        <span>Front end Developer</span>
        <div class="icons-container">
          <a href="https://www.linkedin.com/in/claudiolcastro/"  target="blank"><img src="../assets/linkedin-icon.png" alt="LinkedIn Icon" target="blank"></a>
          <a href="https://github.com/claudiolcastro" target="blank"><img src="../assets/git-hub-icon.png" alt="GitHub Icon"></a>
          <a href="https://twitter.com/claudiolcastro" target="blank"><img src="../assets/twitter-icon.png" alt="Twitter Icon"></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home',
  components: {
  }
}
</script>

<style lang="scss" scoped>
  .container {
    width: 100%;
    height: 100vh;
    position: fixed;
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    background-image: url('../assets/home-bg_Fotor.jpg');
  }
  .profile-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 240px;
    // large screens
    @media (min-width: 1281px) {
      margin-top: 200px;
    }
    // ++ large screens
      @media (min-width: 1920px) {
        margin-top: 300px
      }
    // tablets
    @media (min-width: 768px) and (max-width: 1024px) {
      margin-top: 350px;
    }
    // mobile iphone 5
      @media (min-width: 320px) and (max-width: 374px) {
        margin-top: 200px;
      }
    img {
      width: 170px;
      height:170px;
      border-radius: 50%;
      border: 2px solid #f1f1f1;
      // ++ large screens
      @media (min-width: 1920px) {
        width: 200px;
        height: 200px;
      }
      // 4k screens
      @media (min-width: 1999px) {
        width: 300px;
        height: 300px;
      }
      // mobile iphone 5
      @media (min-width: 320px) and (max-width: 374px) {
        width: 120px;
        height:120px;
      }
    }
    h1 {
      color: #f1f1f1;
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 600;
      font-size: 2.4em;
      // 4k screens
      @media (min-width: 1999px) {
        font-size: 3.5em;
      }
      // mobile iphone 5
      @media (min-width: 320px) and (max-width: 374px) {
        font-size: 1.6em;
      }
    }
    span {
      color: #f1f1f1;
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 300;
      font-size: 1.6em;
      margin-top: -12px;
      // 4k screens
      @media (min-width: 1999px) {
        font-size: 2.5em;
      }
      // mobile iphone 5
      @media (min-width: 320px) and (max-width: 374px) {
        font-size: 1.2em;
      }
    }
  }
  .icons-container {
    width: 200px;
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
    img {
      width: 50px;
      height: 50px;
      border: none;
      border-radius: 0;
      // mobile
      @media (max-width: 768px) {
        width: 40px;
        height: 40px;
      }
    }
  }
</style>

