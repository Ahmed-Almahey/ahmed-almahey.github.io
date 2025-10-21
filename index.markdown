---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
author: Ahmed Almahey
author_profile: true
---
![Ahmed Almahey](/assets/images/IMG_20250911_153717.jpg){: style="float: none; display: block; margin: 0 auto; width: 440px;"}

<!-- Ahmed audio play button (paste this directly AFTER your image line) -->
<div class="ahm-audio-wrapper" aria-hidden="false">
  <button class="ahm-audio-btn" id="ahmPlayBtn" aria-label="Play Ahmed's introduction">
    <!-- PLAY TRIANGLE -->
    <svg class="ahm-icon ahm-play" viewBox="0 0 64 64" width="44" height="44" aria-hidden="true" focusable="false">
      <circle cx="32" cy="32" r="30" fill="none"/>
      <polygon points="26,20 47,32 26,44" />
    </svg>
    <!-- PAUSE BARS (hidden by default) -->
    <svg class="ahm-icon ahm-pause" viewBox="0 0 64 64" width="44" height="44" aria-hidden="true" focusable="false" style="display:none;">
      <rect x="20" y="18" width="6" height="28" rx="1"/>
      <rect x="38" y="18" width="6" height="28" rx="1"/>
    </svg>
  </button>
  <span class="ahm-audio-label">▶ Listen — short intro</span>

  <audio id="ahmIntroAudio" preload="none">
    <source src="/assets/audio/intro-ahmed-almahey.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</div>

<script>
(function(){
  var btn = document.getElementById('ahmPlayBtn');
  var audio = document.getElementById('ahmIntroAudio');
  var label = document.querySelector('.ahm-audio-label');
  if (!btn || !audio) return;

  function setPlaying(isPlaying){
    if(isPlaying){
      btn.classList.add('ahm-playing');
      var playSvg = btn.querySelector('.ahm-play');
      var pauseSvg = btn.querySelector('.ahm-pause');
      if(playSvg) playSvg.style.display = 'none';
      if(pauseSvg) pauseSvg.style.display = 'block';
      if(label) label.textContent = '⏸ Pause intro';
    } else {
      btn.classList.remove('ahm-playing');
      var playSvg = btn.querySelector('.ahm-play');
      var pauseSvg = btn.querySelector('.ahm-pause');
      if(playSvg) playSvg.style.display = 'block';
      if(pauseSvg) pauseSvg.style.display = 'none';
      if(label) label.textContent = '▶ Listen — short intro';
    }
  }

  btn.addEventListener('click', function(){
    if(audio.paused){
      audio.play().catch(function(e){ console.warn('Audio play failed', e); });
      setPlaying(true);
    } else {
      audio.pause();
      audio.currentTime = 0;
      setPlaying(false);
    }
  });

  audio.addEventListener('ended', function(){ setPlaying(false); });
  audio.addEventListener('pause', function(){ setPlaying(false); });
})();
</script>



# Hi there! I'm Ahmed Almahey
a Data Analyst and BI Developer with a background in Mathematics and Statistics. I’m passionate about transforming data into insights and creating impactful dashboards with Power BI and SQL. Explore my projects below or visit [My Work](/mywork) for more.
