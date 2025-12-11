---
layout: page
title: 
permalink: photos/
no_footer: true
---

<div class="photo-grid l-page" style="display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:1rem;align-items:start;">
  {% assign gallery = site.static_files | where_exp: "file", "file.path contains '/images/gallery/'" | sort: 'path' %}
  {% for file in gallery %}
    <a class="flip-card" href="{{ file.path | relative_url }}" style="display:block;">
      <div class="flip-inner">
        <div class="flip-front">
          <img src="{{ file.path | relative_url }}" alt="" style="width:100%;height:auto;display:block;border-radius:0.5rem;">
        </div>
        {% assign meta = site.data.gallery[file.name] %}
        <div class="flip-back">
          {% if meta and meta.caption %}
            {{ meta.caption }}
          {% else %}
            
          {% endif %}
        </div>
      </div>
    </a>
  {% endfor %}
</div>

<script>
document.addEventListener('DOMContentLoaded', function(){
  document.querySelectorAll('.photo-grid img').forEach(function(img){
    function mark(){
      var w = img.naturalWidth, h = img.naturalHeight;
      if (w && h && (w / h) > 1.2) {
        var card = img.closest('.flip-card');
        if (card) card.classList.add('landscape');
      }
    }
    if (img.complete) mark(); else img.addEventListener('load', mark);
  });
});
</script>
