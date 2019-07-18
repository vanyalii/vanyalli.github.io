<!DOCTYPE html>
<html lang="en">
<head>

  <title>Leonardo Da Vinci</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
  <link href="https://fonts.googleapis.com/css?family=Montserrat" rel="stylesheet">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>
  <link rel="stylesheet" type="text/css" href="style\style.css">
</head>
<body onload="startTime()">

<div id="home"><div>
<nav  class="navbar navbar-default navbar-fixed-top">
  <div class="container">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#myNavbar">
      </button>
      <a class="navbar-brand" href="#">Leonardo Da Vinci</a>
    </div>
    <div class="collapse navbar-collapse" id="myNavbar">
      <ul class="nav navbar-nav navbar-right">
        <li><a href="#home">HOME</a></li>
        <li><a href="#aboutme">ABOUT ME</a></li>
        <li><a href="#portfolio">PORTFOLIO</a></li>
        <li><a href="#contact">CONTACT</a></li>
        <li><div id="zegar"></div></li>
      </ul>
    </div>
  </div>
</nav>


<div class="container-fluid bg-1 text-center">
  <h3 class="margin">Kim jestem?</h3>
  <img src="jpg\vinci.jpg" class="img-responsive img-circle margin" style="display:inline" alt="Leonardo" width="350" height="350">
  <h3>Renesansowy malarz, architekt, filozof, muzyk, pisarz, odkrywca, matematyk, mechanik, anatom, wynalazca, geolog, rzeźbiarz</h3>
</div>
<div id="aboutme"><div>
<div class="container-fluid bg-2 text-center">
  <h3 class="margin">Leonardo Da Vinci</h3>
  <p>Jestem często był opisywany jako archetyp „człowieka renesansu”, którego, wydawałoby się, niespożytej ciekawości dorównywała tylko siła jego kreatywności. Szeroko uważa się mnie za jednego z największych malarzy wszech czasów i prawdopodobnie najwszechstronniej utalentowaną osobę w historii. To właśnie talent malarski przysporzył mi największej popularności. Dwie z moich prac, Mona Lisa i Ostatnia Wieczerza, zajmują czołowe miejsca na listach najsławniejszych, najczęściej imitowanych i wspominanych portretów i dzieł malarstwa. Równie wielkie znaczenie w historii sztuki ma szkic Człowiek witruwiański. <br />
Jako inżynier, stowrzyłem projekty wyprzedzające moje czasy, opracowując koncepcje śmigłowca, czołgu, wykorzystania podstaw tektoniki płyt, podwójnego poszycia burt statku i wiele innych innowacji. Względnie mała liczba jego pomysłów została wcielona w życie za jego czasów. Niektóre z jego pomniejszych pomysłów, takie jak automatyczna nawijarka do szpul czy maszyna do sprawdzania wytrzymałości drutu na rozciąganie, weszły do świata techniki bez większego rozgłosu.</p>
</div>
<div id="portfolio"><div>
<div class="container-fluid bg-3 text-center">
  <h3 class="margin">Moje dzieła</h3><br>
  <div class="row">
    <div class="col-sm-4">
      <p>Dama z gronostajem</p>
      <img src="jpg\dama.jpg" class="img-responsive img-rounded margin" style="width:100%" alt="Dama z gronostajem">
    </div>
    <div class="col-sm-4">
      <p>Madonna wśród skał</p>
      <img  src="jpg\madonna.jpg" class="img-responsive img-rounded margin" style="width:83%"  alt="madonna">
    </div>
    <div class="col-sm-4">
      <p>Projekt Człowieka witruwiańskiego</p>
      <img src="jpg\czlowiek.jpg" class="img-responsive img-rounded margin" style="width:96%" alt="Człowiek witruwiański">
    </div>
  </div>
</div>
<div id="contact"><div>
  <div class="container-fluid bg-2 text-center">
    <h3 class="margin">Kontakt</h3>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d92181.08820592653!2d11.170928076872391!3d43.77993676478598!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x132a56a680d2d6ad%3A0x93d57917efc72a03!2sFlorencja%2C+W%C5%82ochy!5e0!3m2!1spl!2spl!4v1561908028229!5m2!1spl!2spl" width="80%" height="350" frameborder="0" style="border:0" allowfullscreen></iframe>

  </div>
  <footer class="container-fluid bg-4 text-center">
<p>Pozdrawiam Leonardo</p>
</footer>

</body>



<script>
function startTime() {
  var today = new Date();
  var h = today.getHours();
  var m = today.getMinutes();
  var s = today.getSeconds();
  m = checkTime(m);
  s = checkTime(s);
  document.getElementById('zegar').innerHTML =
  h + ":" + m + ":" + s;
  var t = setTimeout(startTime, 500);
}
function checkTime(i) {
  if (i < 10) {i = "0" + i};
  return i;
}
</script>
</html>
