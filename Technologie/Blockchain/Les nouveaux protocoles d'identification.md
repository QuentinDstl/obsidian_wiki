L'intérêt grandissant du public pour la blockchain a mit la lumière sur la DeFi, permettant alors à tout l'écosystème décentralisé d'attirer plus de développeur avec une dose de nouveauté et de problème.  
  
Les transactions étants à la racine du projet, elles se sont vu être revisitées de nombreuses fois afin d'assurer leurs sécurités. Ainsi, nous nous intéresserons dans cet article à cette interaction entre deux agents et plus particulièrement à l'identification de l'un par rapport à l'autre.  
  
Que cela soit à la connexion à un portefeuille custodial ou lors d'un consensus dans une blockchain sans permission, il sera nécessaire pour n'importe quel acteur de pouvoir prouver son identité à un moment donné.  
  
Le protocole d'identification le plus répandu est l'authentification par mot de passe (unique ou pas) et bien qu'usuel, c'est de loin le moins sécurisé et c'est principalement à sa simplicité qu'il doit son utilisation bien trop fréquente.  
  
Aujourd'hui, de nombreux protocoles viennent s'ajouter à la liste, avec chacun des avantages et des inconvénients. On peut par exemple y retrouver OAuth2 qui, nécessite un serveur de ressources externes (conf. [RFC6749](https://www.rfc-editor.org/rfc/rfc6749.html#section-1.1)) pour fournir l'autorisation ce qui renforce la sécurité. D'un autre côté, dans le cas d'OAuth2 le _"bearer"_ token (conf. [RFC6750](https://www.rfc-editor.org/rfc/rfc6750)) n'est pas lié au client (_sender constraining_) à la différence d'un PoP (Proof of Possession) classique et donc ne profite pas de la _"confirmation méthode (cnf)"_ (conf. [RFC7800](https://www.rfc-editor.org/rfc/rfc7800.html#section-3.1)).

Ainsi, chaque protocole d'authentification et/ou d'identification est propre à une situation spécifique. Dans le cas de la blockchain et de la DeFi un type de protocole en particulier a attiré mon attention, les ZK proof (pour zero knowledge).


https://cointelegraph.com/news/how-does-zero-knowledge-proof-authentication-help-create-a-portable-digital-identity-solution


explication :

https://www.bibmath.net/crypto/index.php?action=affiche&quoi=moderne/identification#:~:text=L'identification%20par%20mot%20de%20passe%20peut%20aussi%20se%20faire,personne%20est%20(empreintes%20digitales).

webid oidc 

Zero knowledge protocol
==================================
_ZKIP_ pour **Zero Knowledge Interactive proof**
_non-interactive zero-knowledge proof_
_zk-snark_ pour zero-knowledge Succinct Non-interactive Argument of Knowledge
zk-stark
> https://academy.binance.com/en/articles/zk-snarks-and-zk-starks-explained

Solid pod protocol

Masa Finance : protocole d'identité décentralisé