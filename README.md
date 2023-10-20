# StarBucks
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Strabucks Website Landing Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <section>
        <div class="circle"></div>
        <header>
            <a href="#"><img src="./img/logo.png" class="logo"></a>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Menu</a></li>
                <li><a href="#">Whats's New</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </header>
        <div class="content">
            <div class="textBox">
                <h2>It's not just Coffee<br>It's <span>Strabucks</span></h2>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ipsum eveniet dolorem
                     sapiente suscipit, fugiat quis voluptate soluta ex delectus nostrum autem?
                     Deleniti ducimus doloribus distinctio vitae facilis.</p>
                <a href="#">Learn More</a>
            </div>
        </div>
        <div class="imgBox">
            <img src="./img/img1.png" class="Strabucks">
        </div>
        <ul class="thumb">
            <li><img src="./img/thumb1.png" onclick="imgSlider('./img/img1.png')"></li>
            <li><img src="./img/thumb2.png" onclick="imgSlider('./img/img2.png')"></li>
            <li><img src="./img/thumb3.png" onclick="imgSlider('./img/img3.png')"></li>
        </ul>
        <ul class="sci">
            <li><a href="#"><img src="./img/facebook.png"></a></li>
            <li><a href="#"><img src="./img/twitter.png"></a></li>
            <li><a href="#"><img src="./img/instagram.png"></a></li>
        </ul>
    </section>
    <script type="text/javascript">
        function imgSlider(anything){
            document.querySelector('.Strabucks') .src = anything;
        }
    </script>
</body>
</html>


#CSS


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
section {
    position: relative;
    width: 100%;
    min-height: 100vh;
    padding: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #fff;
}
header {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    padding: 20px 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header .logo {
    position: relative;
    max-width: 80px;
}

header ul {
    position: relative;
    display: flex;
}
header ul li {
    list-style: none;
}
header ul li a {
    display: inline-block;
    color: #333;
    font-weight: 400;
    margin-left: 40px;
    text-decoration: none;
}
.content 
{
    position: relative;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.content .textBox
{
    position: relative;
    max-width: 600px;
}
.content .textBox h2 
{
    color: #333;
    font-size: 4em;
    line-height: 1.4em;
    font-weight: 500;
}
.content .textBox h2 span
{
    color: #017143;
    font-size: 1.2em;
    font-weight: 900;
}
.content .textBox p 
{
    color: #333;
}
.content .textBox a
{
    display: inline-block;
    margin-top: 20px;
    padding: 8px 20px;
    background: #017143;
    color: #fff;
    border-radius: 40px;
    font-weight: 500;
    letter-spacing: 1px;
    text-decoration: none;
}

.content .imgBox 
{
    width: 600px;
    display: flex;
    justify-content: flex-end;
    padding-right: 50px;
    margin-top: 50px;
}
.content .imgBox img 
{
    max-width: 340px;
}
.thumb
{
    position: absolute;
    left: 50%;
    bottom: 20px;
    transform: translateX(-50%);
    display: flex;
}
.thumb li 
{
    list-style: none;
    display: inline-block;
    margin: 0 20px;
    cursor: pointer;
    transition: 0.5s;
}
.thumb li :hover
{
    transform: translateY(-15px);
}
.thumb li img 
{
    max-width: 60px;

}
.sci 
{
    position: absolute;
    top: 50%;
    right: 30px;
    transform: translateY(-50%);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.sci li 
{
    list-style: none;
}
.sci li a 
{
    display: inline-block;
    margin: 5px 0;
    transform: scale(0.6);
}
.circle 
{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    /*background-color: #017143;
    clip-path: circle(600px at right 800px);*/

}
