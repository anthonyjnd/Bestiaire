{% assign current = page.url | remove: 'index.html' | remove: '.html' %}

<nav>
  {% unless current == "/" or current == "" %}
    <a href="{{ '/' | relative_url }}">Accueil</a> |
  {% endunless %}
  {% unless current == "/Chats/Pelage" %}
    <a href="{{ '/Chats/Pelage' | relative_url }}">Le Pelage</a> |
  {% endunless %}
  {% unless current == "/Chats/Taille" %}
    <a href="{{ '/Chats/Taille' | relative_url }}">La Taille</a> |
  {% endunless %}
  {% unless current == "/Chats/Caractere" %}
    <a href="{{ '/Chats/Caractere' | relative_url }}">Le Caractère</a> |
  {% endunless %}
  {% unless current == "/Chats/Toilette" %}
    <a href="{{ '/Chats/Toilette' | relative_url }}">La Toilette</a> |
  {% endunless %}
  {% unless current == "/Chats/Adoption" %}
    <a href="{{ '/Chats/Adoption' | relative_url }}">Adoption</a> |
  {% endunless %}
  {% unless current == "/Chats/VIP" %}
    <a href="{{ '/Chats/VIP' | relative_url }}">Le Cartel des Ronrons</a>
  {% endunless %}
</nav>
