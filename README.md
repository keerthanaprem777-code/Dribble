# Project Responsive Web Design using Bootstrap
## Date:15|10|2025

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Bootstrap Page</title>

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">

    <!-- Optional: Add custom CSS for minor tweaks if needed -->
    <style>
        /* Add some vertical padding to sections */
        .content-section {
            padding-top: 5rem;
            padding-bottom: 5rem;
        }
    </style>
</head>
<body>

    <!-- 1. Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
        <div class="container">
            <a class="navbar-brand" href="#">BootstrapSite</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="#home">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#services">Services</a>
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

    <!-- 2. Hero Section (Welcome Area) -->
    <header id="home" class="bg-light py-5" style="margin-top: 56px;"> <!-- Add margin-top to offset fixed navbar -->
        <div class="container text-center py-5">
            <h1 class="display-4 fw-bold">Welcome to Our Website</h1>
            <p class="lead text-muted">A simple and elegant design using Bootstrap 5.</p>
            <a href="#services" class="btn btn-primary btn-lg mt-3">Learn More</a>
        </div>
    </header>

    <!-- 3. Content Sections -->
    <main>
        <!-- Services Section with Cards -->
        <section id="services" class="content-section">
            <div class="container">
                <div class="text-center mb-5">
                    <h2>Our Services</h2>
                    <p class="lead text-muted">Discover what we have to offer.</p>
                </div>
                <div class="row">
                    <!-- Service 1 -->
                    <div class="col-lg-4 col-md-6 mb-4">
                        <div class="card h-100">
                            <img src="https://picsum.photos/400/250?random=1" class="card-img-top" alt="Web Design">
                            <div class="card-body">
                                <h5 class="card-title">Web Design</h5>
                                <p class="card-text">We create beautiful, responsive websites that look great on all devices. Our designs are modern and user-friendly.</p>
                            </div>
                            <div class="card-footer">
                                 <a href="#" class="btn btn-outline-primary">Details</a>
                            </div>
                        </div>
                    </div>
                    <!-- Service 2 -->
                    <div class="col-lg-4 col-md-6 mb-4">
                        <div class="card h-100">
                            <img src="https://picsum.photos/400/250?random=2" class="card-img-top" alt="Digital Marketing">
                            <div class="card-body">
                                <h5 class="card-title">Digital Marketing</h5>
                                <p class="card-text">Our marketing strategies will help you reach a wider audience and grow your business online effectively.</p>
                            </div>
                            <div class="card-footer">
                                 <a href="#" class="btn btn-outline-primary">Details</a>
                            </div>
                        </div>
                    </div>
                    <!-- Service 3 -->
                    <div class="col-lg-4 col-md-6 mb-4">
                        <div class="card h-100">
                            <img src="https://picsum.photos/400/250?random=3" class="card-img-top" alt="App Development">
                            <div class="card-body">
                                <h5 class="card-title">App Development</h5>
                                <p class="card-text">From concept to launch, we build high-quality mobile applications for both iOS and Android platforms.</p>
                            </div>
                            <div class="card-footer">
                                 <a href="#" class="btn btn-outline-primary">Details</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- About Us Section -->
        <section id="about" class="content-section bg-light">
            <div class="container">
                <div class="row align-items-center">
                    <div class="col-md-6">
                        <img src="https://picsum.photos/600/400?random=4" class="img-fluid rounded" alt="About Us Image">
                    </div>
                    <div class="col-md-6">
                        <h2 class="mt-4 mt-md-0">About Us</h2>
                        <p class="lead">We are a team of passionate developers and designers dedicated to creating amazing digital experiences.</p>
                        <p>Our mission is to provide top-notch services that help our clients succeed. We believe in collaboration, innovation, and excellence in everything we do. Join us on our journey to make the web a better place.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Contact Section -->
        <section id="contact" class="content-section">
            <div class="container">
                <div class="text-center mb-5">
                    <h2>Contact Us</h2>
                    <p class="lead text-muted">Have a question? We'd love to hear from you.</p>
                </div>
                <div class="row justify-content-center">
                    <div class="col-lg-8">
                        <form>
                            <div class="mb-3">
                                <label for="name" class="form-label">Name</label>
                                <input type="text" class="form-control" id="name" placeholder="Your Name">
                            </div>
                            <div class="mb-3">
                                <label for="email" class="form-label">Email address</label>
                                <input type="email" class="form-control" id="email" placeholder="name@example.com">
                            </div>
                            <div class="mb-3">
                                <label for="message" class="form-label">Message</label>
                                <textarea class="form-control" id="message" rows="4"></textarea>
                            </div>
                            <div class="text-center">
                                <button type="submit" class="btn btn-primary">Send Message</button>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- 4. Footer -->
    <footer class="bg-dark text-white text-center py-3">
        <div class="container">
            <p class="mb-0">&copy; 2024 BootstrapSite. All Rights Reserved.</p>
        </div>
    </footer>

    <!-- Bootstrap JS Bundle (includes Popper) -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
</body>
</html>
```

## OUTPUT:
![WhatsApp Image 2025-10-15 at 22 44 49_46e026dc](https://github.com/user-attachments/assets/fbc2ad47-5019-4952-b2c2-0e953d4b2a5b)

![WhatsApp Image 2025-10-15 at 22 44 51_4a3de75a](https://github.com/user-attachments/assets/00e71c20-9006-47c4-8ad3-69c9f57eeafe)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
