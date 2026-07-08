# ugas-hub.github.io
ugas hub 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>UGAS Hub</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:"Century Gothic", CenturyGothic, AppleGothic, sans-serif;
    background:#000;
    overflow:hidden;
    height:100vh;
}

/* Star Background */
.stars{
    position:fixed;
    inset:0;
    background-image:
        radial-gradient(2px 2px at 20px 30px,#fff,transparent),
        radial-gradient(1.5px 1.5px at 80px 150px,#fff,transparent),
        radial-gradient(2px 2px at 170px 70px,#fff,transparent),
        radial-gradient(1.5px 1.5px at 250px 220px,#fff,transparent),
        radial-gradient(2px 2px at 340px 120px,#fff,transparent),
        radial-gradient(1.5px 1.5px at 430px 260px,#fff,transparent),
        radial-gradient(2px 2px at 520px 40px,#fff,transparent),
        radial-gradient(1.5px 1.5px at 610px 180px,#fff,transparent),
        radial-gradient(2px 2px at 700px 80px,#fff,transparent),
        radial-gradient(1.5px 1.5px at 790px 240px,#fff,transparent),
        radial-gradient(2px 2px at 880px 120px,#fff,transparent),
        radial-gradient(1.5px 1.5px at 970px 60px,#fff,transparent),
        radial-gradient(2px 2px at 1060px 220px,#fff,transparent),
        radial-gradient(1.5px 1.5px at 1150px 100px,#fff,transparent);
    background-size:250px 250px;
    animation:twinkle 5s infinite alternate;
}

@keyframes twinkle{
    from{opacity:.7;}
    to{opacity:1;}
}

/* Shooting Stars */
.shooting-star{
    position:absolute;
    width:180px;
    height:2px;
    background:linear-gradient(to right,#fff,transparent);
    border-radius:50%;
    transform:rotate(-35deg);
    animation:shoot linear infinite;
}

.shooting-star::before{
    content:"";
    position:absolute;
    width:8px;
    height:8px;
    background:#fff;
    border-radius:50%;
    left:-4px;
    top:-3px;
    box-shadow:0 0 12px white;
}

.s1{top:8%;left:-20%;animation-duration:5s;animation-delay:0s;}
.s2{top:30%;left:-35%;animation-duration:7s;animation-delay:2s;}
.s3{top:55%;left:-25%;animation-duration:6s;animation-delay:4s;}
.s4{top:75%;left:-30%;animation-duration:8s;animation-delay:1s;}

@keyframes shoot{
    from{
        transform:translateX(0) translateY(0) rotate(-35deg);
        opacity:1;
    }
    to{
        transform:translateX(1800px) translateY(600px) rotate(-35deg);
        opacity:0;
    }
}

/* Main Content */
.container{
    position:relative;
    z-index:5;
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
}

h1{
    color:#003b8e;
    font-size:72px;
    letter-spacing:4px;
    margin-bottom:40px;
    text-shadow:0 0 18px rgba(0,59,142,.7);
}

.buttons{
    display:flex;
    gap:20px;
    flex-wrap:wrap;
    justify-content:center;
}

.buttons a{
    text-decoration:none;
}

button{
    font-family:"Century Gothic", CenturyGothic, AppleGothic, sans-serif;
    font-size:20px;
    padding:15px 35px;
    border-radius:40px;
    border:2px solid #003b8e;
    background:rgba(255,255,255,.08);
    color:#003b8e;
    cursor:pointer;
    transition:.25s;
}

button:hover{
    background:#003b8e;
    color:white;
    transform:translateY(-5px) scale(1.05);
    box-shadow:0 0 20px rgba(0,59,142,.8);
}
</style>
</head>

<body>

<div class="stars"></div>

<div class="shooting-star s1"></div>
<div class="shooting-star s2"></div>
<div class="shooting-star s3"></div>
<div class="shooting-star s4"></div>

<div class="container">

    <h1>UGAS Hub</h1>

    <div class="buttons">

        <a href="https://sites.google.com/aacps.org/ugas/games" target="_blank" rel="noopener noreferrer">
            <button>Games</button>
        </a>

        <a href="https://sites.google.com/aacps.org/ugas/sites" target="_blank" rel="noopener noreferrer">
            <button>Sites</button>
        </a>

        <a href="https://sites.google.com/aacps.org/ugas/movies" target="_blank" rel="noopener noreferrer">
            <button>Movies</button>
        </a>

        <a href="https://sites.google.com/aacps.org/ugas/partners" target="_blank" rel="noopener noreferrer">
            <button>Partners</button>

        

</a>
 <a href="https://sites.google.com/aacps.org/ugas/chat" class="back" target="_blank"> <button> Chat </button>

    </div>

</div>

</body>
</html>

