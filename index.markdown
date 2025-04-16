---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<style>
.image-button {
  text-decoration: none;
}

.button-content {
  width: 250px;
  height: 140px;
  background-size: cover;
  background-position: center;
  border-radius: 12px;
  position: relative;
  overflow: hidden;
  transition: filter 0.3s ease;
  display: flex;
  align-items: center;
  justify-content: center;
}

.button-content span {
  color: white;
  font-size: 1.3em;
  font-weight: bold;
  text-shadow: 0 0 8px rgba(0, 0, 0, 0.6);
  z-index: 2;
}

.button-content::after {
  content: "";
  position: absolute;
  inset: 0;
  background: rgba(0, 0, 0, 0.25);
  transition: backdrop-filter 0.3s ease, background 0.3s ease;
}

.image-button:hover .button-content {
  filter: blur(2px) brightness(0.8);
}

.image-button:hover .button-content::after {
  backdrop-filter: blur(2px);
  background: rgba(0, 0, 0, 0.4);
}
</style>


---

## Yann Glémarec

Post-doctorate researcher | INRIA Rennes, France | 🔎  [ORCID](https://orcid.org/0000-0003-1717-6048) 

--- 

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin-top: 30px;">

  <a href="{{ '/yannGlemarec.github.io/portfolio/' | relative_url }}" class="image-button">
    <div class="button-content" style="background-image: url('{{ "/pictures/ScannedAvatar.jpg" | relative_url }}');">
      <span>Portfolio</span>
    </div>
  </a>

  <a href="{{ '/yannGlemarec.github.io/about/' | relative_url }}" class="image-button">
    <div class="button-content" style="background-image: url('{{ "/pictures/yann.jpg" | relative_url }}');">
      <span>About Me</span>
    </div>
  </a>

</div>