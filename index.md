---
layout: default
title: Aktiv in Sekunden
---

# Toolbox
Kurze Übungen mit Bildern und Textanleitungen.

<div style="margin: 12px 0;">
  <a href="#" id="openGallery" style="display:inline-block; text-decoration:none;">
    <div style="width:260px; border:1px solid #eee; border-radius:16px; overflow:hidden; box-shadow:0 2px 10px rgba(0,0,0,0.06);">
      <img src="assets/img/1.png" alt="Galerie öffnen" style="width:100%; height:180px; object-fit:cover; display:block;">
      <div style="padding:12px; font-weight:600;">Galerie öffnen</div>
      <div style="padding:0 12px 12px 12px; color:#666; font-size:14px;">2 Bilder (Probe) – klicken zum Durchblättern</div>
    </div>
  </a>
</div>

<link rel="stylesheet" href="https://unpkg.com/photoswipe@5/dist/photoswipe.css">

<div class="pswp-gallery" id="galerie" style="display:none;">
  <a href="assets/img/1.png" data-pswp-width="1748" data-pswp-height="1240"></a>
  <a href="assets/img/2.png" data-pswp-width="1748" data-pswp-height="1240"></a>
</div>

<script src="https://unpkg.com/photoswipe@5/dist/photoswipe-lightbox.umd.min.js"></script>
<script src="https://unpkg.com/photoswipe@5/dist/photoswipe.umd.min.js"></script>
<script>
  document.addEventListener('DOMContentLoaded', function () {
    const lightbox = new PhotoSwipeLightbox({
      gallery: '#galerie',
      children: 'a',
      pswpModule: PhotoSwipe
    });
    lightbox.init();

    const btn = document.getElementById('openGallery');
    if (btn) {
      btn.addEventListener('click', function(e){
        e.preventDefault();
        lightbox.loadAndOpen(0);
      });
    }
  });
</script>

# Poster
Vier Poster mit Übungsbeispielen und Ideen zur Ritualisierung in Deinem Alltag.

# 30-Tage-Challenge
Challenge-Vorlagen, um Deine Erfolge zu tracken und im Team mit- bzw. gegeneinander anzutreten.

# Sticker und Hintergrundbilder
Zur Erinnerung an Deine aktiven Sekunden.

# Kontakt
Weitere Informationen unter:
