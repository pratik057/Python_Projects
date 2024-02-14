<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>]SCET Sarvey</title>
   
</head>
<style>
    .par {
        display: flex;
        column-gap: 30px;
        margin-top: 100px;
    }
    
    .para2 {
    
        column-gap: 30px;
        margin-top: 30px;
        position: relative;
    }
    
    @property --rotate {
        syntax: "<angle>";
        initial-value: 132deg;
        inherits: false;
    }
    
    :root {
        --card-height: 15vh;
        --card-width: calc(var(--card-height) / 1.5);
    }
    body {
        min-height: 100vh;
        background: #000000;
        display: flex;
        align-items: center;
        flex-direction: column;
        padding-top: 2rem;
        padding-bottom: 2rem;
        box-sizing: border-box;
        overflow-y: hidden;
    }
    
    .card {
        box-shadow: 0px 2px 100px 1px #43434325;
    
        background: #191c29;
        width: var(--card-width);
        height: var(--card-height);
        padding: 3px;
        position: relative;
        border-radius: 6px;
        justify-content: center;
        align-items: center;
        display: flex;
        font-size: 1.5em;
        color: rgb(88 199 250 / 0%);
        cursor: pointer;
        font-family: cursive;
    }
    
    .card2 {
        background: #191c29;
        width: 303px;
        height: var(--card-height);
        padding: 3px;
        position: relative;
        border-radius: 6px;
        justify-content: center;
        align-items: center;
        display: flex;
        font-size: 1.5em;
        color: rgb(88 199 250 / 0%);
        cursor: pointer;
        font-family: cursive;
    }
    
    .card:hover {
        color: rgb(88 199 250 / 100%);
        transition: color 1s;
    }
    
    .card2:hover {
        color: rgb(88 199 250 / 100%);
        transition: color 1s;
    }
    
    .card:hover::before,
    .card:hover::after {
        animation: none;
        opacity: 0;
    }
    
    .card::before {
        content: " ";
        width: 104%;
        height: 102%;
        border-radius: 8px;
        background-image: linear-gradient(var(--rotate), #5ddcff, #3c67e3 43%, #4e00c2);
        position: absolute;
        z-index: -1;
        top: -1%;
        left: -2%;
        animation: spin 2.5s linear infinite;
    }
    
    .card2::after {
        position: absolute;
        content: " ";
        top: calc(var(--card-height) / 6);
        left: 0;
        right: 0;
        z-index: -1;
        height: 100%;
        width: 100%;
        margin: 0 auto;
        transform: scale(0.8);
        filter: blur(calc(var(--card-height) / 6));
        background-image: linear-gradient(var(--rotate), #5ddcff, #3c67e3 43%, #4e00c2);
        opacity: 1;
        transition: opacity .5s;
        animation: spin 2.55 linera infinite;
    }
    
    @keyframes spin {
        0% {
            --rotate: 0deg;
        }
    
        100% {
            --rotate: 360deg;
        }
    }
    
    .card2:hover::before,
    .card2:hover::after {
        animation: none;
        opacity: 0;
    }
    
    .card2::before {
        content: " ";
        width: 104%;
        height: 102%;
        border-radius: 8px;
        background-image: linear-gradient(var(--rotate), #5ddcff, #3c67e3 43%, #4e00c2);
        position: absolute;
        z-index: -1;
        top: -1%;
        left: -2%;
        animation: spin 2.5s linear infinite;
    }
    
    .card2::after {
        position: absolute;
        content: " ";
        top: calc(var(--card-height) / 6);
        left: 0;
        right: 0;
        z-index: -1;
        height: 100%;
        width: 100%;
        margin: 0 auto;
        transform: scale(0.8);
        filter: blur(calc(var(--card-height) / 6));
        background-image: linear-gradient(var(--rotate), #5ddcff, #3c67e3 43%, #4e00c2);
        opacity: 1;
        transition: opacity .5s;
        animation: spin 2.55 linera infinite;
    }
    
    img {
       width: 45px;
        position: relative;
        background-repeat: no-repeat;
        background-size: cover;
        background-position-y: -3rem;
        top: 25px;
    }
    @media (min-width:360px),( max-hight:760px) {
        img {
        width: 50vw;
        height: 30vh;
        position: relative;
        background-repeat: no-repeat;
        background-size: cover;
        background-position-y: -3rem;
        margin-top: -15px;
       }
       .para2 {
    
        column-gap: 30px;
        margin-top: 30px;
        position: relative;
        
    }
    }
    
</style>

<body>
    <div class="par">
        <div class="card">
           heyy
        </div>
        <div class="card">
          you
        </div>
        <div class="card">
            yess
        </div>
    </div>
    <div class="img">
        <img src="https://w0.peakpx.com/wallpaper/683/15/HD-wallpaper-black-and-white-love-white-littel-heart-black-white.jpg"
            alt="Img">
    </div>

    <div class="para2">
        <div class="card2">
        Will you be my valentine🤭❤️🥀
        </div>
    </div>
</body>

</html>
