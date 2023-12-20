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
