# Ex.07 Restaurant Website
# Date:
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
style.css

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', sans-serif;
}

body {
    background-color: #fffaf0;
    color: #333;
}

/* HEADER */
header {
    background: linear-gradient(90deg, #8b0000, #b22222);
    color: white;
    padding: 25px;
    text-align: center;
}

/* NAVBAR */
nav {
    background-color: #222;
    display: flex;
    justify-content: center;
    gap: 40px;
}

nav a {
    color: white;
    padding: 15px 0;
    text-decoration: none;
    font-size: 16px;
    position: relative;
}

nav a::after {
    content: "";
    width: 0;
    height: 2px;
    background: #ffcc00;
    position: absolute;
    bottom: 8px;
    left: 0;
    transition: 0.3s;
}

nav a:hover::after {
    width: 100%;
}

/* HERO SECTION (FULL SCREEN) */
.hero {
    height: 90vh;
    background: url("../images/hero.jpg") center/cover no-repeat;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
}

.hero div {
    background: rgba(0,0,0,0.5);
    padding: 40px;
    border-radius: 15px;
}

.hero h2 {
    font-size: 40px;
    margin-bottom: 15px;
}

/* SECTION */
.section {
    padding: 70px 40px;
    text-align: center;
}

.section h2 {
    font-size: 32px;
    margin-bottom: 30px;
}

/* CARD LAYOUT */
.card-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 30px;
}

/* MENU CARD */
.card {
    background-color: #fff;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 10px 25px rgba(0,0,0,0.15);
    transition: transform 0.3s;
}

.card:hover {
    transform: translateY(-10px);
}

.card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.card .content {
    padding: 20px;
}

.card h3 {
    margin-bottom: 10px;
}

/* BUTTON */
.btn {
    display: inline-block;
    margin-top: 10px;
    padding: 8px 15px;
    background-color: #b22222;
    color: white;
    border-radius: 5px;
    text-decoration: none;
}

/* FOOTER */
footer {
    background-color: #222;
    color: white;
    padding: 15px;
    text-align: center;
}

restaurant.html

<!DOCTYPE html>
<html>
<head>
    <title>Delish Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Delish Restaurant</h1>
    <p>Fresh - Tasty - Hygienic</p>
</header>

<nav>
    <a href="restaurant.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="services.html">Services</a>
    <a href="contact.html">Contact</a>
</nav>

<section class="hero">
    <div>
        <h2>Welcome to Delish</h2>
        <p>Experience food made with love</p>
    </div>
</section>

<section class="section">
    <h2>Why Choose Us?</h2>
    <p>Fresh ingredients - Skilled chefs - Best service</p>
</section>

<footer>
    <p>2025 Delish Restaurant</p>
</footer>

</body>
</html>

menu.html

<!DOCTYPE html>
<html>
<head>
    <title>Menu - Delish Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Our Menu</h1>
</header>

<nav>
    <a href="restaurant.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="services.html">Services</a>
    <a href="contact.html">Contact</a>
</nav>

<section class="section">
    <div class="card-container">

        <div class="card">
            <img src="burger.webp">
            <div class="content">
                <h3>Veg Burger</h3>
                <p>120-Rupees</p>
                <a class="btn">Order Now</a>
            </div>
        </div>

        <div class="card">
            <img src="biriyani.webp">
            <div class="content">
                <h3>Chicken Biryani</h3>
                <p>250-Rupees</p>
                <a class="btn">Order Now</a>
            </div>
        </div>

        <div class="card">
            <img src="pizza.webp">
            <div class="content">
                <h3>Pizza</h3>
                <p>300-Rupees</p>
                <a class="btn">Order Now</a>
            </div>
        </div>

        <div class="card">
            <img src="icecream.webp">
            <div class="content">
                <h3>Ice Cream</h3>
                <p>100-Rupees</p>
                <a class="btn">Order Now</a>
            </div>
        </div>

    </div>
</section>

<footer>
    <p>2025 Delish Restaurant</p>
</footer>

</body>
</html>

services.html

<!DOCTYPE html>
<html>
<head>
    <title>Services - Delish Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Our Services</h1>
    <p>Serving you better every day</p>
</header>

<nav>
    <a href="restaurant.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="services.html">Services</a>
    <a href="contact.html">Contact</a>
</nav>

<section class="section" style="min-height: 90vh;">
    <h2>What We Offer</h2>

    <div class="card-container">

        <div class="card">
            <div class="content">
                <h3>Dine In</h3>
                <p>
                    Enjoy a comfortable dining experience with a cozy ambiance
                    and professional service.
                </p>
            </div>
        </div>

        <div class="card">
            <div class="content">
                <h3>Take Away</h3>
                <p>
                    Quick and hygienic takeaway options for customers on the go.
                </p>
            </div>
        </div>

        <div class="card">
            <div class="content">
                <h3>Home Delivery</h3>
                <p>
                    Get hot and fresh food delivered straight to your doorstep.
                </p>
            </div>
        </div>

        <div class="card">
            <div class="content">
                <h3>Online Ordering</h3>
                <p>
                    Order easily using our online platform anytime, anywhere.
                </p>
            </div>
        </div>

    </div>
</section>

<footer>
    <p>2025 Delish Restaurant</p>
</footer>

</body>
</html>

contact.html

<!DOCTYPE html>
<html>
<head>
    <title>Contact - Delish Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Contact Us</h1>
    <p>We would love to hear from you</p>
</header>

<nav>
    <a href="restaurant.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="services.html">Services</a>
    <a href="contact.html">Contact</a>
</nav>

<section class="section" style="min-height: 90vh;">
    <h2>Get in Touch</h2>

    <div class="card-container">

        <div class="card">
            <div class="content">
                <h3>Our Address</h3>
                <p>
                    Delish Restaurant<br>
                    Chennai, Tamil Nadu
                </p>
            </div>
        </div>

        <div class="card">
            <div class="content">
                <h3>Phone Number</h3>
                <p>
                    +91 98765 43210<br>
                    +91 91234 56789
                </p>
            </div>
        </div>

        <div class="card">
            <div class="content">
                <h3>Contact Email</h3>
                <p>
                    delish@restaurant.com<br>
                    support@restaurant.com
                </p>
            </div>
        </div>

        <div class="card">
            <div class="content">
                <h3>Our Working Hours</h3>
                <p>
                    Mon - Sun<br>
                    10:00 AM - 11:00 PM
                </p>
            </div>
        </div>

    </div>
</section>

<footer>
    <p>2025 Delish Restaurant</p>
</footer>

</body>
</html>
```
# OUTPUT:
<img width="1920" height="1080" alt="Screenshot (62)" src="https://github.com/user-attachments/assets/f80dac17-b9d4-4463-9d5b-d87c34ae2dbe" />
<img width="1920" height="1080" alt="Screenshot (59)" src="https://github.com/user-attachments/assets/987a58d1-e359-4b1e-be35-0add0fea1b56" />
<img width="1920" height="1080" alt="Screenshot (60)" src="https://github.com/user-attachments/assets/377ef040-9781-4457-94b8-d306574314d1" />
<img width="1920" height="1080" alt="Screenshot (58)" src="https://github.com/user-attachments/assets/77bdf46d-3950-467e-a3ac-ca95ecdcc2a6" />

# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
