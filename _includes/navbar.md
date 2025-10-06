{% assign current = page.url | remove: 'index.html' | remove: '.html' %}

{% unless current == "/" or current == "" %}
- [Accueil]({{ '/' | relative_url }})
{% endunless %}

{% unless current == "/Chats/Pelage" %}
- [Le Pelage]({{ '/Chats/Pelage' | relative_url }})
{% endunless %}

{% unless current == "/Chats/Taille" %}
- [La Taille]({{ '/Chats/Taille' | relative_url }})
{% endunless %}

{% unless current == "/Chats/Caractère" %}
- [Le Caractère]({{ '/Chats/Caractère' | relative_url }})
{% endunless %}

{% unless current == "/Chats/Toilette" %}
- [La Toilette]({{ '/Chats/Toilette' | relative_url }})
{% endunless %}

{% unless current == "/Chats/Adoption" %}
- [Adoption]({{ '/Chats/Adoption' | relative_url }})
{% endunless %}

{% unless current == "/Chats/VIP" %}
- [Le Cartel des Ronrons]({{ '/Chats/VIP' | relative_url }})
{% endunless %}
