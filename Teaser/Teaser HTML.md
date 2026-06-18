




\<div id="startScreen"\>

  CLICK TO START

\</div\>


\<audio id="introSound" src="Intro/Better2.mp3" preload="auto"\>\</audio\>




\<style\>

\#startScreen \{

  position: fixed;

  inset: 0;

  z-index: 999999;

  background: black;

  color: white;

  display: flex;

  align-items: center;

  justify-content: center;

  font-family: Georgia, serif;

  font-size: 2em;

  cursor: pointer;

\}

\</style\>


\<script\>

setTimeout(function () \{

  var btn = document.getElementById("startScreen");

  var sound = document.getElementById("introSound");


  btn.onclick = function () \{

    btn.style.display = "none";

    sound.volume = 1;

    sound.currentTime = 0;

    sound.play();

  \};

\}, 100);

\</script\>


\<div id="faceWrap"\>

\<img id="face1" src="Intro/1.png"\>

\<img id="face2" src="Intro/2.png"\>

\</div\>


\<div id="prototypeTitle"\>

  \<span class="p p1"\>P\</span\>

  \<span class="p p2"\>R\</span\>

  \<span class="p p3"\>O\</span\>

  \<span class="p p4"\>T\</span\>

  \<span class="p p5"\>O\</span\>

  \<span class="p p6"\>T\</span\>

  \<span class="p p7"\>Y\</span\>

  \<span class="p p8"\>P\</span\>

  \<span class="p p9"\>E\</span\>

\</div\>


\<div id="titleWrap"\>

\<span class="noemeChar n" data-letter="N"\>N\</span\>

\<span class="noemeChar o" data-letter="O"\>O\</span\>

\<span class="noemeChar e1" data-letter="E"\>E\</span\>

\<span class="noemeChar m" data-letter="M"\>M\</span\>

\<span class="noemeChar e2" data-letter="E"\>E\</span\>

\</div\>


\<style\>

\#titleWrap \{

  position: fixed;

  top: 55%;

  left: 50%;

  transform: translateX(-50%);

  z-index: 3;

  display: flex;

  gap: 0.20em;


  font-family: "Cormorant Garamond", Georgia, serif;

  font-size: 3em;

  font-weight: 300;

  letter-spacing: 0.21em;

color: rgba(185,185,190,0.4);


text-shadow: 0 0 2px rgba(255,255,255,0.04);


  filter: blur(13px);

  animation: noemeWordUnblur 2s ease 3.8s forwards;

  

\}


.noemeChar \{

  opacity: 0;

  filter: blur(8px);

  display: block;

  animation-fill-mode: forwards;

\}



:root \{


  --prototype-out: 14s;


\}




.e2 \{ animation: appearN 0.4s ease 3.2s forwards, vanishN 39.5s ease 5.5s forwards; \}


.m  \{ animation: appearN 0.4s ease 2.6s forwards, vanishN 29s ease 5.7s forwards; \}


.e1 \{ animation: appearN 0.4s ease 2s forwards, vanishN 20.5s ease 5.9s forwards; \}


.n  \{ animation: appearN 0.4s ease 0.8s forwards, vanishN  15s ease 6.1s forwards; \}


.o  \{ animation: appearN 0.4s ease 1.4s forwards, vanishN  8.2s ease 6.3s forwards; \}



@keyframes appearN \{

  from \{

    opacity: 0;

    filter: blur(0px);

  \}


  to \{

    opacity: 1;

    filter: blur(0);

  \}

\}

@keyframes vanishN \{

  0% \{

    opacity: 100;

    filter: blur(1px);

    text-shadow:

      0 0 0 rgba(255,255,255,0.6);

  \}


  30% \{

    opacity: 0;

    filter: blur(0px);

    text-shadow:

      0 0 10px rgba(255,255,255,0.05),

      0 0 22px rgba(255,255,255,0.1);

  \}



  100% \{

    opacity: 0 ;

    filter: blur(0px);

    text-shadow:

      0 0 20px rgba(255,255,255,0.18),

      0 0 42px rgba(255,255,255,0.08);

  \}

\}


