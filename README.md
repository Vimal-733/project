# Project Responsive Web Design using Bootstrap
# Date:
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TOP PRODUCTS 2024</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Top Navigation Bar -->
    <div class="top-bar">
        <a class="navbar-brand" href="#">MOHAN S   </a>
        <input type="text" class="search-bar" placeholder="Comments">
        <a href="#" class="nav-item">Mobiles</a>
        <a href="#" class="nav-item">Refrigerators</a>
        <a href="#" class="nav-item">Tv</a>
        <a href="#" class="nav-item">Customer Service</a>
        <a href="#" class="nav-item blue-text">Sign up</a>
        <a href="#" class="nav-item blue-text">Log in</a>
    </div>

    <!-- Header Section -->
    <header>
        <div class="header-content">
            <h1>Explore Top-Rated Products Tailored to Your Needs.</h1>
            <p>Welcome to TopProducts, your ultimate destination for discovering the finest products across a variety of categories! </p>
            <input type="text" class="search-input" placeholder="Which Product are you looking for?">
        </div>
    </header>

    <!-- Trending Searches Section -->
    <section class="trending">
        <h2>Top Products 2024</h2>
        <div class="trending-tags">
            <span>Oneplus 12</span>
            <span>iphone16 pro</span>
            <span>Sony QLED TV</span>
            <span>Godrej Refrigerators</span>
            <span>Samsung Full HD TV</span>
            <span>Apple Watches</span>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="gallery">

        <div class="card">
            <img src="https://cdn.mos.cms.futurecdn.net/yDn3ZSXu9eSBxmXQDZ4PCF-1200-80.jpg" alt="Top Products">
            <h3>Apple iPhone 15 (128 GB) - Pink</h3>
            <p>₹65,900</p>
            <p>48MP MAIN CAMERA WITH 2X TELEPHOTO </p>
        </div>

        <div class="card">
            <img src="https://c.ndtvimg.com/2023-07/9b829qg_oneplus-nord-ce-2-lite_625x300_16_July_23.jpg?downsize=400:*" alt="Top Products">
            <h3>OnePlus Nord CE 2 Lite 5G (Blue Tide, 6GB RAM, 128GB Storage)</h3>
            <p>₹17,485</p>
            <p>Camera: 64MP Main Camera with EIS</p>
        </div>

        <div class="card">
            <img src="https://m.media-amazon.com/images/I/81V3wgQBeuL.SX679.jpg" alt="Top Products">
            <h3>Apple Watch Ultra 2 </h3>
            <p>₹1,04,900</p>
        </div>

        <div class="card">
            <img src="https://img.freepik.com/free-photo/air-conditioner-mounted-white-wall_53876-128235.jpg" alt="Top Products">
            <h3>Daikin 1.5 Ton 5 Star Inverter Split AC</h3>
            <p>₹45,490</p>
            <p>Copper, PM 2.5 Filter, 2024 Model, MTKM50U, White</p>
        </div>

        <div class="card">
            <img src="https://img.freepik.com/free-photo/television-houseplants-room-scene-generative-ai_188544-12145.jpg" alt="Top Products">
            <h3>LG 108 cm (43 inches) 4K Ultra HD Smart LED TV</h3>
            <p>₹29,990</p>
            <p>Resolution: 4K Ultra HD (3840x2160) | Refresh Rate: 60 hertz</p>
        </div>

        <div class="card">
            <img src="https://m.media-amazon.com/images/I/61-XXPIOivL.jpg" alt="Top Products">
            <h3>Lenovo ThinkPad E14 Intel Core i5 13th Gen</h3>
            <p>₹71,230</p>
        </div>

        <!-- Add more cards as needed -->
    </section>

    <!-- Footer Section -->
    <footer>
        <p>&copy;Top Products|MOHAN S|212223240094|All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
```
style.css
```
/* Reset and basic styles */
body, h1, h2, p, a, input, button {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f5f5f5;
    color: #333;
}

