
# Ex02 Commercial Website
## Date: 11/08/2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

### index.html

```

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Leaf & Bean - Nature Café</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <div class="logo">Leaf & Bean</div>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#menu">Menu</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

<section id="home" class="hero">
  <div class="hero-overlay">
    <h1>Welcome to Leaf & Bean</h1>
    <p>Your cozy corner for fresh brews and nature’s goodness.</p>
  </div>
</section>


  <section id="menu" class="menu">
    <h2>Our Specialties</h2>
    <div class="menu-container">
      <div class="item">
        <img src="coffee.jpg" alt="Coffee">
        <h3>Organic Coffee</h3>
        <p>Rich aroma, pure taste, sustainably sourced beans.</p>
      </div>
      <div class="item">
        <img src="salad.jpg" alt="Salad">
        <h3>Garden Salad</h3>
        <p>Fresh greens and herbs straight from local farms.</p>
      </div>
      <div class="item">
        <img src="dessert.jpg" alt="Dessert">
        <h3>Vegan Desserts</h3>
        <p>Sweet treats without guilt, made from natural ingredients.</p>
      </div>
    </div>
  </section>

  <section id="about" class="about">
    <h2>About Us</h2>
    <p>
      At Leaf & Bean, we believe in serving food that’s good for you and the planet. 
      Our café is a cozy retreat where you can enjoy organic coffee, farm-fresh meals, and a peaceful atmosphere.
    </p>
  </section>

  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message" rows="5" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Leaf & Bean Café. All rights reserved.</p>
  </footer>
</body>
</html>


```

### styles.css

```

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', sans-serif;
  line-height: 1.6;
  color: #3a3a3a;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #4b6043;
  color: #fff;
}

header .logo {
  font-size: 1.8rem;
  font-weight: bold;
}

header nav ul {
  display: flex;
  list-style: none;
}

header nav ul li {
  margin-left: 1.5rem;
}

header nav ul li a {
  color: #fff;
  text-decoration: none;
  transition: color 0.3s;
}

header nav ul li a:hover {
  color: #d4edc9;
}
.hero {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: url('bg.png') center/cover no-repeat;
  color: #fff;
  text-align: center;
}

.hero-overlay {
  background-color: rgba(0, 0, 0, 0.4);
  padding: 2rem;
  border-radius: 10px;
}

.hero h1 {
  font-size: 3rem;
  margin-bottom: 0.5rem;
}

.hero p {
  font-size: 1.3rem;
  max-width: 600px;
  margin: auto;
}


.cta-button {
  padding: 0.8rem 1.5rem;
  background-color: #d4edc9;
  color: #2f4f2f;
  text-decoration: none;
  border-radius: 30px;
  font-weight: bold;
  transition: background-color 0.3s;
}

.cta-button:hover {
  background-color: #c2dbb8;
}

.menu {
  padding: 2rem;
  text-align: center;
  background-color: #f8f8f8;
}

.menu h2 {
  margin-bottom: 1.5rem;
}

.menu-container {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}

.menu-container .item {
  flex: 1 1 30%;
  background: #fff;
  margin: 1rem;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.menu-container img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.menu-container h3 {
  margin: 1rem 0 0.5rem;
}

.menu-container p {
  padding: 0 1rem 1rem;
}

.about {
  padding: 2rem;
  text-align: center;
}

.contact {
  padding: 2rem;
  text-align: center;
  background-color: #f8f8f8;
}

.contact form {
  max-width: 500px;
  margin: auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.contact input,
.contact textarea {
  padding: 0.75rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.contact button {
  padding: 0.75rem 1.5rem;
  background-color: #4b6043;
  color: #fff;
  border: none;
  border-radius: 30px;
  cursor: pointer;
}

.contact button:hover {
  background-color: #3a4c34;
}

footer {
  text-align: center;
  padding: 1rem;
  background-color: #4b6043;
  color: #fff;
}

@media (max-width: 768px) {
  header {
    flex-direction: column;
    text-align: center;
  }

  header nav ul {
    flex-direction: column;
    margin-top: 1rem;
  }

  header nav ul li {
    margin: 0.5rem 0;
  }

  .menu-container {
    flex-direction: column;
  }

  .menu-container .item {
    flex: 1 1 100%;
  }
}

```
## OUTPUT

![alt text](<Screenshot 2025-08-13 193152.png>) 

![alt text](<Screenshot 2025-08-13 193205.png>)

![alt text](<Screenshot 2025-08-13 193220.png>) 

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.

