<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
    <title>Profile Card</title>
    
</head>
<body>
    <div class="profile-card">
        <div class="image">
            <img src="IMG_4044.JPG" alt="" class="profile-img">
        </div>

        <div class="text-data">
            <span class="name">Rafli Arsala Pratama</span>
            <span class="job">Web Development</span>
        </div>

        <div class="media-buttons">
            <a href="https://www.instagram.com/rafli.arsalaa/" style="background-color: #e1306c;" class="link">
                <i class='bx bxl-instagram'></i>
            </a>
            <a href="rafliarsalapratama@gmail.com" style="background-color: greenyellow;" class="link">
                <i class='bx bxl-gmail' ></i>
            </a>
            <a href="https://www.linkedin.com/in/rafli-arsala-pratama-094aa8284/" class="link">
                <i class='bx bxl-linkedin' ></i>
            </a>
            <a href="https://api.whatsapp.com/send/?phone=081211608340&text&type=phone_number&app_absent=0" style="background-color: green;" class="link">
                <i class='bx bxl-whatsapp' ></i>
            </a>
        </div>

        <div class="buttons">
            <button class="button">About me</button>
            <button class="button">Massage</button>
        </div>

        <div class="analytics">
            <div class="data">
                <i class='bx bx-heart' ></i>
                <span class="number">15k</span>
            </div>
            <div class="data">
                <i class='bx bx-message-rounded-dots' ></i>
                <span class="number">2k</span>
            </div>
            <div class="data">
                <i class='bx bx-share' ></i>
                <span class="number">3k</span>
            </div>
        </div>
    </div>
</body>
</html>

!!!CSS!!!
/* Google fonts poppins */
@import url('https://fonts.googleapis.com/css2?family=Noto+Serif:wght@100&family=Playfair+Display:ital,wght@0,400;0,500;0,600;0,700;0,800;0,900;1,400;1,500;1,600;1,700;1,800;1,900&family=Poppins:ital,wght@0,300;0,400;0,600;1,500&display=swap');

* {
    margin:  0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #f4f4f4;
}

.profile-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    max-width: 370px;
    width: 100%;
    background: #fff;
    border-radius: 24px;
    padding: 25px;
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
    position: relative;
}

.profile-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    height: 35%;
    width: 100%;
    border-radius: 24px 24px 0 0;
    background-color: #4070f4;

}

.image {
    position: relative;
    height: 150px;
    width: 150px;
    border-radius: 50%;
    background-color: #4070f4;
    padding: 3px;
    margin-bottom: 10px;
   
}

.image > .profile-img {
    height: 100%;
    width: 100%;
    object-fit: cover;
    border-radius: 50%;
    border: 3px solid #fff;
}

.profile-card > .text-data {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #333;
}

.text-data > .name {
    font-size: 22px;
    font-weight: 500;
}

.text-data > .job {
    font-size: 14px;
    font-weight: 400;
}

.profile-card > .media-buttons {
    display: flex;
    align-items: center;
    margin-top: 15px;
}

.media-buttons > .link {
    display: flex;
    justify-content: center;
    align-items: center;
    color: #fff;
    width: 34px;
    height: 34px;
    font-size: 18px;
    border-radius: 50%;
    background-color: #4070f4;
    text-decoration: none;
    margin: 0 8px;
}

.profile-card > .buttons {
    display: flex;
    align-items: center;
    margin-top: 20px;
}

.buttons > .button {
    font-size: 16px;
    font-weight: 410;
    color: #fff;
    border: none;
    border-radius: 24px;
    margin: 0 10px;
    padding: 5px;
    background-color: #4070f4;
    cursor: pointer;
    transition: all 0.3s ease;
}

.buttons > .button:hover {
    background-color: #0e4bf1;
}

.profile-card > .analytics {
    display: flex;
    align-items: center;
    margin-top: 13px;
}

.analytics > .data {
    display: flex;
    align-items: center;
    color: #333;
    border-right: 2px solid #e7e7e7;
    padding: 0 10px;
}

.data > i {
    font-size: 10px;
    margin-right: 6px;
}

.data:last-child {
    border-right: none;
}

