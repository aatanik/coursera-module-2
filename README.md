<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="stylee.css">
    <meta charset="utf-8">
    <meta name='viewport' content='width=device-width, initial-scale=1'>
    <title>Module 2 solution</title>
</head>
<body>
    <h1>Our Menu</h1>
    <div class='row'>
        <div class='col-lg-4 col-md-6 col-sm-12'>
            <div class='section'>
                <span id='pp1'>Chicken</span>
                <p>Tender chicken cooked with love and seasoned with a secret sauce. An ideal choice for true lovers of classic dishes.</p>
            </div>
        </div>
        <div class='col-lg-4 col-md-6 col-sm-12'>
            <div class='section'>
                <span id='pp2'>Beef</span>
                <p>Selected beef, roasted to perfect juiciness and served with exquisite seasonings. Enjoy the rich taste of our gourmet beef dishes.</p>
            </div>
        </div>
        <div class='col-lg-4 col-md-12 col-sm-12'>
            <div class='section'>
                <span id='pp3'>Sushi</span>
                <p>Exquisite rolls and sushi made from the freshest seafood and selected rice. Plunge into the world of oriental flavors and enjoy every bite of our unique sushi.</p>
            </div>
        </div>
    </div>
</body>
</html>
{
  box-sizing: border-box;
}

body {
  background-color: rgb(51, 232, 255);
}

h1 {
  font-size: 27px;
  font-family: Georgia, serif;
  text-align: center;
  color: rgb(0, 0, 0);
  margin-bottom: 30px;
}

p {
  padding: 15px 5px 0px 5px;
  font-family: 'Georgia', sans-serif;
  font-size: 16px;
  position: relative;
}

.section {
  background-color: rgb(150, 150, 150);
  border: 2px solid black;
  margin-top: 20px;
  margin-right: 20px;
  padding: 3px;
  text-align: justify;
  position: relative; /* Changed from absolute to relative */
}

span {
  font-size: 20px;
  width: 150px;
  border: 1px solid black;
  font-weight: bold;
  text-align: center;
  float: right;
  top: 0;
  right: 0;
  margin: 0;
  position: absolute;
}

#pp1 {
  background-color: rgb(250, 150, 150);
  color: rgb(0, 0, 0);
}

#pp2 {
  background-color: rgb(250, 0, 0);
  color: rgb(250, 250, 250);
}

#pp3 {
  background-color: rgb(200, 200, 100);
  color: rgb(0, 0, 0);
}

.row::after {
  content: "";
  clear: both;
  display: table;
}

/* PC view */
@media (min-width: 992px) {
  .col-lg-4 {
    width: 33.33%;
    float: left;
  }
}

/* Tablet view */
@media (min-width: 768px) and (max-width: 991px) {
  .col-md-6 {
    width: 50%;
    float: left;
  }
  .col-md-12 {
    width: 100%;
    float: left;
  }
}

/* Mobile view */
@media (max-width: 767px) {
  .col-sx-12 {
    float: left;
    width: 100%;
  }
}
