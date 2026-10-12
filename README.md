<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="icon" type="image/gif" href="https://i.pinimg.com/originals/f7/2a/1c/f72a1cb4c70a0ae5ad99a6d20ff1f7d7.gif">  
<title>For Nielle 💖</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', sans-serif; }
        body { background: linear-gradient(135deg, #fff7f9, #ffe4e1, #ffecd2); min-height: 100vh; }
        .container { max-width: 1200px; margin: 0 auto; padding: 2rem; }
        
        /* Envelope */
        .envelope-container { display: flex; justify-content: center; align-items: center; min-height: 85vh; cursor: pointer; transition: opacity 0.5s ease; }
        .envelope-container.hidden { opacity: 0; pointer-events: none; }
        .envelope { position: relative; width: 360px; height: 230px; background: linear-gradient(135deg, #ffd4c4, #ffb5a7); border-radius: 12px; box-shadow: 0 15px 30px rgba(212,115,106,0.25); transition: transform 0.4s ease; transform-style: preserve-3d; }
        .envelope:hover { transform: translateY(-8px); }
        .flap { position: absolute; top: 0; left: 0; width: 100%; height: 130px; background: linear-gradient(180deg, #ffc9b9, #ffb5a7); clip-path: polygon(0 0, 50% 45%, 100% 0); transform-origin: top center; transition: transform 0.8s ease; z-index: 3; }
        .envelope.opened .flap { transform: rotateX(180deg); }
        .seal { position: absolute; top: 95px; left: 50%; transform: translateX(-50%); width: 50px; height: 50px; background: #fff; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1.4rem; z-index: 5; transition: all 0.5s ease; }
        .envelope.opened .seal { opacity: 0; transform: translateX(-50%) scale(0); }
        .envelope-text { position: absolute; bottom: 35px; left: 50%; transform: translateX(-50%); font-size: 1.2rem; color: #8b5a50; font-weight: 600; }
        
        /* Content */
        .content-wrapper { display: none; opacity: 0; transform: translateY(20px); transition: all 1s ease-out; }
        .content-wrapper.show { display: block; opacity: 1; transform: translateY(0); }
        .top-title { text-align: center; padding: 1rem 0 2rem; color: #d4736a; }
        .top-title h1 { font-size: 2.5rem; animation: bounce 1.5s ease-in-out infinite alternate; }
        @keyframes bounce { from { transform: translateY(0); } to { transform: translateY(-8px); } }
        
        .letter-section { background: #fff; border-radius: 20px; padding: 2.5rem; margin: 0 auto 3rem; box-shadow: 0 10px 30px rgba(212,115,106,0.18); line-height: 1.8; color: #5a4a4a; max-width: 900px; }
        .letter-section h2 { color: #e0897f; margin-bottom: 1.5rem; padding-bottom: 0.5rem; border-bottom: 2px solid #ffd4c4; }
        .signature { margin-top: 2rem; text-align: right; font-style: italic; color: #d4736a; font-weight: bold; }
        
        /* Photos */
        .photo-section { opacity: 0; transform: translateY(30px); transition: all 1s ease-out 0.5s; }
        .photo-section.show { opacity: 1; transform: translateY(0); }
        .photo-section h2 { text-align: center; color: #d4736a; margin-bottom: 2rem; font-size: 1.8rem; }
        .photo-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem; }
        .photo-card { border-radius: 16px; overflow: hidden; background: #fff; box-shadow: 0 6px 15px rgba(212,115,106,0.12); opacity: 0; transform: translateY(20px); transition: all 0.7s ease-out; cursor: pointer; }
        .photo-card.show { opacity: 1; transform: translateY(0); }
        .photo-card:hover { transform: translateY(-5px); }
        .photo-card img { width: 100%; height: 260px; object-fit: cover; display: block; }
        
        /* Lightbox */
        .lightbox { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.85); display: flex; align-items: center; justify-content: center; z-index: 1000; opacity: 0; visibility: hidden; transition: all 0.3s ease; padding: 2rem; }
        .lightbox.active { opacity: 1; visibility: visible; }
        .lightbox img { max-width: 90%; max-height: 85vh; border-radius: 12px; transform: scale(0.8); transition: transform 0.3s ease; }
        .lightbox.active img { transform: scale(1); }
        
        /* Confetti */
        .confetti { position: fixed; width: 10px; height: 10px; opacity: 0.8; animation: fall 5s linear infinite; pointer-events: none; }
        @keyframes fall { 0% { transform: translateY(-10px) rotate(0deg); } 100% { transform: translateY(100vh) rotate(720deg); } }
        
        /* Responsive */
        @media (max-width: 900px) { .photo-grid { grid-template-columns: repeat(2, 1fr); } }
        @media (max-width: 550px) { .photo-grid { grid-template-columns: 1fr; } .photo-card img { height: 220px; } }

/* PINK ENVELOPE BADGE — GLOW ANIMATION */
.envelope {
  background: linear-gradient(135deg, #ffc2d1, #ff9ebb, #ff7aa2) !important;
  box-shadow: 
    0 0 20px rgba(255,122,162,0.5),
    0 0 40px rgba(255,158,187,0.3),
    inset 0 0 15px rgba(255,255,255,0.2);
  animation: pinkGlow 2s ease-in-out infinite;
}
.flap {
  background: linear-gradient(180deg, #ffd6e0, #ffb6c9) !important;
}
.seal {
  background: #fff0f5 !important;
  color: #ff4d80 !important;
  box-shadow: 0 0 10px rgba(255,77,128,0.3) !important;
}
.envelope-text {
  color: #b33a60 !important;
}

@keyframes pinkGlow {
  0% {
    box-shadow: 
      0 0 20px rgba(255,122,162,0.5),
      0 0 40px rgba(255,158,187,0.3);
  }
  50% {
    box-shadow: 
      0 0 30px rgba(255,122,162,0.7),
      0 0 60px rgba(255,158,187,0.5);
  }
  100% {
    box-shadow: 
      0 0 20px rgba(255,122,162,0.5),
      0 0 40px rgba(255,158,187,0.3);
  }
}

        
    </style>

</head>
<body>
    <div class="lightbox" id="lightbox"><img src="" alt="" id="lightboxImg"></div>

    <div class="container">
        <div class="envelope-container" id="envelopeContainer">
            <div class="envelope" id="envelope">
                <div class="flap"></div>
                <div class="seal">💌</div>
                <div class="envelope-text">Open the Letter</div>
            </div>
        </div>

        <div class="content-wrapper" id="contentWrapper">
            <div class="top-title"><h1>✨ Happy 18th Birthday Nielle! ✨</h1></div>

            <div class="letter-section">
                <h2>To My Dearest Nielle,</h2>
                <p> It’s been a while, Nielle! Kamusta? Welcome to college life. Hindi tayo masyadong nag-usap noong nagkita tayo since busy ka
                     that time preparing for your debut hehehhaha. So… may jowa ka na ba?
    As for me, ginawang rebound ako, jusko po. turns out he wasn’t ready at all and still misses his ex, hahaha. (Nasaan na yung alak? XD)
    As for my update about sa life ko… hmmm, I shifted and transferred schools and changed my course, kasi why not.
    I’m now taking Bachelor of Science in Entertainment and Multimedia Computing, major in Game Development, mostly drawing, making games,
    that kind of stuff. Lola Dory doesn’t even know I switched courses yet, XD. 
    Everything’s good though, Tita Chie’s doing great and is still a certified K-pop fan.
    Bubbles? Always sleeping and asking for Jollibee chicken, as usual. When gala naten magpipinsan?XD
    <br> 
<br>
        But anyways, you’re officially an adult now, and I couldn’t be prouder of the amazing person you’ve become. 
        kailan lang 14 years old ka lang eh, tapos bigla 18 ka na. Ang bilis talaga ng panahon, ‘no? 
        Naalala ko pa nga noong iyakin ka pa dati, nung 3–4 years old ka pa lang. Tapos ngayon puro alak na
        Watching you grow has been such a blessing, kahit minsan lang tayo magkita I know this new chapter will be filled with 
        adventures, dreams coming true, and endless happiness.
        Thank you for being uhhh… being pinsan parang nakita kapatid kinda.
        And I’m so happy being your pinsan. I just really mean it, sobrang thankful ako sa’yo.
        Parang tunay na kapatid talaga ang turing ko sa’yo, kahit ano pa man. Andito lang ako palagi para sa’yo, no matter what.
         Super proud ako sa’yo always. May this year bring you closer to everything you’ve ever wished for.
         Never forget how talented, smart, and truly wonderful you are.
        Don’t be afraid to chase your dreams, you’re capable of achieving anything you set your heart on.
        I hope your 18th birthday is as magical and extraordinary as you are. Always take care of yourself, okay? Drink water, eat well, 
        and sleep properly. 
        Here’s to new beginnings and beautiful memories ahead.
        Once again, Happy 18th Birthday, Nielle! :D
<p class="signature">With all my love,<br>Your Ate Xyza</p>
     </div>

            <div class="photo-section" id="photoSection">
                <h2> Memories  </h2>
                <div class="photo-grid">
                    <div class="photo-card"><img src="1a.jpg" ></div>
                    <div class="photo-card"><img src="1b.jpg" ></div>
                    <div class="photo-card"><img src="1c.jpg" ></div>
                    <div class="photo-card"><img src="1d.jpg" ></div>
                    <div class="photo-card"><img src="1e.jpg" ></div>
                    <div class="photo-card"><img src="1f.jpg" ></div>
                    <div class="photo-card"><img src="1g.jpg" ></div>
                    <div class="photo-card"><img src="1h.jpg" ></div>
                    <div class="photo-card"><img src="1i.jpg" ></div>
                    <div class="photo-card"><img src="1j.jpg" ></div>
                    <div class="photo-card"><img src="1k.jpg" ></div>
                    <div class="photo-card"><img src="1kk.jpg" ></div>



                    <div class="photo-card"><img src="1.jpg" ></div>
                    <div class="photo-card"><img src="2.jpg" alt="Memory 2"></div>
                    <div class="photo-card"><img src="3.jpg" alt="Memory 3"></div>
                    <div class="photo-card"><img src="4.jpg" alt="Memory 4"></div>
                    <div class="photo-card"><img src="5.jpg" alt="Memory 5"></div>
                    <div class="photo-card"><img src="6.jpg" alt="Memory 6"></div>
                    <div class="photo-card"><img src="7.jpg" alt="Memory 7"></div>
                    <div class="photo-card"><img src="8.jpg" alt="Memory 8"></div>
                    <div class="photo-card"><img src="9.jpg" alt="Memory 9"></div>
                    <div class="photo-card"><img src="10.jpg" alt="Memory 10"></div>
                    
                    <div class="photo-card"><img src="11.jpg" alt="Memory 11"></div>
                    <div class="photo-card"><img src="12.jpg" alt="Memory 12"></div>
                    <div class="photo-card"><img src="13.jpg" alt="Memory 13"></div>
                    <div class="photo-card"><img src="14.jpg" alt="Memory 14"></div>
                    <div class="photo-card"><img src="15.jpg" alt="Memory 15"></div>
                    <div class="photo-card"><img src="16.jpg" alt="Memory 16"></div>
                    <div class="photo-card"><img src="17.jpg" alt="Memory 17"></div>
                    <div class="photo-card"><img src="18.jpg" alt="Memory 18"></div>
                    <div class="photo-card"><img src="19.jpg" alt="Memory 19"></div>
                    <div class="photo-card"><img src="20.jpg" alt="Memory 20"></div>
                    
                    <div class="photo-card"><img src="21.jpg" alt="Memory 21"></div>
                    <div class="photo-card"><img src="22.jpg" alt="Memory 22"></div>
                    <div class="photo-card"><img src="23.jpg" alt="Memory 23"></div>
                    <div class="photo-card"><img src="24.jpg" alt="Memory 24"></div>
                    <div class="photo-card"><img src="25.jpg" alt="Memory 25"></div>
                    <div class="photo-card"><img src="26.jpg" alt="Memory 26"></div>
                    <div class="photo-card"><img src="27.jpg" alt="Memory 27"></div>
                    <div class="photo-card"><img src="28.jpg" alt="Memory 28"></div>
                    <div class="photo-card"><img src="29.jpg" alt="Memory 29"></div>
                    <div class="photo-card"><img src="30.jpg" alt="Memory 30"></div>
                    
                    <div class="photo-card"><img src="31.jpg" alt="Memory 31"></div>
                    <div class="photo-card"><img src="32.jpg" alt="Memory 32"></div>
                    <div class="photo-card"><img src="33.jpg" alt="Memory 33"></div>
                    <div class="photo-card"><img src="34.jpg" alt="Memory 34"></div>
                    <div class="photo-card"><img src="35.jpg" alt="Memory 35"></div>
                    <div class="photo-card"><img src="36.jpg" alt="Memory 36"></div>
                    <div class="photo-card"><img src="37.jpg" alt="Memory 37"></div>
                    <div class="photo-card"><img src="38.jpg" alt="Memory 38"></div>
                    <div class="photo-card"><img src="39.jpg" alt="Memory 39"></div>
                    <div class="photo-card"><img src="40.jpg" alt="Memory 40"></div>
                    
                    <div class="photo-card"><img src="41.jpg" alt="Memory 41"></div>
                    <div class="photo-card"><img src="42.jpg" alt="Memory 42"></div>
                    <div class="photo-card"><img src="43.jpg" alt="Memory 43"></div>
                    <div class="photo-card"><img src="44.jpg" alt="Memory 44"></div>
                    <div class="photo-card"><img src="45.jpg" alt="Memory 45"></div>
                    <div class="photo-card"><img src="46.jpg" alt="Memory 46"></div>
                    <div class="photo-card"><img src="47.jpg" alt="Memory 47"></div>
                    <div class="photo-card"><img src="48.jpg" alt="Memory 48"></div>
                    <div class="photo-card"><img src="49.jpg" alt="Memory 49"></div>
                    <div class="photo-card"><img src="50.jpg" alt="Memory 50"></div>
                    
                </div>
            </div>
        </div>
    </div>

    <script>
        const lightbox = document.getElementById('lightbox');
        const lightboxImg = document.getElementById('lightboxImg');
        function openLightbox(src) { lightboxImg.src = src; lightbox.classList.add('active'); document.body.style.overflow='hidden'; }
        function closeLightbox() { lightbox.classList.remove('active'); document.body.style.overflow=''; }
        lightbox.addEventListener('click', closeLightbox);
        document.addEventListener('keydown', e => e.key==='Escape' && closeLightbox());

        const envelopeContainer = document.getElementById('envelopeContainer');
        const envelope = document.getElementById('envelope');
        const contentWrapper = document.getElementById('contentWrapper');
        const photoSection = document.getElementById('photoSection');
        let opened = false;

        envelopeContainer.addEventListener('click', () => {
            if (opened) return;
            opened = true;
            envelope.classList.add('opened');
            setTimeout(() => envelopeContainer.classList.add('hidden'), 800);
            setTimeout(() => contentWrapper.classList.add('show'), 900);
            
            setTimeout(() => {
                photoSection.classList.add('show');
                const cards = document.querySelectorAll('.photo-card');
                cards.forEach((card, i) => {
                    setTimeout(() => {
                        card.classList.add('show');
                        card.querySelector('img').addEventListener('click', e => {
                            e.stopPropagation();
                            openLightbox(card.querySelector('img').src);
                        });
                    }, i * 60);
                });
            }, 1900);

            // Confetti
            const colors = ['#ffd4c4','#ffb5a7','#fcd5ce','#f8edeb','#f9c7c2','#e8a598'];
            function makeConfetti() {
                const c = document.createElement('div');
                c.className = 'confetti';
                c.style.left = Math.random()*100+'vw';
                c.style.backgroundColor = colors[Math.floor(Math.random()*colors.length)];
                c.style.width = c.style.height = (Math.random()*8+6)+'px';
                c.style.borderRadius = Math.random()>0.5 ? '50%' : '0';
                document.body.appendChild(c);
                setTimeout(()=>c.remove(),6000);
            }
            setInterval(makeConfetti, 300);
            for(let i=0;i<15;i++) setTimeout(makeConfetti,i*50);
        });
    </script>

    <!-- COPYRIGHT / DATE — BOTTOM OF PAGE -->
<footer style="text-align: center; padding: 1.5rem; color: #d4736a; font-size: 0.85rem; border-top: 1px solid #ffd4c4; margin-top: 2rem;">
  © Made with love for Nielle 💖 | Started: October 12, 2026
</footer>

</body>
</html>
