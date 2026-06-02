# Ex09 Event Registration Web Application
## Date:02-06-2026

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Infinity Arena 2026</title>

<link rel="stylesheet" href="style.css">
</head>

<body>

<div class="container">

    <h1 class="title">INFINITY ARENA 2026</h1>

    <p class="subtitle">
        Technical • Sports • Gaming Festival
    </p>

    <div class="events-section">

        <div class="card">
            <h2>💻 Technical Events</h2>
            <ul>
                <li>Coding Challenge</li>
                <li>Web Design Contest</li>
                <li>Hackathon</li>
                <li>Technical Quiz</li>
            </ul>
        </div>

        <div class="card">
            <h2>⚽ Sports Events</h2>
            <ul>
                <li>Cricket</li>
                <li>Football</li>
                <li>Volleyball</li>
                <li>Chess</li>
            </ul>
        </div>

        <div class="card">
            <h2>🎮 Gaming Events</h2>
            <ul>
                <li>BGMI</li>
                <li>Valorant</li>
                <li>Free Fire MAX</li>
                <li>FIFA</li>
            </ul>
        </div>

    </div>

    <a href="registration.html" class="register-btn">
        REGISTER NOW
    </a>

</div>

</body>
</html>
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Infinity Arena 2026 - Registration</title>

    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&display=swap" rel="stylesheet">

    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="container">

    <div class="form-card">

        <h1>EVENT REGISTRATION</h1>

        <form action="contact.html">

            <input type="text" placeholder="Full Name" required>

            <input type="text" placeholder="Register Number" required>

            <input type="text" placeholder="Department" required>

            <input type="number" placeholder="Age" required>

            <input type="tel" placeholder="Mobile Number" required>

            <input type="email" placeholder="Email ID" required>

            <select required>
                <option value="">Select Event</option>

                <option>Coding Challenge</option>
                <option>Web Design Contest</option>
                <option>Hackathon</option>
                <option>Technical Quiz</option>

                <option>Cricket</option>
                <option>Football</option>
                <option>Volleyball</option>
                <option>Chess</option>

                <option>BGMI</option>
                <option>Valorant</option>
                <option>Free Fire MAX</option>
                <option>FIFA</option>
            </select>

            <button type="submit">
                REGISTER NOW
            </button>

        </form>

    </div>

</div>

</body>
</html>
```
```css
/* =========================
   RESET
========================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

/* =========================
   BODY
========================= */

body{
    min-height:100vh;

    background:
    linear-gradient(
        rgba(0,0,0,0.75),
        rgba(0,0,0,0.75)
    ),
    url("images/background.jpg");

    background-size:cover;
    background-position:center;
    background-repeat:no-repeat;
    background-attachment:fixed;

    font-family:'Cinzel', serif;

    display:flex;
    justify-content:center;
    align-items:center;

    overflow-x:hidden;
}

/* =========================
   CONTAINER
========================= */

.container{
    width:95%;
    max-width:1200px;

    text-align:center;

    animation:fadeIn 1.2s ease;
}

/* =========================
   TITLE
========================= */

.title,
.college h1{
    color:#FFD700;

    font-size:60px;
    font-weight:700;

    text-shadow:
        0 0 10px gold,
        0 0 20px gold,
        0 0 40px gold;

    animation:glow 2s infinite alternate;
}

.subtitle{
    color:white;
    font-size:20px;
    margin-top:10px;
    margin-bottom:40px;
}

/* =========================
   EVENT CARDS
========================= */

.events-section{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:25px;
}

.card{
    width:300px;

    background:rgba(255,255,255,0.08);

    backdrop-filter:blur(12px);

    border:1px solid rgba(255,215,0,0.5);

    border-radius:20px;

    padding:25px;

    color:white;

    transition:0.4s;

    animation:float 4s ease-in-out infinite;
}

.card:hover{
    transform:translateY(-10px);

    box-shadow:
        0 0 25px gold,
        0 0 50px rgba(255,215,0,0.5);
}

.card h2{
    color:#FFD700;
    margin-bottom:20px;
}

.card ul{
    list-style:none;
}

.card li{
    margin:12px 0;
    font-size:16px;
}

