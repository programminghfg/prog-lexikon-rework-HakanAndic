<script>
import csspad from '$lib/img/csspad.png';
import divPad from '$lib/img/divPad.png';
import divPad1 from '$lib/img/divPad1.png';
import divPad2 from '$lib/img/divPad2.png';
import MarginPadding from '$lib/img/MarginPadding.png';
import padding from '$lib/img/padding.png';
</script>

<a href="/">Home</a>
<div class="site">
        <div class="content">
               
                   
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="css/style.css">
    <link rel="stylesheet" type="text/css" href="css/mobile.css">
    <link rel="stylesheet" type="text/css" href="fonts/stylesheet.css">

    <title>Margin & Padding</title>
</head>

<body>
    <div id="wrapper">
        <header>Margin & Padding</header>
        <nav>
            <ul class="nav-links">
                <li class="nav-item"><a href="../index.html">Home</a></li>
                <li class="nav-item"><a href="#">Grundlegendes</a></li>
                <li class="nav-item"><a href="#">Unterkategorien</a></li>
                <li class="nav-item"><a href="#">Responsive</a></li>
            </ul>
        </nav>
        <aside>
            <img src={MarginPadding} alt=Margin id="pic7">
        </aside>
        <div id="dscbtn">
            <h1>Margin</h1>
            In HTML und CSS bezieht sich der Begriff "Margin" auf den Abstand zwischen den Rändern eines Elements und
            den Rändern des umgebenden Elements.
            Der Margin kann entweder auf der oberen, unteren, linken oder rechten Seite des Elements angewendet werden
            oder auf alle vier Seiten gleichzeitig.
            <br><br>
            In CSS kannst du den Margin eines Elements mithilfe der Eigenschaften "margin-top", "margin-bottom",
            "margin-left" und "margin-right" festlegen.
            Du kannst entweder eine feste Größe wie z.B. "10px" oder eine relative Größe wie z.B. "10%" angeben. Wenn du
            den Margin auf alle vier Seiten gleichzeitig anwenden möchtest, kannst du die Kurzschreibweise "margin"
            verwenden, gefolgt von den Werten für die oberen, rechten, unteren und linken Ränder in dieser Reihenfolge.
            <br><br>

            <h1>Padding</h1>
            In HTML und CSS bezieht sich der Begriff "Padding" auf den Abstand zwischen dem Inhalt eines Elements und
            dem Rand des Elements.
            Das Padding kann entweder auf der oberen, unteren, linken oder rechten Seite des Elements angewendet werden
            oder auf alle vier Seiten gleichzeitig.
            <br><br>
            In CSS kannst du das Padding eines Elements mithilfe der Eigenschaften "padding-top", "padding-bottom",
            "padding-left" und "padding-right" festlegen.
            Du kannst entweder eine feste Größe wie z.B. "10px" oder eine relative Größe wie z.B. "10%" angeben. Wenn du
            das Padding auf alle vier Seiten gleichzeitig anwenden möchtest,
            kannst du die Kurzschreibweise "padding" verwenden, gefolgt von den Werten für die oberen, rechten, unteren
            und linken Ränder in dieser Reihenfolge.
            <br><br>


        </div>
       
        <footer>
            <ul class="ftr-links">
                <li class="ftr-item"><a href="#">Impressum</a></li>
                <li class="ftr-item"><a href="#">Kontakt</a></li>
                <li class="ftr-item"><a href="#">Datenschutz</a></li>
            </ul>
        </footer>
    </div>
</body>
</div>
</div>


<style>
    *{
    opacity: 1;
    color: white;
    background-color: #333333;
    font-family: 'Open Sans', sans-serif;

}

#wrapper{
    display: grid;
    width: 2000px;
    margin: auto;
    grid-template-columns: repeat(6,1fr);
    grid-template-rows: 120px 50px 600px 100px 40px 70px;
    grid-template-areas: 
        "hdr hdr hdr hdr hdr hdr"
        "nv nv nv nv nv nv"
        "dscbtn dscbtn dscbtn dscbtn asd asd"
        "pic1 pic2 pic3 pic4 pic5 pic6"
        "tag1 tag2 tag3 tag4 tag5 tag6"
        "ftr ftr ftr ftr ftr ftr";
}

header {
    font-weight: bold;
    background-color: #333333;
    padding: 10px;
    grid-area: hdr;
    font-size: 50pt;
}

nav {
    margin-left: 0px;
    margin: 0px;
    background-color: #333333;
    grid-area: nv;
    display: flex;
    justify-content: space-between;
    align-items: center;

}

.nav-links {
    margin-left: 0;
    list-style: none;
    display: flex;
    justify-content: left;
    background-color: #333333;

}

.nav-item a {
    margin-left: 0;
    display: inline-block;
    padding-right: 15px;
    text-decoration: none;
    background-color: #333333;
}

aside{
    background-color: #333333;
    grid-area: asd;
    padding: 80px;
}

#pic7{
    max-width: 500px;
    justify-self: center;
    grid-area: asd;
}

#dscbtn {
    padding: 20px;
    background-color: #333333;
    grid-area: dscbtn;
}



footer {
    background-color: #333333;
    grid-area: ftr;
    margin-top: 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;

}



</style>