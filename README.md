<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>The Nook</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
    <style>
        * {
            margin: 0;
            box-sizing: border-box;
        }
        body {
            Background-color:black;
        }
        .wrapper {
            width: 1180px;
            height: 4000px;
            background-color: dimgrey;
            position: relative;
            margin: 0 auto
        }
        nav {
            width: 100%;
            height: 200px;
            background-color: black;
            background-repeat: no-repeat;
            margin-top: .05%;
            padding-top: 50px;
            text-align: center;
            position: fixed;
        }
        a:link {
            text-decoration:none;
            color:white;
        }
        a:visited {
            text-decoration: none;
            color: whitesmoke;
            color:white;
            size: 50px;
        }
        a:hover {
            text-decoration: none;
            color: mediumpurple;
            cursor: grab;
            color:rebeccapurple;

        }
        a:active {
            text-decoration: none;
            color:white;
        }
        #section-01{
            width: 1180px;
            height: 800px;
            background-size: contain;
            background-attachment:fixed;
            color: white;
            text-align: center;
            padding-top: 60px;


        }
        #section-02 {
            width: 1180px;
            height: 1700px;
            background-size: contain;
            background-color: white;
            color: black;
            position: relative;
            padding-top: 450px;
        }
        #section-03 {
            width: 1100px;
            height: 1800px;
            background-color: white;
            color: black;
            text-align: center;
            padding-top: 490px;
        }
        #section-04 {
            width: 1180px;
            height: 3900px;
            position: absolute;
            margin-bottom: 60px;
            background-color: white;
            color: black;
            text-align: center;
            padding-top: 290px;
        }
        #section-05 {
            width: 1180px;
            height: 800px;
            background-color: black;
            color: black;
            text-align: center;
        }
        #section-06 {
            width: 1180px;
            height: 800px;
            background-color: white;
            color: black;
            text-align: center;
        }
        p {
            display: inline;
            padding: 0 10px;
            font-family: "ClementePDac";
            font-size: 40px;
            font-weight: lighter;

        }
        footer {
            width: 1180px;
            height: 50px;
            background-color: black;
            font-family: "ClementePDac";
            text-align: center;
            position: fixed;
            bottom: 0;

        }

        #burger {
            width: 10px;
            height: 10px;
            margin-left: 47.5%;
            margin-top: .5%;
            position: relative;
        }


       </style>
    <link rel="shortcut icon" href="favicon.ico"/>
</head>
<body>
<div id="top"></div>
<div class="wrapper">
    <nav>
        <a href="#section-01"><p id="nav-section-01"> </p></a>
        <a href="#section-02"><p id="nav-section-02"> HOURS</p></a>
        <a href="#section-03"><p id="nav-section-03"> CONTACT</p></a>
        <a href="#section-04"><p id="nav-section-04"> MENU</p></a>
        <a href="#section-05"><p id="nav-section-05"> EVENTS</p></a>
        <a href="#section-06"><p id="nav-section-06"> PHOTOS</p></a>
        <div id="burger"><img src="burger.png" width=110px height=90px></img></div>



        <footer><a href="#top">Back To Top</a></footer>
    </nav>

<div id="section-01"><img src="homepage.png" width=1180px height=800px id="bg" alt=""></div>
<div id="section-02"><img src="hours.png" width=1180px height=1700px></div>
<div id="section-03"><img src="contact.png" width=1100px height=1800px></div>
<div id="section-04"><img src="menu.pdf" width=1180px height=3900px></div>
<div id="section-05"></div>
<div id="section-06"></div>

</div><!--End of wrapper!-->
<script>
    $(document).ready(function () {
        // Add smooth scrolling to all links
        $("a").on('click', function (event) {

            // Make sure this.hash has a value before overriding default behavior
            if (this.hash !== "") {
                // Prevent default anchor click behavior
                event.preventDefault();

                // Store hash
                var hash = this.hash;

                // Using jQuery's animate() method to add smooth page scroll
                // The optional number (800) specifies the number of milliseconds it takes to scroll to the specified area
                $('html, body').animate({
                    scrollTop: $(hash).offset().top
                }, 800, function () {

                    // Add hash (#) to URL when done scrolling (default click behavior)
                    window.location.hash = hash;
                });
            } // End if
        });
    });
</script>
</body>
</html>