/* =========================
   FORM CARD
========================= */

.form-card{
    width:100%;
    max-width:450px;

    margin:auto;

    background:rgba(255,255,255,0.08);

    backdrop-filter:blur(12px);

    border:1px solid rgba(255,215,0,0.5);

    border-radius:20px;

    padding:30px;

    box-shadow:
        0 0 20px rgba(255,215,0,0.2);
}

.form-card h1{
    color:#FFD700;
    margin-bottom:25px;
}

.form-card input,
.form-card select{
    width:100%;

    padding:14px;

    margin-bottom:15px;

    border:1px solid rgba(255,215,0,0.5);

    border-radius:10px;

    background:rgba(255,255,255,0.08);

    color:white;

    font-size:15px;
}

.form-card input::placeholder{
    color:#ddd;
}

.form-card select option{
    color:black;
}

.form-card input:focus,
.form-card select:focus{
    outline:none;

    border-color:gold;

    box-shadow:0 0 10px gold;
}

/* =========================
   THANK YOU CARD
========================= */

.thankyou-card{
    max-width:500px;

    background:rgba(255,255,255,0.08);

    backdrop-filter:blur(12px);

    border:1px solid rgba(255,215,0,0.5);

    border-radius:20px;

    padding:30px;

    color:white;

    box-shadow:
        0 0 20px rgba(255,215,0,0.2);
}

.thankyou-card h1{
    color:#FFD700;
    margin-bottom:20px;
}

.contact-section{
    margin-top:25px;
    text-align:left;
}

.contact-section h2{
    color:#FFD700;
    margin-bottom:10px;
}

.contact-section p{
    margin-bottom:15px;
    line-height:1.6;
}

/* =========================
   BUTTONS
========================= */

.login-btn,
.register-btn,
.gold-btn{

    display:inline-block;

    text-decoration:none;

    padding:15px 35px;

    border:none;

    border-radius:50px;

    background:linear-gradient(
        135deg,
        #FFD700,
        #caa400
    );

    color:black;

    font-weight:bold;

    cursor:pointer;

    transition:0.4s;

    box-shadow:
        0 0 15px rgba(255,215,0,0.5);
}

.login-btn:hover,
.register-btn:hover,
.gold-btn:hover{

    transform:scale(1.08);

    box-shadow:
        0 0 20px gold,
        0 0 40px gold,
        0 0 60px gold;
}

.btn-area{
    margin-top:25px;
}

/* =========================
   ANIMATIONS
========================= */

@keyframes glow{

    from{
        text-shadow:
            0 0 10px gold,
            0 0 20px gold;
    }

    to{
        text-shadow:
            0 0 20px gold,
            0 0 40px gold,
            0 0 80px gold;
    }
}

@keyframes float{

    0%,100%{
        transform:translateY(0);
    }

    50%{
        transform:translateY(-10px);
    }
}

@keyframes fadeIn{

    from{
        opacity:0;
        transform:translateY(30px);
    }

    to{
        opacity:1;
        transform:translateY(0);
    }
}

/* =========================
   RESPONSIVE
========================= */

@media(max-width:768px){

    .title,
    .college h1{
        font-size:40px;
    }

    .events-section{
        flex-direction:column;
        align-items:center;
    }

    .card{
        width:90%;
    }
}
<h1>THANK YOU!</h1>

<p>
Your registration for Infinity Arena 2026
has been submitted successfully.
</p>

<a href="index.html" class="gold-btn">
    Back to Home
</a>
```

## OUTPUT:
<img width="1319" height="989" alt="{8F31BC6F-7082-4E7A-94E3-161FEDD60069}" src="https://github.com/user-attachments/assets/10e5561b-60de-4e03-bd5d-87382344377c" />
<img width="1803" height="994" alt="{B571CCA3-AC64-404F-B9B2-5F6F529A5977}" src="https://github.com/user-attachments/assets/2b6371a6-fef4-4a0c-949a-ff87950fe1fa" />
<img width="1680" height="277" alt="{A3C6C1BE-DDC1-4FEA-8F98-6899B71EFD79}" src="https://github.com/user-attachments/assets/10d5dd68-435f-4141-85cb-cdae6863ea73" />



## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
