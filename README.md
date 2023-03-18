# Collision

# Collision

Suite au poste que j'ai déjà fais pour expliquer un peu mon projet de base qui ce situe ici ==> https://instant-hack.to/threads/génération-bitcoin.220062/

Le projet avance très bien et des test ont été effectuer sans sucés d’ailleurs puis au fil du temps bien meilleur.

Je tiens à signaler que ce projet m'as couter un PC en grillant tout en poussant trop la capacité de mon programme.

Aujourd'hui les test sont effectués sur un i9 avec geforce gtx 1660 (c'est pas super ouf mais déjà de bon résultats)

Je commencerais donc par l'algorithme de hachage pré-calculé pour la recherche de collision Bitcoin qui est conçu en utilisant C++ et Python pour permettre une utilisation efficace de la mémoire, une implémentation rapide et une flexibilité dans l'écriture de l'algorithme. L'algorithme stock les résultats de hachage RIPEMD-160 de toutes les clés publiques possibles pour un accès rapide. Il utiliserait des techniques d'optimisation telles que la parallélisation, le multithreading, le GPU, la mise en cache, la précharge et la pré-lecture pour accélérer les opérations de hachage et de recherche. Cet algorithme est de loin plus performant que les implémentations actuelles sur GitHub - JeanLucPons/BTCCollider: Generate BTC address pair that share the same prefix en réduisant considérablement le temps de calcul nécessaire (12.3 x moins) pour effectuer des opérations de hachage fréquentes ce qui est énorme.

Le programme est écrit en C++ et Python pour permettre une utilisation efficace de la mémoire, une implémentation rapide et une souplesse dans l'écriture de l'algorithme. Il serait conçu pour générer des adresses Bitcoin avec des patterns de 20 caractères hexadécimaux en utilisant une méthode de recherche de collision. Le but serait de trouver une paire de clés privées qui ont la même adresse Bitcoin, ce qui permettrait de récupérer les Bitcoins stockés à cette adresse.

Le programme commence par générer une clé privée aléatoire à l'aide de la bibliothèque OpenSSL entre Python et C++ en utilisant un générateur de nombres pseudo-aléatoires cryptographiquement sécurisé. Ensuite, il calcule l'adresse Bitcoin correspondante en utilisant la bibliothèque pybitcointools et une autre C++ en convertissant la clé privée en clé publique, en hachant la clé publique avec SHA-256, puis en hachant le résultat avec RIPEMD-160.

Le programme utilise ensuite une méthode de recherche de collision pour trouver une autre clé privée qui a la même adresse Bitcoin. Une méthode courante pour cela est la marche aléatoire. Le programme commence par choisir une clé privée aléatoire et générer une adresse Bitcoin correspondante. Ensuite, il effectue une série de marches aléatoires en modifiant la clé privée d'une petite quantité à chaque étape et en vérifiant si l'adresse Bitcoin correspondante est la même que celle de la clé privée initiale.

Comparaison avec BTCCollider : Le programme que nous avons développé (et oui je suis pas seul) est plus rapide que BTCCollider car nous avons utilisé des algorithmes de recherche avancés et des bibliothèques externes pour améliorer les performances. En outre, notre programme est écrit en C++ et Python, ce qui lui permet d'exploiter pleinement les avantages des deux langages. Nous avons également optimisé notre programme pour maximiser l'utilisation des ressources du système, ce qui lui permet de fonctionner de manière plus rapide et plus efficace.

Les premiers test comme dis dessus m’ont griller un pc pour avoir été trop gourmand.