@keyframes noemeWordUnblur \{

  from \{ filter: blur(12px); \}

  to   \{ filter: blur(0); \}

\}



\</style\>




\#faceWrap \{

  position: fixed;

  inset: 0;

  z-index: 1;

  background: \#000;

  overflow: hidden;

\}


\#faceWrap img \{

  position: absolute;

  inset: 0;

  width: 100%;

  height: 100%;

  object-fit: contain;

  opacity: 0;

  display: block;

\}


\#face1 \{

  animation:

    faceOneFade 1.5s ease 3.8s forwards,

    faceOneOut 3s ease 17s forwards;

  z-index: 1;

\}


\#face2 \{

  animation:

    faceTwoFade 1.5s ease 7s forwards,

    faceTwoOut 3s ease 13s forwards;

  z-index: 2;

\}



@keyframes faceOneFade \{

  from \{ opacity: 0; \}

  to   \{ opacity: 1; \}

\}


@keyframes faceTwoFade \{

  from \{ opacity: 0; \}

  to   \{ opacity: 1; \}

\}


@keyframes faceOneOut \{

  from \{ opacity: 1; \}

  to   \{ opacity: 0; \}

\}


@keyframes faceTwoOut \{

  from \{ opacity: 1; \}

  to   \{ opacity: 0; \}

\}


\#prototypeTitle \{

  position: fixed;

  top: 66%;

  left: 50%;

  transform: translateX(-50%);

  z-index: 3;

  display: flex;

  gap: 0.15em;


  font-family: "Cormorant Garamond", Georgia, serif;

  font-size: 2.1em;

  font-weight: 300;

  letter-spacing: 0.32em;


color: rgba(165,170,180,0.3);

  text-shadow: 0 0 4px rgba(180,190,210,0.04);

\}



.p \{

  opacity: 0;

  filter: blur(8px);

  display: block;

  animation:

    prototypeAppear 0.2s ease forwards,

    prototypeVanish var(--prototype-out) ease forwards;

\}


.p9 \{ animation-delay: 4.18s, 5.5s; \} /\* right \*/

.p1 \{ animation-delay: 4.17s, 5.6s; \} /\* left \*/


.p8 \{ animation-delay: 4.16s, 5.7s; \} /\* right \*/

.p2 \{ animation-delay: 4.15s, 5.8s; \} /\* left \*/


.p7 \{ animation-delay: 4.14s, 5.9s; \} /\* right \*/

.p3 \{ animation-delay: 4.13s, 6s; \} /\* left \*/


.p6 \{ animation-delay: 4.12s, 6.1s; \} /\* right \*/

.p4 \{ animation-delay: 4.11s, 6.2s; \} /\* left \*/


.p5 \{ animation-delay: 4.10s, 6.3s; \} /\* center O \*/


@keyframes prototypeAppear \{

  0% \{

    opacity: 0;

    filter: blur(1px);

    text-shadow: 0 0 0 rgba(255,255,255,0);

  \}


  35% \{

    opacity: 0.8;

    filter: blur(1px);

    text-shadow:

      0 0 15px rgba(255,255,255,0.45),

      0 0 25px rgba(180,190,210,0.55);

  \}


  100% \{

    opacity: 0.7;

    filter: blur(0);

    text-shadow:

      0 0 6px rgba(255,255,255,0.),

      0 0 12px rgba(180,190,210,0.35);

  \}

\}


@keyframes prototypeVanish \{

  0% \{

    opacity: 0;

    filter: blur(0px);

    text-shadow:

      0 0 8px rgba(255,255,255,0.21),

      0 0 12px rgba(180,190,210,0.1);

  \}


  45% \{

    opacity: 0;

    filter: blur(0px);

    text-shadow:

      0 0 10px rgba(255,255,255,0.4),

      0 0 22px rgba(180,190,210,0.55);

  \}


  100% \{

    opacity: 0;

    filter: blur(0px);

    text-shadow:

      0 0 5px rgba(255,255,255,0.15),

      0 0 10px rgba(180,190,210,0.08);

  \}

\}
