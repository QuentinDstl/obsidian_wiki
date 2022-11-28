L'intérêt grandissant du public pour la blockchain a mit la lumière sur la DeFi, permettant alors à tout l'écosystème décentralisé d'attirer plus de développeurs. C'est à travers leurs innovations que le système s'est compléxifié, apportant de nouvelles problématiques.  
  
Les transactions étants à la racine de cette technologie, elles se sont vues être revisitées de nombreuses fois afin d'assurer leurs sécurisations. Ainsi, nous nous intéresserons dans cet article à l'interaction entre deux agents et plus particulièrement à l'identification de l'un par rapport à l'autre.  
  
Que cela soit pour la connexion à un portefeuille custodial ou lors d'un consensus dans une blockchain sans permission, il sera nécessaire pour n'importe quel acteur de pouvoir prouver son identité à un moment donné.  
  
Le protocole d'identification le plus répendu est l'authentification par mot de passe (unique ou pas), solution peu sécurisée mais simple d"application.
  
Aujourd'hui, de nombreux protocoles viennent s'ajouter à la liste, avec pour chacun, des avantages et des inconvénients. On peut par exemple y retrouver OAuth2 qui nécessite un serveur de ressources externes (conf. [RFC6749](https://www.rfc-editor.org/rfc/rfc6749.html#section-1.1)) pour fournir l'autorisation, ce qui renforce la sécurité. D'un autre côté, dans le cas d'OAuth2 le _"bearer"_ token (conf. [RFC6750](https://www.rfc-editor.org/rfc/rfc6750)) n'est pas lié au client (_sender constraining_) à la différence d'un PoP (Proof of Possession) classique et donc ne profite pas de la _"confirmation method (cnf)"_ (conf. [RFC7800](https://www.rfc-editor.org/rfc/rfc7800.html#section-3.1)).

Ainsi, chaque protocole d'authentification et/ou d'identification est propre à une situation spécifique. Dans le cas de la blockchain et de la DeFi un type de protocole en particulier a attiré mon attention, les ZK proof (pour zero knowledge) utilisé notamment pour les rollups dans la blockchain Ethereum.

Un rollup est un processus (conf. [zk proof avec ethereum](https://ethereum.org/en/zero-knowledge-proofs/)) propre au layer 2 Ethereum qui permet de réduire les temps et les ressources (dont frais de transaction) allouées aux transactions sur la blockchain. 

C’est ainsi qu’en plus d’exporter une partie du calcul et des validations en dehors de la chaîne, les informations conservées sur la chaîne sont compressées pour diminuer leur taille ainsi que les gas-fees associés. Les transactions sont exécutées à l'extérieur de la chaîne, seuls les résultats de calcul et validations y sont ajoutés après avoir été compressés, rectifiant ainsi la scalabilité (conf. [layer 2 scaling](https://ethereum.org/en/developers/docs/scaling/)) du réseau.

Cette application précise est bien loin de notre problème d'identification, mais nous y reviendrons. Ainsi, lorsqu'un nœud exécute une transaction en dehors d'Ethereum, il soumet une preuve de validité qui garantit grâce au ZK proof la légitimité de l'opération.

Commencons par expliquer la logique derrière le concepte de Zero Knowlege Proof.

Théorisé en 1985, il n'est loin d'être considéré comme une nouveauté. C'est cependant, les protocoles qui en découlent qui innovent de part leurs ...

StarkNet : "StarkNet is a permissionless decentralized Validity-Rollup (often referred to as ZK-Rollup). It operates as an L2 network over Ethereum, enabling any dApp to achieve unlimited scale for its computation – without compromising Ethereum's composability and security."

https://cointelegraph.com/news/how-does-zero-knowledge-proof-authentication-help-create-a-portable-digital-identity-solution


explication :

https://www.bibmath.net/crypto/index.php?action=affiche&quoi=moderne/identification#:~:text=L'identification%20par%20mot%20de%20passe%20peut%20aussi%20se%20faire,personne%20est%20(empreintes%20digitales).

webid oidc 

Zero knowledge protocol
==================================
_ZKIP_ pour **Zero Knowledge Interactive proof**
_non-interactive zero-knowledge proof_
_zk-snark_ pour zero-knowledge Succinct Non-interactive Argument of Knowledge
zk-stark pour s zero-knowledge succinct transparent argument of knowledge
> https://academy.binance.com/en/articles/zk-snarks-and-zk-starks-explained

Solid pod protocol

Masa Finance : protocole d'identité décentralisé

---

>  1 token ≠ 1 action !

Ca c'est dit ! Pour tous ceux qui ne l'avaient pas encore compris... Maintenant, je pense qu'on peut entrer dans les détails du sujet sur de meilleures bases. 😄

  

Aujourd’hui, l’émergence des cryptomonnaies, les sommes levées par certaines ICO et l’effet de mode de la technologie Blockchain peuvent donner envie à certains entrepreneurs de privilégier une ICO (Initial Coin Offering)  plutôt qu’une levée de fonds classique (IPO : Initial Public Offering).

❓Mais dans quelle situation ce choix est-il réellement pertinent et dans quel cas ne l’est-il pas ?

  

C’est dans le cadre de ma formation sur les technologies Blockchain dispensée en majeur Objets Connectés, Réseaux et Services à l’ECE Paris qu’il m’a été demandé de réfléchir à un sujet lié à la technologie Blockchain. De par mon appétence pour l’entrepreneuriat, il m’a été naturel de tenter de répondre à la question que de nombreux entrepreneurs se posent aujourd’hui : « alors, IPO ou ICO pour ma levée de fonds ? 🧐 »

💡Pour réaliser ce travail, je me suis également inspiré des mots de Clément Jeanneau, ex-CEO d’ICO Mentor, dont je vous conseille de suivre le [contenu super intéressant sur Youtube](https://www.youtube.com/results?search_query=cl%C3%A9ment+jeanneau) !

Pour revenir à notre problématique, il n’y a pas de bonne ou de mauvaise réponse à cette question ni de type de levée de fonds qui fait gagner plus d’argent que l’autre à la startup. Tout dépend du modèle économique choisi par la boîte.

🧠 Pour comprendre la nuance, il faut rappeler qu’une ICO, au contraire d’une IPO classique, ne permet pas aux actionnaires de prendre des parts de l’entreprise. L’ICO émet en réalité des tokens qui vont répartir la valeur de la solution délivrée par l’entreprise entre les investisseurs.

Heeeu… un exemple peut-être ?? 😅

Effectivement, ce sera plus simple pour comprendre. Prenons l’exemple de Storge ! Cette entreprise fondée en 2014 voulait exploiter les espaces de mémoire restants dans les ordinateurs de chacun des particuliers. Et pour que les utilisateurs acceptent de mettre à dispo leur espace de mémoire, il leur fallait une récompense… de la thune quoi ! … D’où les tokens ! 🤑

  

Ainsi, les investisseurs présents au début du projet pouvaient acheter de l’espace de stockage à prix faible auprès de nouvelles personnes souhaitant entrer dans le projet ou bien spéculer puis revendre leurs tokens ayant pris entre temps de la valeur ! 🕶️

Le fonctionnement d'un tel système se base sur les tokens achetés par les clients contre de la cryptomonnaie. Les transactions sont quant à elles enregistrées sur une Blockchain qui les rend infalsifiables. (Enfin en théorie mais ce n’est pas notre sujet d’aujourd’hui …)

  

📝 Pour synthétiser, il est important de comprendre que la différence entre une ICO et une IPO réside dans le type d'acquisition de l'investisseur :

-   Dans le cadre d'une ICO, un investisseur est propriétaire d'une partie de la valeur de la solution.
-   Dans le cadre d'une IPO, un investisseur est propriétaire d'une partie de la valeur de l'entreprise.


Ainsi, l'actionnaire, suite à une IPO, prend part aux décisions de l'entreprise et intègre le comité de direction. Concernant les actions des investisseurs, elles sont centralisées et ce même comité de direction en prend la responsabilité.

Au contraire, un investisseur ayant acheté des tokens n'a pas de visibilité sur l'évolution de l'entreprise mais la décentralisation lui assure la valeur de sa propriété. En effet, la décentralisation permet d’assurer aux détenteurs de tokens que l’entreprise ne va pas soudainement en créer de nouveau et diminuer drastiquement la valeur des tokens qu’ils possèdent. Cela crée une véritable économie entre les utilisateurs ! 🔄️

En conséquence, si la société utilise au cœur de la solution qu’elle délivre à ses clients des tokens, alors, l’ICO sera très intéressante ! En effet, les investisseurs seront les premiers utilisateurs et feront tout pour créer la boucle de viralité dont a besoin la startup pour grossir très vite. 🔝

En revanche, une ICO réalisée par un projet n’utilisant pas de tokens pour répartir la valeur du produit entre ses utilisateurs ne fait pas sens et sera certainement contre-productive. Les investisseurs ayant acheté des tokens ne parviendront pas à les échanger et le token ne prendra pas de valeur… Et ceci même si la solution plaît à son marché ! ❌🚫❌

Pour conclure, dorénavant, si je devais conseiller quelqu’un qui s’interroge entre ICO et IPO, je lui dirais :

_Pas de décentralisation, pas d’ICO !!!_ 😉