{% assign current = page.url | remove: 'index.html' | remove: '.html' %}

{% unless current == "/" or current == "" %}
- [Accueil]({{ '/' | relative_url }})
{% endunless %}

{% unless current == "/Chats/pelage" %}
- [Le Pelage]({{ '/Chats/pelage' | relative_url }})
{% endunless %}

{% unless current == "/Chats/Taille" %}
- [La Taille]({{ '/Chats/Taille' | relative_url }})
{% endunless %}

{% unless current == "/Chats/Charactère" %}
- [Le Caractère]({{ '/Chats/Charactère' | relative_url }})
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
