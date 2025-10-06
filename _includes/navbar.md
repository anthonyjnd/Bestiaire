{% assign pages = 
  "/index:Accueil,
/Chats/pelage:Le Pelage,
/Chats/taille:La Taille,
/Chats/charactere:Le Caractère,
/Chats/toilette:La Toilette,
/Chats/adoption:Adoption,
/Chats/VIP:Le Cartel des Ronrons" | split: "," %}

{% assign current = page.url | remove: '.html' %}

{% for item in pages %}
  {% assign parts = item | split: ":" %}
  {% assign url = parts[0] %}
  {% assign name = parts[1] %}
  {% unless current == url %}
  - [{{ name }}]({{ url | relative_url }})
  {% endunless %}
{% endfor %}
