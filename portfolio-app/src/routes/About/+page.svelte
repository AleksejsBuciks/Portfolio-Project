<script>
    function goHome() {
      window.location.href = '/'; 
    }
  </script>
  
  <div class="header" on:click={goHome}>
    Portfolio
  </div>
  
  <div class="about-container">
    <div class="about-text">
      <p>
        I'm a developer with experience in HTML, JavaScript, and C++, passionate about creating dynamic web apps.
        Outside of coding and web design, I have a deep fondness for video games, which sparks my creativity.
        I'm always ready to learn and collaborate, I strive to deliver impactful results in both tech and gaming.
      </p>
    </div>
    <div class="about-image">
      <img src="me.png" alt="">
    </div>
  </div>
  
  <style>

  body {
  background-color: #1e2a38;
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}

.header {
  text-align: center;
  font-size: 24px;
  color: #7d0edf;
  margin-top: 20px;
  cursor: pointer;
}

.about-container {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  margin: 60px auto;
  max-width: 900px;
  border: 2px solid #7d0edf;
  padding: 30px;
}

.about-text {
  flex: 1;
  color: white;
  padding-right: 30px;
  font-size: 18px;
  line-height: 1.6;
}

.about-image {
  flex: 1;
  border-left: 2px solid #7d0edf;
  margin-left: 30px;
  min-height: 300px; 
}

.about-image img {
  width: 100%;
  height: auto;
  max-height: none; 
  object-fit: contain;
  display: block;
  margin: 0 auto;
}
  </style>
  