/* Top Bar Styling */
.top-bar {
    display: flex;
    align-items: center;
    background-color: #ffffff;
    padding: 10px 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.search-bar {
    margin-right: 15px;
    padding: 8px;
    border: 1px solid #ddd;
    border-radius: 4px;
    outline: none;
}

.nav-item {
    margin: 0 10px;
    color: #333;
    text-decoration: none;
}

.blue-text {
    color: #007bff;
    font-weight: bold;
}

.blue-text:hover {
    text-decoration: underline;
}

/* Header Section */
header {
    background-image: url('https://xmple.com/wallpaper/magenta-graph-paper-grid-yellow-2778x1284-c2-f57cde-d3ed54-l2-20-80-a-60-f-20.svg'); /* Add your header image */
    background-size: cover;
    padding: 80px 20px;
    text-align: center;
    color: #fff;
    text-overflow: initial;
}

.header-content h1 {
    font-size: 36px;
    margin-bottom: 10px;
}

.header-content p {
    font-size: 18px;
    margin-bottom: 20px;
}

.search-input {
    padding: 10px;
    width: 60%;
    max-width: 500px;
    border: none;
    border-radius: 4px;
    outline: none;
}

/* Trending Searches Section */
.trending {
    padding: 20px;
    text-align: center;
}

.trending h2 {
    font-size: 24px;
    margin-bottom: 10px;
}

.trending-tags {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.trending-tags span {
    background-color: #bce11b;
    color: #fff;
    padding: 5px 10px;
    margin: 5px;
    border-radius: 4px;
    font-size: 14px;
}

/* Gallery Section */
.gallery {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
    width: 200px;
    text-align: center;
}

.card img {
    width: auto;
    height: auto;
}

.card h3 {
    font-size: 16px;
    margin: 10px 0;
}

.card p {
    font-size: 12px;
    color: #555;
    margin-bottom: 10px;
}

/* Gallery Section */
.gallery {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
    width: 200px;
    text-align: center;
    position: relative;
}

.card img {
    width: 100%;
    height: auto;
    transition: transform 0.3s ease;
}

.card:hover img {
    transform: scale(1.2); /* Scale image to 120% on hover */
}

.card h3 {
    font-size: 16px;
    margin: 10px 0;
}

.card p {
    font-size: 12px;
    color: #555;
    margin-bottom: 10px;
}

/* Footer Section */
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 20px;
    margin-top: 20px;
}
```
style.js
```
// Search functionality
const searchBar = document.querySelector('.search-bar');

searchBar.addEventListener('keydown', function(event) {
    if (event.key === 'Enter') {
        event.preventDefault(); // Prevent default form submission
        alert(Searching for: ${searchBar.value});
    }
});
```

login.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <style>
        /* Reset and basic styles */
        body, h1, p, input, button {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #f5f5f5;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .login-container {
            background-color: #fff;
            padding: 20px 30px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px;
        }

        .login-container h1 {
            font-size: 24px;
            margin-bottom: 20px;
            color: #333;
            text-align: center;
        }

        .login-container input {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ddd;
            border-radius: 4px;
            outline: none;
        }

        .login-container button {
            width: 100%;
            padding: 10px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }

        .login-container button:hover {
            background-color: #0056b3;
        }

        .login-container .forgot-password {
            text-align: center;
            margin-top: 10px;
        }

        .login-container .forgot-password a {
            color: #007bff;
            text-decoration: none;
        }

        .login-container .forgot-password a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="login-container">
        <h1>Login</h1>
        <form>
            <input type="email" placeholder="Email" required>
            <input type="password" placeholder="Password" required>
            <button type="submit">Login</button>
        </form>
        <div class="forgot-password">
            <p><a href="#">Forgot Password?</a></p>
        </div>
    </div>
</body>
</html>
```
sign_in.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign In</title>
    <style>
   
        body, h1, p, input, button {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #f0f2f5;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .sign-in-container {
            background-color: #fff;
            padding: 30px 40px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px;
            text-align: center;
        }

        .sign-in-container h1 {
            font-size: 24px;
            margin-bottom: 20px;
            color: #333;
        }

        .sign-in-container input {
            width: 100%;
            padding: 12px;
            margin-bottom: 15px;
            border: 1px solid #ddd;
            border-radius: 4px;
            outline: none;
            font-size: 14px;
        }

        .sign-in-container button {
            width: 100%;
            padding: 12px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }

        .sign-in-container button:hover {
            background-color: #0056b3;
        }

        .sign-in-container .alternative {
            margin-top: 20px;
            font-size: 14px;
            color: #555;
        }

        .sign-in-container .alternative a {
            color: #007bff;
            text-decoration: none;
        }

        .sign-in-container .alternative a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="sign-in-container">
        <h1>Sign In</h1>
        <form>
            <input type="text" placeholder="first name" required>
            <input type="text" placeholder="last name" required>
            <input type="email" placeholder="Email Address" required>
            <input type="number" placeholder="phone number" required>
            <input type="password" placeholder="Password" required>
            <button type="submit">Sign In</button>
        </form>
        <div class="alternative">
            <p>Don't have an account? <a href="#">Sign Up</a></p>
            <p><a href="#">Forgot Password?</a></p>
        </div>
    </div>
</body>
</html>

```

# OUTPUT:

![11](https://github.com/user-attachments/assets/d5129269-f5b3-4291-a5db-fe1325686253)
![Screenshot (11)](https://github.com/user-attachments/assets/584d9fbd-1bb7-4d3e-9712-415db15f9a3f)
![Screenshot (12)](https://github.com/user-attachments/assets/63a96916-e3ce-4105-95fd-f01a2d3e05ad)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
