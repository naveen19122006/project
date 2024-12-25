# Project Responsive Web Design using Bootstrap
# Date:10-12-2024
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
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Creative Showcase</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f9fa;
        }
        .navbar {
            background-color: #212529;
        }
        .navbar-brand {
            font-weight: bold;
        }
        .hero-section {
            background-color: #343a40;
            color: white;
            padding: 50px 0;
            text-align: center;
        }
        .portfolio-grid {
            margin-top: 30px;
        }
        .portfolio-item {
            position: relative;
            overflow: hidden;
            border-radius: 8px;
        }
        .portfolio-item img {
            width: 100%;
            transition: transform 0.3s ease-in-out;
        }
        .portfolio-item:hover img {
            transform: scale(1.1);
        }
        .portfolio-item .overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.6);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.3s ease-in-out;
        }
        .portfolio-item:hover .overlay {
            opacity: 1;
        }
        footer {
            background-color: #212529;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
    </style>
</head>
<body>
  
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">CreativeHub</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link active" href="#">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#portfolio">Portfolio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#about">About</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact">Contact</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>


    <section class="hero-section">
        <div class="container">
            <h1>Welcome to CreativeHub</h1>
            <p class="lead">Showcasing creativity and talent from around the world.</p>
        </div>
    </section>

    <section id="portfolio" class="py-5">
        <div class="container">
            <h2 class="text-center mb-4">Explore Our Portfolio</h2>
            <div class="row portfolio-grid">
                <div class="col-md-4 mb-4">
                    <div class="portfolio-item">
                        <img src="d 1.webp" alt="Portfolio 1">
                        <div class="overlay">
                            <p>Project Title 1</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="portfolio-item">
                        <img src="d 2.webp" alt="Portfolio 2">
                        <div class="overlay">
                            <p>Project Title 2</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="portfolio-item">
                        <img src="d 3.webp" alt="Portfolio 3">
                        <div class="overlay">
                            <p>Project Title 3</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="portfolio-item">
                        <img src="d 4.webp" alt="Portfolio 4">
                        <div class="overlay">
                            <p>Project Title 4</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="portfolio-item">
                        <img src="d 5.webp" alt="Portfolio 5">
                        <div class="overlay">
                            <p>Project Title 5</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="portfolio-item">
                        <img src="d 6.webp  " alt="Portfolio 6">
                        <div class="overlay">
                            <p>Project Title 6</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>


    <section id="about" class="py-5 bg-light">
        <div class="container">
            <h2 class="text-center">About Us</h2>
            <p class="text-center">CreativeHub is a platform dedicated to showcasing exceptional designs and creative works. Our mission is to connect designers with audiences and help them thrive.</p>
        </div>
    </section>


    <section id="contact" class="py-5">
        <div class="container">
            <h2 class="text-center">Contact Us</h2>
            <form>
                <div class="mb-3">
                    <label for="name" class="form-label">Name</label>
                    <input type="text" class="form-control" id="name" placeholder="Your Name">
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email</label>
                    <input type="email" class="form-control" id="email" placeholder="Your Email">
                </div>
                <div class="mb-3">
                    <label for="message" class="form-label">Message</label>
                    <textarea class="form-control" id="message" rows="5" placeholder="Your Message"></textarea>
                </div>
                <button type="submit" class="btn btn-primary">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 CreativeHub. All rights reserved.</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

~~~
# OUTPUT:
![image](https://github.com/user-attachments/assets/03b05ba7-9b6c-4e4f-bcdc-160608d5a445)

![image](https://github.com/user-attachments/assets/e71c5b73-fb5f-4002-a694-d5ce66c42d48)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
