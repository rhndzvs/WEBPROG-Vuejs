<template>
    <header>
        <h1>Welcome to My Personal Website!</h1>
        <nav>
          <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About Me</a></li>
            <li><a href="#picture-gallery">Picture Gallery</a></li>
            <li><a href="#resources">Resources</a></li>
          </ul>
        </nav>
      </header>
    
      <main>
        <section id="home" class="center-content">
          <img src="https://github.com/rhndzvs/WEBPROG-Personal-Website/blob/feature/2_RZB_customize_my_website/home/pictures/FORMAL%20PICTURE.jpg?raw=true" alt="Profile Picture" class="profile-pic">
          <h2>Hi! I am Rhundei Zen R. Ballesteros</h2>
          <p>IT Student</p>
          <button onclick="clickMe()">Click Me</button>
        </section>
    
        <div class="social-links">
          <a href="#"><img src="https://cdn2.iconfinder.com/data/icons/social-icons-33/128/Facebook-512.png" alt="Facebook"></a>
          <a href="#"><img src="https://img.freepik.com/free-vector/instagram-logo_1199-122.jpg?semt=ais_hybrid" alt="Instagram"></a>
          <a href="#"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRokEYt0yyh6uNDKL8uksVLlhZ35laKNQgZ9g&s" alt="LinkedIn"></a>
        </div>
      </main>
    
      <footer>
        <p class="footer-text">© 2024 Rhundei Zen Ballesteros</p>
      </footer>
</template>

<script>
</script>

<style>
body {
  font-family: Arial, sans-serif;
  background-color: #f0fff8;
  color: #004d40;
  text-align: center;
}

header {
  background-color: #00695c;
  color: white;
  padding: 10px 0;
  text-align: center;
}

header h1 {
  margin-bottom: 15px;
}

nav {
  background-color: white;
  padding: 10px 0;
}

nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  margin: 0;
  padding: 0;
}

nav li {
  margin: 0 30px;
}

nav a {
  color: #00695c;
  padding: 12px 25px;
  text-align: center;
  border: none;
  text-decoration: none;
  font-weight: bold;
  font-size: 1.1em;
  transition-duration: 0.4s;
}

nav a:hover {
  background-color: #004d40;
  color: white;
}

.center-content {
  padding: 50px 20px;
}

.profile-pic {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 4px solid #00695c;
  margin-bottom: 20px;
}

h2 {
  color: #00695c;
  margin-bottom: 10px;
}

p {
  font-size: 1.2em;
  color: #333;
  margin-bottom: 20px;
}

button {
  background-color: #00695c;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  font-size: 1em;
  cursor: pointer;
  transition: background-color 0.3s;
}

button:hover {
  background-color: #004d40;
}

.social-links {
  margin-top: 30px;
}

.social-links img {
  width: 40px;
  margin: 0 10px;
  transition: transform 0.3s;
}

.social-links img:hover {
  transform: scale(1.01);
}

footer {
  background-color: #00695c;
  color: white;
  padding: 10px;
  margin-top: 30px;
}

.footer-text {
  font-family: Arial, sans-serif;
  color: white;
}
</style>