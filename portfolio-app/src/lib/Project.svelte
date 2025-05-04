<script>
      import { base } from '$app/paths';
</script>

<div class="project-row">

    <div class="project-box">
      <img src="{base}/flatland.png" alt="" />
      <p>I took the text of the book Flatland by Edwin Abbott and made it readable on a webpage, browser and mobile.</p>
      <a href="{base}/https://codeberg.org/Aleksejs-Buciks/C00300235-Aleksejs-Buciks-Flatland-Webpage"><button class="project-btn">See Project</button></a>
    </div>
  
    <div class="project-box">
      <img src="{base}/trainer.png" alt="" />
      <p>I created a simple collection game in JavaScript where you have to collect 10 pallets while an enemy chases you.</p>
      <a href="{base}/https://codeberg.org/UI-Programming-24-25/Aleksejs_Buciks_C00300235-UI-Programming-Module-Project"><button class="project-btn">See Project</button></a>
    </div>
  
    <div class="project-box">
      <img src="{base}/mega-man.png" alt="" />
      <p>In C++ I coded a mockup level of the classic game Mega Man from the Nintendo Entertainment System.</p>
      <a href="{base}/https://github.com/PeterLowe/springinteractive24-AleksejsBuciks"><button class="project-btn">See Project</button></a>
      
    </div>

  </div>

<style>
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