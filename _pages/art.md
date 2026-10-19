---
title: "Art"
permalink: /art/
author_profile: true
---

Outside of research, I like to draw and paint — mostly pencil and ink drawings, and painted landscapes. Click any piece to see it larger.

<div class="art-gallery">
{% for piece in site.data.art %}
  <figure class="art-gallery__item">
    <a href="{{ '/images/art/web/' | append: piece.file | append: '.jpg' | relative_url }}" class="art-gallery__link" data-title="{{ piece.title | escape }}" data-medium="{{ piece.medium | escape }}">
      <img src="{{ '/images/art/web/' | append: piece.file | append: '-thumb.jpg' | relative_url }}" alt="{{ piece.title | escape }} ({{ piece.medium | downcase }})" loading="lazy">
    </a>
    <figcaption><span class="art-gallery__title">{{ piece.title }}</span> · {{ piece.medium }}</figcaption>
  </figure>
{% endfor %}
</div>

<dialog class="art-lightbox" aria-label="Artwork viewer">
  <button type="button" class="art-lightbox__btn art-lightbox__close" aria-label="Close">&times;</button>
  <button type="button" class="art-lightbox__btn art-lightbox__prev" aria-label="Previous">&#8249;</button>
  <figure>
    <img alt="">
    <figcaption></figcaption>
  </figure>
  <button type="button" class="art-lightbox__btn art-lightbox__next" aria-label="Next">&#8250;</button>
</dialog>

<script>
  // Lightbox: click a piece to view it large; arrows / ← → to move, Esc or click outside to close.
  // Without JS (or <dialog> support) the links simply open the full-size image.
  (function () {
    var dialog = document.querySelector(".art-lightbox");
    if (!dialog || typeof dialog.showModal !== "function") return;
    var links = Array.prototype.slice.call(document.querySelectorAll(".art-gallery__link"));
    var img = dialog.querySelector("img");
    var caption = dialog.querySelector("figcaption");
    var current = 0;

    function show(i) {
      current = (i + links.length) % links.length;
      var link = links[current];
      img.src = link.href;
      img.alt = link.dataset.title;
      caption.textContent = link.dataset.title + " · " + link.dataset.medium;
    }

    links.forEach(function (link, i) {
      link.addEventListener("click", function (e) {
        e.preventDefault();
        show(i);
        dialog.showModal();
      });
    });
    dialog.querySelector(".art-lightbox__close").addEventListener("click", function () { dialog.close(); });
    dialog.querySelector(".art-lightbox__prev").addEventListener("click", function () { show(current - 1); });
    dialog.querySelector(".art-lightbox__next").addEventListener("click", function () { show(current + 1); });
    dialog.addEventListener("click", function (e) { if (e.target === dialog) dialog.close(); });
    dialog.addEventListener("keydown", function (e) {
      if (e.key === "ArrowLeft") show(current - 1);
      if (e.key === "ArrowRight") show(current + 1);
    });
  })();
</script>
