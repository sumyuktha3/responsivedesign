# Design of Responsive Website
## AIM:
To design a responsive website with two break points.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 7:
Create a database model and migrate the database.
### Step 8:
Retrieve data from database and display it in a dynamic webpage.
### Step 9:
Publish the website in the given URL.

## PROGRAM:

## responsivebase.html

{% load static %}
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>ANODE Private Limited</title>
  </head>
  <body>
    <div class="jumbotron">
        <div class="container text-center">
            <h1 class="display-3">ANODE Private Limited</h1>
            <p class="lead">We manufacture high qualilty electronic products</p>
        </div>
    </div>
    <div class="container">
        <div class="row text-center">
            <div class="col-12 col-md-3"><a href="/responsivehome">Home</a></div>
            <div class="col-12 col-md-3"><a href="/responsiveproduct">Product</a></div>
            <div class="col-12 col-md-3"><a href="/responsivepeople">People</a></div>
            <div class="col-12 col-md-3"><a href="/responsivecontactus">Contact us</a></div>
        </div>
    </div>
    <div class="container">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="container">
        <div class="row align-items-end">
            <div class="col text-center">
                Copyright © 2021 ANODE Private Limited, Developed by SUMYUKTHA
            </div>
        </div>
    </div>
    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
  </body>
</html>

## responsivehome.html

{% extends "design/responsivebase.html" %}

{% block content %}
<div class="card" style=>
  <img class="card-img-top" src="/static/img/office.jpg" alt="Card image cap" height="300">
  <div class="card-body">
    <h5 class="card-title">About Us</h5>
    <p class="card-text">ANODE Private Limited, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> </p>
  </div>
</div>
{% endblock  %}

## responsiveproduct.html

{% extends "design/responsivebase.html" %}

{% block content %}
<div class="row text-center">
    <div class="col-12">
        <p class="lead">Our Premium Products</p>
    </div>
  
