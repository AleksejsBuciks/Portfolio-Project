<script>

</script>

<div class="text-row">

    <div class="box">
      <div class="logo html">HTML<br>5</div>
      <p>I've worked extensively with HTML to create structured, responsive web pages and ensure cross-browser compatibility.</p>
    </div>
  
    <div class="box">
      <div class="logo js">JS</div>
      <p>I have hands-on experience with JavaScript, building dynamic and interactive web applications.</p>
    </div>
  
    <div class="box">
      <div class="logo css">C++</div>
      <p>I have experience using C++ to develop efficient, high-performance applications, utilizing object-oriented principles and managing memory effectively.</p>
    </div>
  
  </div>

<div class="project-row">

    <div class="project-box">
      <img src="flatland.png" alt="" />
      <p>I took the text of the book Flatland by Edwin Abbott and made it readable on a webpage, browser and mobile.</p>
      <a href="https://codeberg.org/Aleksejs-Buciks/C00300235-Aleksejs-Buciks-Flatland-Webpage"><button class="project-btn">See Project</button></a>
    </div>
  
    <div class="project-box">
      <img src="trainer.png" alt="" />
      <p>I created a simple collection game in JavaScript where you have to collect 10 pallets while an enemy chases you.</p>
      <a href="https://codeberg.org/UI-Programming-24-25/Aleksejs_Buciks_C00300235-UI-Programming-Module-Project"><button class="project-btn">See Project</button></a>
    </div>
  
    <div class="project-box">
      <img src="mega-man.png" alt="" />
      <p>In C++ I coded a mockup level of the classic game Mega Man from the Nintendo Entertainment System.</p>
      <a href="https://github.com/PeterLowe/springinteractive24-AleksejsBuciks"><button class="project-btn">See Project</button></a>
      
    </div>

  </div>

<style>

.text-row {
    margin-top: 100px;
}

.text-row {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    margin-top: 250px;
    gap: 30px;
    flex-wrap: wrap;
}

.box {
    background-color: #7d0edf;
    padding: 20px;
    border-radius: 10px;
    width: 280px;
    text-align: center;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
    color: white;
}

.logo {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    margin: 0 auto 10px auto;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: bold;
    font-size: 16px;
    color: white;
}

.logo.html {
    background-color: #e44d26;
}

.logo.js {
    background-color: #f7df1e;
    color: black;
}

.logo.css {
    background-color: #4dabf7;
}

.project-row {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 30px;
    margin: 60px auto;
}

.project-box {
    background-color: #141d26;
    color: white;
    width: 260px;
    padding: 20px;
    border-radius: 12px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
    text-align: center;
}

.project-box img {
    width: 100%;
    height: auto;
    border-radius: 8px;
    margin-bottom: 15px;
}

.project-btn {
    margin-top: 15px;
    background-color: #7d0edf;
    border: none;
    color: white;
    padding: 10px 16px;
    font-size: 14px;
    border-radius: 6px;
    cursor: pointer;
}

.project-btn:hover {
    background-color: #a026ff;
}

</style>