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
```
HTML and BOOTSTRAP


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: 'Pacifico', cursive;
            margin: 0;
            padding: 0;
            background-image: url("1011.jpeg"); /* Add your image URL here */
            background-size: cover; /* Ensure the image covers the entire background */
            background-position: center; /* Position the image in the center */
            background-repeat: no-repeat; /* Prevent the image from repeating */
            color: #2c3e50; /* Dark, contrasting text */
        }
        .gallery-item {
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease;
        }
        .gallery-item:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        .gallery-img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        body {
            background-image: url('1010.jpeg'); /* Replace with the path to your image */
            background-size: cover; /* Makes sure the image covers the entire screen */
            background-position: center center; /* Centers the image */
            background-repeat: no-repeat; /* Prevents repeating the image */
            margin: 0;
            height: 100vh; /* Ensures the body takes up the full viewport height */
        }
    </style>
    <!-- Google Font for Pacifico -->
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <a class="navbar-brand" href="#">Dribbble</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item"><a class="nav-link" href="#">Shots</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Designers</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Teams</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Community</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Jobs</a></li>
                <li class="nav-item"><a class="btn btn-primary" href="#">Sign Up</a></li>
            </ul>
        </div>
    </nav>

    <!-- Main Content Section -->
    <div class="container mt-4">
        <div class="text-center mb-4 header-section">
            <h4>FaRz </h4>
            <h3>"Bringing You the Best of Fashion, Tech, and More!"</h3>

            <p class="lead">"Find What You Love!"</p>
        </div>

        <!-- Gallery Section -->
        <div class="row gallery-section">
            <!-- Gallery Items (8 items in total) -->
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p1.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">AESTHETIC HOODIES</p>
                        <small class="text-muted">H&M</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p2.jpeg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">COMBOS</p>
                        <small class="text-muted">4 IN 1</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p3.jpeg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">SHOES</p>
                        <small class="text-muted">PUMA</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p4.jpeg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">ACCESSORIES</p>
                        <small class="text-muted">ARMANI</small>
                    </div>
                </div>
            </div>
            <!-- Additional Gallery Items -->
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p5.jpeg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">HOODIES</p>
                        <small class="text-muted">H&M</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p6.jpeg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">CROCS</p>
                        <small class="text-muted"></small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p7.jpeg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">KURTI</p>
                        <small class="text-muted">BOYS</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p8.jpeg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">WATCHES</p>
                        <small class="text-muted">ROLEX</small>
                    </div>
                    
                            
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-dark text-white text-center py-3">
        <p>© Dribbble. All rights reserved.</p>
        <p>Designed by Pharsheen Rahuman.M</p>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.bundle.min.js"></script>
</body>
</html>

# OUTPUT:
# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
