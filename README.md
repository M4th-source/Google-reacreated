<!DOCTYPE html>
<html>
   <head>
   	  <meta charset="utf-8" />
   	  <meta name="viewport" content="width=device-width, initial-scale=1.0">
   	  <link rel="stylesheet" href="style.css" />
      <title>Google</title>
      <style>
      	<pjustify-self: center>
      </style>
   </head>

   <body>
      	<div id="header">
      		<a href="https://mail.google.com" id="gmail">Gmail</a>
      		<a href="" id="images">Images</a>
      		<a href="https://www.google.fr/intl/en/about/products?tab=wh" id="menu"><img src="menu.png" height=30px width=30px></a>
      		<a href="https://www.google.fr/imghp?hl=en&tab=wi&authuser=0&ogbl" id="signin">Sign in</a>
      	</div>
      	<div id="navbar">
      		<p><img clas="logo" src="logo.png"</p>
      		<input type="text" id="search">
      		<button id="google-search-btn">Google Search</button>
      		<button id="random-search-btn">I'm Feeling Lucky</button>
      	</div>
      	<div id="footer">
      		<p>France</p>
      		<fr>
      		<a href="https://www.google.com/intl/en_fr/ads/?subid=ww-ww-et-g-awa-a-g_hpafoot1_1!o2&utm_source=google.com&utm_medium=referral&utm_campaign=google_hpafooter&fg=1" id="advertising">Advertising</a>
      		<a href="https://www.google.com/services/?subid=ww-ww-et-g-awa-a-g_hpbfoot1_1!o2&utm_source=google.com&utm_medium=referral&utm_campaign=google_hpbfooter&fg=1" id="business">Business</a>
      		<a href="https://about.google/?utm_source=google-FR&utm_medium=referral&utm_campaign=hp-footer&fg=1" id="about">About</a>
      		<a href="https://www.google.com/preferences?hl=en" id="howsearchworks">How Search works</a>
      		<a href="" id="consumerinformation">Consumer Information</a>
      		<a href="https://support.google.com/websearch?p=fr_consumer_info&hl=en-FR&fg=1" id="privacy">Privacy</a>
      		<a href="https://policies.google.com/terms?hl=en-FR&fg=1" id="terms">Terms</a>
      		<a href="https://www.google.com/preferences?hl=en" id="settings">Settings</a>
      	</div>
   </body>
</html>

html {
    height: 100%;
    width: 100%;
}
/*Header Section*/
#header {
    display: grid;
    grid-template-columns: 100px 50px 50px 50px 50px;
    grid-template-rows: 50px;
    grid-template-areas: 
    " . gmail image menu sign-in";
    margin: 0 20px 0 10px;
}

a, p {
    text-decoration: none;
    color: rgba(0,0,0,0.87);
    font-size: 13px;
    font-family: Arial, Helvetica, sans-serif;
}
a:hover {
    text-decoration: underline;
}
#gmail {
    grid-area: gmail;
    justify-self: center;
    align-self: center;
}
#images {
    grid-area: image;
    justify-self: center;
    align-self: center;
    margin-right: 10px;
}
#menu {
    grid-area: menu;
    justify-self: center;
    align-self: center;
    margin-right: 20px;
}
#signin {
    grid-area: sign in;
    justify-self: center;
    align-self: center;
    background-color: #4683ea;
    height: 30px;
    width: 65px;
    line-height: 30px;
    text-align: centeR;
    color: white;
    font-weight: bold;
    border: 1px solid #4285f4;
}

/*Navbar Section*/
#navbar {
    min-height: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 250px 70px 70px 250px;
    grid-template-areas: 
    ". logo ."
    ". search ."
    ". flexbox ."
    ". google-text .";
}

#logo {
    grid-area: logo;
    justify-self: center;
    align-self: end;
}
#search {
    grid-area: search;
    height: 30px;
    width: 80%;
    align-self: center;
    justify-self: center;
    border: 1px solid rgba(0, 0, 0, 0.151);
    border-radius: 30px;
}

#search:focus {
    box-shadow: 1px 1px 5px grey;
}
#search:hover {
    box-shadow: 1px 1px 5px grey;
}

#flexbox {
    display: flexbox;
    grid-area: flexbox;
    justify-self: center;
    align-self: center;
}
#google-search-btn {
    border: none;
    font-size: 15px;
    color: #5F6368;
    margin-right: 25px;
    padding: 7px 15px 7px 15px;
    border-radius: 3px;
}
#random-search-btn {
    border: none;
    font-size: 15px;
    color: #5F6368;
    padding: 7px 15px 7px 15px;
    border-radius: 3px;
}
#google-search-btn:hover {
    border: 1px solid rgba(0, 0, 0, 0.226);
}
#random-search-btn:hover {
    border: 1px solid rgba(0, 0, 0, 0.226);
}

#google-text {
    grid-area: google-text;
    justify-self: center;
}

/*Footer Section*/
#footer {
    position: absolute;
    bottom: 0;
    display: grid;
    grid-template-columns: 80px 80px 60px 120px 1260px 70px 70px 70px 70px;
    grid-template-rows: 50px;
    grid-template-areas: 
    "advertising business about howsearchworks . consumerinformation privacy terms settings";
}

#advertising {
    grid-area: advertising;
    justify-self: center;
    align-self: center;
}
#business {
    grid-area: business;
    justify-self: center;
    align-self: center;
}
#about {
    grid-area: about;
    justify-self: center;
    align-self: center;
}
#howsearchworks {
    grid-area: hsw;
    justify-self: center;
    align-self: center;
}
#privacy {
    grid-area: privacy;
    justify-self: center;
    align-self: center;
}
#terms {
    grid-area: terms;
    justify-self: center;
    align-self: center;
}
#settings {
    grid-area: settings;
    justify-self: center;
    align-self: center;
}
