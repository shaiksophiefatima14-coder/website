# Ex.06 Restaurant Website
# Date:21/05/2026
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
HOME.HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Flimzy Fox</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#e5e5e5;
}

.container{
    width:90%;
    margin:auto;
}

.logo{
    text-align:center;
    padding:30px 0;
}

.logo h1{
    font-size:50px;
    color:#4f5d57;
    letter-spacing:5px;
}

.navbar{
    background:#333;
    border-radius:10px;
    display:flex;
    justify-content:space-around;
    padding:15px;
    margin-bottom:20px;
}

.navbar a{
    color:white;
    text-decoration:none;
    font-weight:bold;
}

.banner{
    background:url('https://images.unsplash.com/photo-1513104890138-7c749659a591') no-repeat center;
    background-size:cover;
    height:250px;
    border-radius:15px;
    padding:40px;
    color:white;
    margin-bottom:20px;
}

.banner h2{
    font-size:45px;
    margin-bottom:15px;
}

.banner p{
    width:60%;
    line-height:1.5;
}

.cards{
    display:flex;
    gap:20px;
    margin-bottom:30px;
}

.card{
    background:#eadccf;
    padding:20px;
    border-radius:15px;
    flex:1;
}

.card h3{
    margin-bottom:15px;
    font-size:28px;
}

.card img{
    width:100%;
    height:220px;
    object-fit:cover;
    margin-bottom:15px;
}

.card p{
    text-align:justify;
    line-height:1.5;
    margin-bottom:15px;
}

.footer{
    display:flex;
    justify-content:space-between;
    align-items:center;
    border-top:2px solid #777;
    padding:20px 0;
}


.footer p{
    color:#7a3e3e;
    font-size:20px;
}
</style>
</head>

<body>

<div class="container">

    <div class="logo">
        <h1>FLIMZY FOX</h1>
    </div>

    <div class="navbar">
        <a href="index.html">Home</a>
        <a href="menu.html">Menu</a>
        <a href="admin.html">Administration</a>
        <a href="contact.html">Contact Us</a>
    </div>

    <div class="banner">
        <h2>30% Off This Weekend</h2>
        <p>
            Enjoy delicious dishes with exciting weekend offers at Little Lemon Restaurant.
            Fresh ingredients, tasty meals and a wonderful dining experience await you.
        </p>
    </div>

    <div class="cards">

        <div class="card">
            <h3>Our New Menu</h3>
            <img src="https://images.unsplash.com/photo-1529042410759-befb1204b468" alt="">
            <p>
                Explore our newly added grilled dishes and chef special recipes prepared with fresh ingredients.
            </p>
            <a href="menu.html">See our new menu</a>
        </div>

        <div class="card">
            <h3>Book a Table</h3>
            <img src="https://images.unsplash.com/photo-1540189549336-e6e99c3679fe" alt="">
            <p>
                Reserve your table online and enjoy a peaceful dining experience with family and friends.
            </p>
            <a href="#">Book your table now</a>
        </div>

        <div class="card">
            <h3>Opening Hours</h3>
            <img src="https://images.unsplash.com/photo-1559339352-11d035aa65de" alt="">
            <p>
                Mon - Fri : 2pm - 10pm<br>
                Sat : 2pm - 11pm<br>
                Sun : 2pm - 9pm
            </p>
        </div>

    </div>

    <div class="footer">
        <p>Designed and Developed by Sophie Fatima</p>
        <p>Reg no 212224043002</p>
    </div>

</div>