</div>
<div class="row text-center">
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/earphone.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b> EARPHONE</b></h5>
        <p class="card-text">(Ultra Bass and Dolby Sound)<br>Price: Rs.999.00</p>
        <a href="https://www.amazon.in/Crucial-4gb-ddr4-2666-Desktop/dp/B07GMRJTS9/ref=sr_1_5?dchild=1&keywords=ram&qid=1610077354&s=computers&sr=1-5" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/headset.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>HEADSET</b></h5>
        <p class="card-text">(Wireless and Foldable)<br> Price: Rs.3,099.00</p>
        <a href="https://www.amazon.in/HyperX-3200MHz-Desktop-Memory-HX432C16FB3/dp/B07WJJ9CNG/ref=sr_1_3?dchild=1&keywords=ram&qid=1610077354&s=computers&sr=1-3" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/card.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>MEMORY CARD</b></h5>
        <p class="card-text">(128GB)<br>Price: Rs.349.00</p>
        <a href="https://www.amazon.in/XPG-3200MHz-PC4-25600-CL16-20-20-AX4U320038G16A-DW60/dp/B0828CSTWC/ref=sr_1_2_sspa?dchild=1&keywords=ram&qid=1610094328&s=computers&sr=1-2" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/jbl.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>SPEAKER</b></h5>
        <p class="card-text">(Wireless, Bluetooth)<br>Price: Rs.5,000.00</p>
        <a href="https://www.amazon.in/Seagate-BarraCuda-ST1000DM010-Desktop-Latest/dp/B01LNJBA2I/ref=sr_1_2?dchild=1&keywords=hdd&qid=1610088209&s=computers&sr=1-2" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/keyboard.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>KEYBOARD</b></h5>
        <p class="card-text"> (Wireless and Attachable)<br>Price: Rs.1239.00</p>
        <a href="https://www.amazon.in/Western-Digital-WD10EZEX-Internal-Desktop/dp/B0088PUEPK/ref=sr_1_1?dchild=1&keywords=Western+Digital+Blue+1TB&psr=EY17&qid=1610099690&s=todays-deals&sr=1-1" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/modem.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>MODEM</b></h5>
        <p class="card-text">(4G LTE)<br>Price: Rs.6,999.00</p>
        <a href="https://www.amazon.in/Western-Digital-Internal-Drive-WD2005FBYZ/dp/B01IY9UTMM/ref=sr_1_1?crid=1FMIGIV7SISBB&dchild=1&keywords=western+digital+hard+disk+gold&qid=1610100444&s=computers&sprefix=wes%2Ccomputers%2C369&sr=1-1" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/mouse.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>MOUSE</b></h5>
        <p class="card-text">(Wireless)<br>Price: Rs.1,300.00</p>
        <a href="https://www.amazon.in/Western-Digital-WDS240G2G0A-240GB-Internal/dp/B076Y374ZH/ref=sr_1_1?dchild=1&keywords=sdd&qid=1610100140&s=computers&sr=1-1" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/pen.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>PENDRIVE</b></h5>
        <p class="card-text"> (256GB)<br>Price: Rs.1,500.00</p>
        <a href="https://www.amazon.in/Crucial-BX500-240GB-2-5-inch-CT240BX500SSD1/dp/B07G3YNLJB/ref=sr_1_2?dchild=1&keywords=sdd&qid=1610100913&s=computers&sr=1-2" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/router.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>ROUTER</b></h5>
        <p class="card-text"> (2.5 Inch SATA 6Gb/s)<br>Price: Rs.5,099.00</p>
        <a href="https://www.amazon.in/Seagate-Barracuda-240GB-Internal-Solid/dp/B08FJB98F1/ref=pd_sbs_147_3/259-4979351-0376003?_encoding=UTF8&pd_rd_i=B08FJB98F1&pd_rd_r=b0bac50d-3" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/temper.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>TEMPER GLASS</b></h5>
        <p class="card-text"> (Screen Protector Guard)<br>Price: Rs.499.00</p>
        <a href="https://www.amazon.in/TP-LINK-TD-W8961N-300Mbps-Antenna-Wireless/dp/B00RK5VU5M/ref=sr_1_2_sspa?crid=11RANSQBZB0TM&dchild=1&keywords=wifi+modem&qid=1610102045&s" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/nikon.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>NIKON CAMERA</b></h5>
        <p class="card-text"> (D5600 Digital Camera<br>Price: Rs.50,199.00</p>
        <a href="https://www.amazon.in/TP-Link-TL-WR902AC-Wireless-Travel-Router/dp/B01N5RCZQH/ref=sr_1_15_sspa?crid=11RANSQBZB0TM&dchild=1&keywords=wifi+modem&qid=1610102045&s" class="btn btn-primary">Buy now</a>
    </div>
    </div>
    <div class="card col-12 col-md-6 col-lg-3">
    <img class="card-img-top" src="/static/img/printer.jpg" alt="Card image cap">
    <div class="card-body">
        <h5 class="card-title"><b>PRINTER</b></h5>
        <p class="card-text"> (Canon Wireless)<br>Price: Rs.5099.00</p>
        <a href="https://www.amazon.in/dp/B07Z5NZ9CQ/ref=sspa_dk_detail_7?psc=1&pd_rd_i=B07Z5NZ9CQ&pd_rd_w=s4RPI&pf_rd_p=1801b34c-8af9-42b5-8961-11f124edc99b&pd_rd" class="btn btn-primary">Buy now</a>
    </div>
    </div>
</div>
{% endblock  %}
```

## responsivepeople.html

<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Responsive People Design</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container text-center">
            <h1 class="display-3">ANODE Private Limited</h1>
            <h5 class="display-6">crew people</h5>
        </div>
    </div>
    <div class="row text-center">
        <div class="col-12">
            <h5 class="display-6">Our Crew People</h5>
        </div>
    </div>
    <div class="row text-center">
        <div class="card col-12 col-md-6 col-lg-3">
            <img class="card-img-top" src="/static/img/steve.jpg" alt="card image cap">
            <div class="card-body">
                <h5 class="card-title">STEVE</h5>
                <p class="card-text">President of a company</p>
                <a href="https://en.wikipedia.org/wiki/steve" class="btn btn-primary">More Details</a>
            </div>
        </div>
        <div class="card col-12 col-md-6 col-lg-3">
            <img class="card-img-top" src="/static/img/Rani.jpg" alt="card image cap">
            <div class="card-body">
                <h5 class="card-title">RANI</h5>
                <p class="card-text">Cheif Executive Officer of a company</p>
                <a href="https://en.wikipedia.org/wiki/Rani" class="btn btn-primary">More Details</a>
            </div>
        </div>
        <div class="card col-12 col-md-6 col-lg-3">
            <img class="card-img-top" src="/static/img/raina.jpg" alt="card image cap">
            <div class="card-body">
                <h5 class="card-title">SURESH</h5>
                <p class="card-text">Cheif Operating Officer of a company</p>
                <a href="https://en.wikipedia.org/wiki/Suresh_Raina" class="btn btn-primary">More Details</a>
            </div>
        </div>
        <div class="card col-12 col-md-6 col-lg-3">
            <img class="card-img-top" src="/static/img/sudha.jpg" alt="card image cap">
            <div class="card-body">
                <h5 class="card-title">SUDHA</h5>
                <p class="card-text">Cheif Financial Officer of a company</p>
                <a href="https://en.wikipedia.org/wiki/Sudha" class="btn btn-primary">More Details</a>
            </div>
        </div>
        <div class="card col-12 col-md-6 col-lg-3">
            <img class="card-img-top" src="/static/img/ram.jpg" alt="card image cap">
            <div class="card-body">
                <h5 class="card-title">RAM</h5>
                <p class="card-text">Cheif Legal Officer of a company</p>
                <a href="https://www.ibm.com/blogs/client-voices/author/ram/" class="btn btn-primary">More Details</a>
            </div>
        </div>
        <div class="card col-12 col-md-6 col-lg-3">
            <img class="card-img-top" src="/static/img/jaanu.jpg" alt="card image cap">
            <div class="card-body">
                <h5 class="card-title">JAANU</h5>
                <p class="card-text">Cheif Marketing Officerof a company</p>
                <a href="https://en.wikipedia.org/wiki/jaanu" class="btn btn-primary">More Details</a>
            </div>
        </div>
    </div>
    <div class="row">
        <div class="col-12">
            <p>Copyright © 2021 ANODE Private Limited, Developed by SUMYUKTHA.</p>
        </div>
    </div>
   


    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>


## responsivecontactus.html

{% extends "design/responsivebase.html" %}

{% block content %}
<div class="card" style="width: 150">
  <img class="card-img-top" src="/static/img/contact1.jpg" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title"><div class="col text-center">Contact Us</div></h5>
    <p class="card-text">
        <hr>
        <div class="col text-center">
        <h4 class="lead">Email: anodepvt@gmail.com</h4></br>
        <h4 class="lead">Phone: +1-1594227</h4></br>
        <h4 class="lead">Address: © ANODE Private Limited,Mountain View, California, United-States</h4>
        </div>
        <hr>
    </p>
  </div>
</div>
{% endblock  %}
```

## OUTPUT:
![output](./static/img/a1.JPG)
![output](./static/img/a2.JPG)
![output](./static/img/a3.JPG)
![output](./static/img/a4.JPG)
![output](./static/img/a5.JPG)
![output](./static/img/a6.JPG)
![output](./static/img/a7.JPG)
![output](./static/img/a8.JPG)
![output](./static/img/p1.JPG)
![output](./static/img/p2.JPG)
![output](./static/img/p3.JPG)
![output](./static/img/p4.JPG)
![output](./static/img/p5.JPG)
![output](./static/img/p6.JPG)
![output](./static/img/p7.JPG)
![output](./static/img/p8.JPG)
![output](./static/img/p9.JPG)
Phone View
![output](./static/img/s1.JPG)
![output](./static/img/s2.JPG)
![output](./static/img/s3.JPG)
![output](./static/img/s4.JPG)
![output](./static/img/s5.JPG)
![output](./static/img/s6.JPG)
![output](./static/img/s7.JPG)
![output](./static/img/s8.JPG)
![output](./static/img/s9.JPG)
![output](./static/img/s10.JPG)
![output](./static/img/s11.JPG)
![output](./static/img/s12.JPG)
![output](./static/img/s13.JPG)
![output](./static/img/s14.JPG)
![output](./static/img/s15.JPG)
Validation Report
![output](./static/img/r1.JPG)
![output](./static/img/r2.JPG)
![output](./static/img/r3.JPG)
![output](./static/img/r4.JPG)

## RESULT:
Thus, a responsive website with two break points is designed and is hosted in the URL 
http://sumyuktha.student.saveetha.in:8000/
