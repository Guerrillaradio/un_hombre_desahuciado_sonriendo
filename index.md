              
<p><a href="https://guerrillaradio.github.io/Q/"><div><font color="#000">❤</font></div><div></div><div><font color="#000"> </font><font color="#000"> </font></div></a>
  
<p>
<p>    
<div><font color="#00ff00">En la mañana del segundo, Louis de Broglie expuso su nueva teoría de «ondas piloto»,</font></div><div></div><div><font color="#00ff00"> </font><font color="#00ff00"> </font></div>
<div><font color="#00ff00">que explicaba el movimiento del electrón como si estuviera viajando montado,</font></div><div></div><div><font color="#00ff00"> </font><font color="#00ff00"> </font></div>
<div><font color="#00ff00">en la cúspide de una onda, al igual que un surfista</font></div><div></div><div><font color="#00ff00"> </font><font color="#00ff00"> </font></div>
<div></div>  

{% raw %}
<script>
(function () {
  const ACTIVATION_CLICKS = 7;
  const LOOP_DURATION_MS = 180000; // 3 minutos

  const clicksKey = 'heartClicks';
  const loopUntilKey = 'loopUntil';

  const now = Date.now();

  let clicks = parseInt(localStorage.getItem(clicksKey) || '0', 10);
  clicks++;
  localStorage.setItem(clicksKey, clicks);

  if (clicks === ACTIVATION_CLICKS) {
    localStorage.setItem(loopUntilKey, now + LOOP_DURATION_MS);
  }

  const loopUntil = parseInt(localStorage.getItem(loopUntilKey) || '0', 10);

  if (now < loopUntil) {
    const here = window.location.href;

    if (here.includes('/Q/')) {
      window.location.href = 'https://guerrillaradio.github.io/un_hombre_desahuciado_sonriendo/';
    }

    if (here.includes('un_hombre_desahuciado_sonriendo')) {
      window.location.href = 'https://guerrillaradio.github.io/Q/';
    }
  }

  if (loopUntil && now >= loopUntil) {
    localStorage.removeItem(loopUntilKey);
  }
})();
</script>
{% endraw %}