</body>
</html>
```

MENU.HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Menu - Little Lemon</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#e5e5e5;
}

.container{
    width:90%;
    margin:auto;
}

.header{
    text-align:center;
    padding:30px;
    color:#4f5d57;
    font-size:40px;
    letter-spacing:4px;
}

.navbar{
    background:#333;
    border-radius:10px;
    display:flex;
    justify-content:space-around;
    padding:15px;
    margin-bottom:30px;
}

.navbar a{
    color:white;
    text-decoration:none;
    font-weight:bold;
}

.menu-title{
    text-align:center;
    margin-bottom:30px;
    font-size:35px;
    color:#333;
}

.menu-container{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
    margin-bottom:40px;
}

.menu-card{
    background:#eadccf;
    padding:15px;
    border-radius:15px;
    text-align:center;
}

.menu-card img{
    width:100%;
    height:220px;
    object-fit:cover;
    border-radius:10px;
    margin-bottom:15px;
}

.menu-card h3{
    margin-bottom:10px;
    color:#333;
}

.menu-card p{
    margin-bottom:10px;
    color:#555;
}

.price{
    font-size:20px;
    color:darkred;
    font-weight:bold;
}

.footer{
    border-top:2px solid gray;
    text-align:center;
    padding:20px;
    color:#7a3e3e;
}

</style>
</head>

<body>

<div class="container">

    <div class="header">
        LITTLE LEMON
    </div>

    <div class="navbar">
        <a href="index.html">Home</a>
        <a href="menu.html">Menu</a>
        <a href="admin.html">Administration</a>
        <a href="contact.html">Contact Us</a>
    </div>

    <div class="menu-title">
        Our Delicious Menu
    </div>

    <div class="menu-container">

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1513104890138-7c749659a591">
            <h3>Cheese Pizza</h3>
            <p>Hot cheesy pizza with fresh toppings.</p>
            <div class="price">₹250</div>
        </div>

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1550547660-d9450f859349">
            <h3>Burger</h3>
            <p>Juicy grilled burger with fries.</p>
            <div class="price">₹180</div>
        </div>

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1544025162-d76694265947">
            <h3>Fish</h3>
            <p>Nicely deep fried in creamy sauce.</p>
            <div class="price">₹220</div>
        </div>

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1565299624946-b28f40a0ae38">
            <h3>Chicken Pizza</h3>
            <p>Loaded chicken pizza with cheese.</p>
            <div class="price">₹240</div>
        </div>

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1604908176997-125f25cc6f3d">
            <h3>Chicken Grill</h3>
            <p>Spicy grilled chicken with salad.</p>
            <div class="price">₹350</div>
        </div>

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1546069901-ba9599a7e63c">
            <h3>Healthy Salad</h3>
            <p>Fresh vegetables and lemon dressing.</p>
            <div class="price">₹150</div>
        </div>

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1551024601-bec78aea704b">
            <h3>Donuts</h3>
            <p>with varieties of flavours.</p>
            <div class="price">₹120</div>
        </div>

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836">
            <h3>Steak</h3>
            <p>HAve different varieties.</p>
            <div class="price">₹200</div>
        </div>

        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1525755662778-989d0524087e">
            <h3>Honey chilli Potato</h3>
            <p>Sweet and tangy flavour.</p>
            <div class="price">₹100</div>
        </div>


        <div class="menu-card">
            <img src="https://images.unsplash.com/photo-1473093295043-cdd812d0e601">
            <h3>Pasta</h3>
            <p>Creamy sauce with cheese</p>
            <div class="price">₹130</div>
        </div>

    </div>

    <div class="footer">
        Designed and Developed by Sophie Fatima
    </div>

</div>

</body>
</html>
```
ADMIN.HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Administration - Little Lemon</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#e5e5e5;
}

.container{
    width:90%;
    margin:auto;
}

.header{
    text-align:center;
    padding:30px;
    color:#4f5d57;
    font-size:40px;
    letter-spacing:4px;
}

.navbar{
    background:#333;
    border-radius:10px;
    display:flex;
    justify-content:space-around;
    padding:15px;
    margin-bottom:30px;
}

.navbar a{
    color:white;
    text-decoration:none;
    font-weight:bold;
}

.title{
    text-align:center;
    font-size:35px;
    margin-bottom:30px;
    color:#333;
}

.admin-container{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
    margin-bottom:40px;
}

.admin-card{
    background:#eadccf;
    padding:20px;
    border-radius:15px;
    text-align:center;
}

.admin-card img{
    width:100%;
    height:450px;
    object-fit:cover;
    border-radius:10px;
    margin-bottom:15px;
}

.admin-card h3{
    color:#333;
    margin-bottom:10px;
}

.admin-card p{
    color:#555;
    font-size:18px;
}

.footer{
    border-top:2px solid gray;
    text-align:center;
    padding:20px;
    color:#7a3e3e;
}

</style>
</head>

<body>

