# REFLEXION.md : à compléter

1. `robots.txt` empêche-t-il, à lui seul, le duplicate content entre
   `/produits?tri=prix` et `/produits?tri=prix-asc` ? Pourquoi ?
   Non car robots.txt sert uniquement à bloquer l'exploration, pas l'indexation.

2. Pourquoi la balise canonique est-elle l'outil adapté ici, plutôt que
   `robots.txt` ou une meta `noindex` ?
   La balise canonique indique à Google la version maîtresse de la page. robots.txt bloque le crawl 
   et noindex fait disparaître la page de l'index.

3. Si demain `/admin` existe sur ce site et ne doit jamais être exploré par
   Google, quelle ligne ajoutes-tu dans `robots.txt` ?
   Il faut ajouter la ligne d'interdiction "Disallow: /admin/"