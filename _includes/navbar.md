{% assign current = page.url | remove: 'index.html' | remove: '.html' %}

{% unless current == "/" %}
- [Accueil](/)
{% endunless %}

{% unless current == "Chats/pelage" %}
- [Le Pelage](Chats/Pelage)
{% endunless %}

{% unless current == "/Chats/Taille" %}
- [La Taille](/Chats/Taille)
{% endunless %}

{% unless current == "/Chats/Charactère" %}
- [Le Caractère](/Chats/Charactère)
{% endunless %}

{% unless current == "/Chats/Toilette" %}
- [La Toilette](/Chats/Toilette)
{% endunless %}

{% unless current == "/Chats/Adoption" %}
- [Adoption](Chats/Adoption)
{% endunless %}

{% unless current == "Chats/VIP" %}
- [Le Cartel des Ronrons](Chats/VIP)
{% endunless %}