<div class="container">

    <div class="header">
        FLIMZY FOX
    </div>

    <div class="navbar">
        <a href="index.html">Home</a>
        <a href="menu.html">Menu</a>
        <a href="admin.html">Administration</a>
        <a href="contact.html">Contact Us</a>
    </div>

    <div class="title">
        Administration Team
    </div>

    <div class="admin-container">

        <div class="admin-card">
            <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e">
            <h3>David Miller</h3>
            <p>Restaurant Manager</p>
        </div>

        <div class="admin-card">
            <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330">
            <h3>Emma Wilson</h3>
            <p>Head Chef</p>
        </div>

        <div class="admin-card">
            <img src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d">
            <h3>James Smith</h3>
            <p>Assistant Manager</p>
        </div>

        <div class="admin-card">
            <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2">
            <h3>Sophia Brown</h3>
            <p>Food Supervisor</p>
        </div>

        <div class="admin-card">
            <img src="https://images.unsplash.com/photo-1504257432389-52343af06ae3">
            <h3>Michael Lee</h3>
            <p>Customer Support</p>
        </div>

        <div class="admin-card">
            <img src="https://images.unsplash.com/photo-1488426862026-3ee34a7d66df">
            <h3>Olivia Taylor</h3>
            <p>Marketing Executive</p>
        </div>

    </div>

    <div class="footer">
        Designed and Developed by Sophie Fatima
    </div>

</div>

</body>
</html>
```
CONTACT.HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Contact Us - Little Lemon</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#e5e5e5;
}

.container{
    width:90%;
    margin:auto;
}

.header{
    text-align:center;
    padding:30px;
    color:#4f5d57;
    font-size:40px;
    letter-spacing:4px;
}

.navbar{
    background:#333;
    border-radius:10px;
    display:flex;
    justify-content:space-around;
    padding:15px;
    margin-bottom:40px;
}

.navbar a{
    color:white;
    text-decoration:none;
    font-weight:bold;
}

.contact-box{
    background:#eadccf;
    padding:40px;
    border-radius:15px;
    width:70%;
    margin:auto;
    margin-bottom:40px;
}

.contact-box h2{
    text-align:center;
    margin-bottom:30px;
    color:#333;
    font-size:35px;
}

.contact-box p{
    font-size:20px;
    margin-bottom:20px;
    color:#555;
    line-height:1.8;
}

.footer{
    border-top:2px solid gray;
    text-align:center;
    padding:20px;
    color:#7a3e3e;
}

</style>
</head>

<body>

<div class="container">

    <div class="header">
        FLIMZY FOX
    </div>

    <div class="navbar">
        <a href="index.html">Home</a>
        <a href="menu.html">Menu</a>
        <a href="admin.html">Administration</a>
        <a href="contact.html">Contact Us</a>
    </div>

    <div class="contact-box">

        <h2>Contact Information</h2>

        <p>
            <b>Restaurant Address:</b><br>
            FLIMZY FOX Restaurant,<br>
            25 Food Street,<br>
            Chennai, Tamil Nadu - 600001
        </p>

        <p>
            <b>Phone Number:</b><br>
            +91 98765 43210
        </p>

        <p>
            <b>Email Address:</b><br>
            flimzyfox@gmail.com
        </p>

        <p>
            <b>Working Hours:</b><br>
            Monday - Friday : 10 AM to 10 PM<br>
            Saturday - Sunday : 11 AM to 11 PM
        </p>

    </div>

    <div class="footer">
        Designed and Developed by Sophie Fatima
        Reg no: 212224043002
    </div>

</div>

</body>
</html>
```

# OUTPUT:
HOME PAGE
<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/ff393b0a-b6d8-49d8-8451-0a42f688e88f" />

MENU PAGE
<img width="1919" height="1038" alt="image" src="https://github.com/user-attachments/assets/1fcb43ac-937f-49bf-9171-24bb31f2d221" />

ADMIN PAGE
<img width="1920" height="1140" alt="Screenshot 2026-05-21 143135" src="https://github.com/user-attachments/assets/1e79ad05-a5a9-411f-9b6c-1aa85c731847" />

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/65651547-f14f-4b31-b481-dadf3eb2ea8c" />

CONTACT US
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/23d78acf-8a0a-4f5a-82ad-1832a76f0eb9" />


# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
