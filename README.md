# diaryme
<!DOCTYPE html>
<html>
<title>DIARY ME</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
body,h1,h2,h3,h4,h5,h6 {font-family: "Raleway", sans-serif}
body, html {
    height: 100%;
    line-height: 1.8;
}
.w3-bar .w3-button {
    padding: 16px;
}
</style>

<body>
<!-- Navbar (sit on top) -->
<div class="w3-top">
  <div class="w3-bar w3-white w3-card" id="myNavbar">
    <img src="logo.jpg" width="10%">
    <!-- Right-sided navbar links -->
    <div class="w3-right w3-hide-small">
      <a href="#about" class="w3-bar-item w3-button">HOME</a>
      <a href="#team" class="w3-bar-item w3-button"><i class="fa fa-user"></i> DIARY ME</a>
      <a href="#work" class="w3-bar-item w3-button"><i class="fa fa-th"></i> GALLERY</a>
      <a href="#contact" class="w3-bar-item w3-button"><i class="fa fa-envelope"></i> CONTACT</a>
    </div>
    <!-- Hide right-floated links on small screens and replace them with a menu icon -->

    <a href="javascript:void(0)" class="w3-bar-item w3-button w3-right w3-hide-large w3-hide-medium" onclick="w3_open()">
      <i class="fa fa-bars"></i>
    </a>
  </div>
</div>

<!-- Sidebar on small screens when clicking the menu icon -->
<nav class="w3-sidebar w3-bar-block w3-black w3-card w3-animate-left w3-hide-medium w3-hide-large" style="display:none" id="mySidebar">
  <a href="javascript:void(0)" onclick="w3_close()" class="w3-bar-item w3-button w3-large w3-padding-16">Close ×</a>
  <a href="#about" onclick="w3_close()" class="w3-bar-item w3-button">HOME</a>
  <a href="#team" onclick="w3_close()" class="w3-bar-item w3-button">DIARY ME</a>
  <a href="#work" onclick="w3_close()" class="w3-bar-item w3-button">GALLERY</a>
  <a href="#contact" onclick="w3_close()" class="w3-bar-item w3-button">CONTACT</a>
</nav>

</header>
<!-- HOME Section -->
<div class="w3-container" style="padding:128px 16px" id="about">
    <h3 class="w3-center">HOME</h3>
</div>

<!-- DIARY ME Section -->
<div class="w3-container" style="padding:128px 16px" id="team">
  <h3 class="w3-center">DIARY ME</h3>
</div>

<!-- GALLERY Section -->
<div class="w3-container" style="padding:128px 16px" id="work">
  <h3 class="w3-center">GALLERY</h3>
  <!-- photo -->
     <div class="w3-row">
   <div class="w3-third">
     <img src="img1.jpg" style="width:100%" onclick="onClick(this)" alt="A boy surrounded by beautiful nature">
     <img src="img.jpg" style="width:100%" onclick="onClick(this)" alt="What a beautiful scenery this sunset">
     <img src="img.jpg" style="width:100%" onclick="onClick(this)" alt="The Beach. Me. Alone. Beautiful">
   </div>

   <div class="w3-third">
     <img src="img2.jpg" style="width:100%" onclick="onClick(this)" alt="Quiet day at the beach. Cold, but beautiful">
     <img src="img.jpg" style="width:100%" onclick="onClick(this)" alt="Waiting for the bus in the desert">
     <img src="img.jpg" style="width:100%" onclick="onClick(this)" alt="Nature again.. At its finest!">
   </div>

   <div class="w3-third">
     <img src="img1.jpg" style="width:100%" onclick="onClick(this)" alt="Canoeing again">
     <img src="img.jpg" style="width:100%" onclick="onClick(this)" alt="A girl, and a train passing">
     <img src="img.jpg" style="width:100%" onclick="onClick(this)" alt="What a beautiful day!">
   </div>
 </div>
</div>

<!-- Modal for full size images on click-->
<div id="modal01" class="w3-modal w3-black" onclick="this.style.display='none'">
  <span class="w3-button w3-xxlarge w3-black w3-padding-large w3-display-topright" title="Close Modal Image">×</span>
  <div class="w3-modal-content w3-animate-zoom w3-center w3-transparent w3-padding-64">
    <img id="img01" class="w3-image">
    <p id="caption" class="w3-opacity w3-large"></p>
  </div>
</div>

<!-- Skills Section -->
<div class="w3-container w3-light-grey w3-padding-64">
  <div class="w3-row-padding">
    <div class="w3-col m6">
      <h3>Our Skills.</h3>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod<br>
      tempor incididunt ut labore et dolore.</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod<br>
      tempor incididunt ut labore et dolore.</p>
    </div>

<!-- Contact Section -->
<div class="w3-container w3-light-grey" style="padding:128px 16px" id="contact">
  <h3 class="w3-center">CONTACT</h3>
  <p class="w3-center w3-large">Lets get in touch. Send us a message:</p>
  <div class="w3-row-padding" style="margin-top:64px">
    <div class="w3-half">
      <p><i class="fa fa-map-marker fa-fw w3-xxlarge w3-margin-right"></i> Songkla, thailand</p>
      <p><i class="fa fa-phone fa-fw w3-xxlarge w3-margin-right"></i> Phone: 0847462470</p>
      <p><i class="fa fa-envelope fa-fw w3-xxlarge w3-margin-right"> </i> Email: bankpanjr12@gmail.com</p>
      <br>
      <form action="/action_page.php" target="_blank">
        <p><input class="w3-input w3-border" type="text" placeholder="Name" required name="Name"></p>
        <p><input class="w3-input w3-border" type="text" placeholder="Email" required name="Email"></p>
        <p><input class="w3-input w3-border" type="text" placeholder="Subject" required name="Subject"></p>
        <p><input class="w3-input w3-border" type="text" placeholder="Message" required name="Message"></p>
        <p>
          <button class="w3-button w3-black" type="submit">
            <i class="fa fa-paper-plane"></i> SEND MESSAGE
          </button>
        </p>
      </form>
    </div>
    <div class="w3-half">
      <!-- Add Google Maps -->
      <div class="w3w3-animate-left">
      <img src="map.jpg" width="150%">
    </div>
    </div>
  </div>
</div>

<!-- Footer -->
<footer class="w3-center w3-black w3-padding-64">
  <div class="w3-xlarge w3-section">
    <i class="fa fa-facebook-official w3-hover-opacity"></i>
    <i class="fa fa-instagram w3-hover-opacity"></i>
    <i class="fa fa-snapchat w3-hover-opacity"></i>
    <i class="fa fa-pinterest-p w3-hover-opacity"></i>
    <i class="fa fa-twitter w3-hover-opacity"></i>
    <i class="fa fa-linkedin w3-hover-opacity"></i>
  </div>
  <p>Powered by <a href="https://web.facebook.com/pop.magaritar?ref=bookmarks" title="DIARY ME" target="_blank" class="w3-hover-text-green">DIARY ME</a></p>
</footer>

</body>
</html>
