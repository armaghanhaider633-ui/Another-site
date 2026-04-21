# Another-site<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>3D Portfolio Website</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial, sans-serif;
scroll-behavior:smooth;
}

body{
background:linear-gradient(135deg,#00c853,#ffffff,#2962ff);
color:#111;
overflow-x:hidden;
}

/* HERO */
.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
background:rgba(255,255,255,0.2);
backdrop-filter:blur(10px);
}

.logo{
font-size:90px;
animation:float 3s ease-in-out infinite;
}

@keyframes float{
0%,100%{transform:translateY(0)}
50%{transform:translateY(-20px)}
}

/* SECTION COMMON */
.section{
min-height:100vh;
padding:60px 20px;
display:flex;
flex-direction:column;
align-items:center;
justify-content:center;
gap:30px;
}

h1{
font-size:40px;
}

/* SERVICES */
.services{
display:flex;
gap:20px;
flex-wrap:wrap;
justify-content:center;
}

.card{
width:250px;
height:320px;
background:white;
border-radius:20px;
overflow:hidden;
box-shadow:0 10px 30px rgba(0,0,0,0.2);
transition:0.5s;
transform-style:preserve-3d;
}

.card:hover{
transform:rotateY(15deg) scale(1.05);
}

.card img{
width:100%;
height:70%;
object-fit:cover;
}

.card h3{
text-align:center;
padding:10px;
}

/* VIDEO GRID */
.videos{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:20px;
width:90%;
}

video{
width:100%;
border-radius:15px;
box-shadow:0 10px 20px rgba(0,0,0,0.2);
}

/* PROJECTS */
.projects{
display:flex;
flex-wrap:wrap;
gap:20px;
justify-content:center;
}

.project{
width:300px;
height:200px;
background:white;
border-radius:15px;
overflow:hidden;
transition:0.4s;
box-shadow:0 8px 20px rgba(0,0,0,0.2);
}

.project:hover{
transform:scale(1.08);
}

.project img{
width:100%;
height:100%;
object-fit:cover;
}

/* CONTACT */
.contact-box{
display:flex;
flex-direction:column;
gap:10px;
width:300px;
}

input,textarea{
padding:10px;
border:none;
border-radius:10px;
outline:none;
}

button{
padding:10px;
border:none;
border-radius:10px;
background:#2962ff;
color:white;
cursor:pointer;
}

button:hover{
background:#00c853;
}
</style>
</head>

<body>

<!-- HERO -->
<div class="hero">
  <div class="logo">🎥</div>
  <h2>Welcome to My 3D Portfolio</h2>
  <p>Scroll to explore services, work & contact</p>
</div>

<!-- SERVICES -->
<div class="section">
  <h1>Services</h1>
  <div class="services">

    <div class="card">
      <img src="https://images.unsplash.com/photo-1626785774573-4b799315345d">
      <h3>Video Editing</h3>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1522542550221-31fd19575a2d">
      <h3>Website Development</h3>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1611926653458-09294b3142bf">
      <h3>Google Ads</h3>
    </div>

  </div>
</div>

<!-- DEMO VIDEOS -->
<div class="section">
  <h1>Demo & Editing Videos</h1>
  <div class="videos">

    <video controls>
      <source src="https://www.w3schools.com/html/mov_bbb.mp4">
    </video>

    <video controls>
      <source src="https://www.w3schools.com/html/movie.mp4">
    </video>

  </div>
</div>

<!-- PROJECTS -->
<div class="section">
  <h1>Projects</h1>
  <div class="projects">

    <div class="project">
      <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085">
    </div>

    <div class="project">
      <img src="https://images.unsplash.com/photo-1522199710521-72d69614c702">
    </div>

    <div class="project">
      <img src="https://images.unsplash.com/photo-1557804506-669a67965ba0">
    </div>

  </div>
</div>

<!-- CONTACT -->
<div class="section">
  <h1>Contact</h1>

  <div class="contact-box">
    <input type="text" placeholder="Name">
    <input type="email" placeholder="Email">
    <textarea placeholder="Message"></textarea>
    <button>Send Message</button>
  </div>

</div>

</body>
</html>
