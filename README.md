# orbit-CSS-
The animation behind the orbit html file


/* Orbit Animation*/

@-webkit-keyframes starPulse {
     from {opacity: 1;}
    to {opacity: 0.2;}
}

@keyframes starPulse{
    from {opacity: 1;}
    to {opacity: 0.2;}
}

@-webkit-keyframes sunFire {
    from { -webkit-box-shadow: 0 0 50px #f5c91a;
    box-shadow: 0 0 50px #f5c91a
    
    }
    
    to {-webkit-box-shadow: 0 0 100px #f5c91a;
    box-shadow: 0 0 100px #f5c91a;
    }
}

@keyframes sunFire {
    from { -webkit-box-shadow: 0 0 50px #f5c91a;
    box-shadow: 0 0 50px #f5c91a;
    
    }
    
    to {-webkit-box-shadow: 0 0 100px #f5c91a;
    box-shadow: 0 0 100px #f5c91a;
    }
}

/* rotate animation */

@-webkit-keyframes spin {
    from {transform: rotate(0);}
    to {transform: rotate(360deg)}
}

@keyframes spin {
    from {transform: rotate(0);}
    to {transform: rotate(360deg)}
}


html, body{
    height: 100%;
    width: 100%;
    
}

#universe {
    background: black;
    background: -webkit-radical-gradient(#555, #000);
}

#stars{
    position: relative;
    z-index: 2;
    height: 100%;
    width: 100%;
    background: url('images/stars.png');
    
    -webkit-animation: starPulse 4s infinite alternate;
    animation: starPulse 4s infinite alternate;
}

#sun {
    position: absolute;
    top: 50%;
    left: 50%;
    z-index: 4;
    margin-top: -100px;
    margin-left: -100px;
    height: 200px;
    width: 200px;
    
    -webkit-border-radius: 100%;
    border-radius: 100%;
    
    background: orange;
    background: -webkit-radical-gradient(#f5c313, #ec7e08);
    
    -webkit-box-shadow: 0 0 50px #f5c91a;
    box-shadow: 0 0 50px #f5c91a;
    
    -webkit-animation: sunFire 4s infinite alternate;
    animation: sunFire 4s infinite alternate;
    
}

#earthOrbit {
   
    position: absolute;
    top: 50%;
    left: 50%;
    margin-top: -300px;
    margin-left: -300px;
    z-index: 4;
    height: 700px;
    width: 600px;
    
    -webkit-border-radius: 100%;
    border-radius: 100%;
    
    -webkit-animation: spin 30s linear infinite;
    animation: spin 30s linear infinite;
    
}

#earth {
    position: absolute;
    top: 50%;
    left: 0;
    
    margin-top: -40px;
    
    -webkit-animation: spin 3s linear infinite;
    animation: spin 3s linear infinite;
}

#moonOrbit{
    
    
   height: 120px;
    width: 120px;
    position: absolute;
    z-index: 4;
    top: 50%;
    left: -20px;
    margin-top: -60px;
    
    -webkit-border-radius: 100%;
    -moz-border-radius: 100%;
    border-radius: 100%;
    
    -webkit-animation: spin 4s linear infinite reverse;
    -moz-animation: spin 4s linear infinite reverse;
    -o-animation: spin 4s linear infinite reverse;
    animation: spin 4s linear infinite reverse;
}
    
    
#moon {
    height: 20px;
    width: 20px;
    
    
    background: gray;
    background: -webkit-radial-gradient(#ddd, #888);
    background: -moz-radial-gradient(#ddd, #888);
    background: radial-gradient(#ddd, #888);
    
     -webkit-border-radius: 100%;
    -moz-border-radius: 100%;
    border-radius: 100%;
    

}

