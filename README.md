# A<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile Card</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #ffffff;
        }
        .card {
            background: rgb(232, 232, 232);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s;
        }

        .card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 50%;
            background: black;
            border-top-left-radius: 10px;
            border-top-right-radius: 10px;
            z-index: -1;
        }
        
        .card:hover {
            transform: scale(1.05);
        }
        .profile-pic {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 3px solid blue;
            object-fit: cover;
            margin-bottom: 10px;
        }
        .name {
            font-size: 22px;
            font-weight: bold;
        }
        .designation {
            color: gray;
            margin-bottom: 10px;
        }
        .bio {
            font-size: 14px;
            margin-bottom: 15px;
            color: #555;
        }
        .social-icons a {
            display: inline-block;
            margin: 0 5px;
            text-decoration: none;
            color: #555;
            font-size: 18px;
            transition: color 0.3s;
        }
        .social-icons a:hover {
            color: #007bff;
        }
    </style>
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</head>
<body>
    <div class="card">
        <img src="abc.jpg" alt="Profile Picture" class="profile-pic">
        <div class="name">Abhishek Pharswan</div>
        <div class="designation">Web Developer</div>
        <div class="social-icons">
            <a href="#"><i class='bx bxl-facebook-circle'></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-linkedin"></i></a>
        </div>
        <div class="bio">Passionate about building interactive web experiences and user-friendly designs.</div>
       
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/js/all.min.js"></script>
</body>
</html>
