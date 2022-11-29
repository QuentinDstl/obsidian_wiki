L'intérêt grandissant du public pour la blockchain a mit la lumière sur la DeFi, permettant alors à tout l'écosystème décentralisé d'attirer plus de développeurs. C'est à travers leurs innovations que le système s'est compléxifié, apportant de nouvelles problématiques.  
  
Les transactions étants à la racine de cette technologie, elles se sont vues être revisitées de nombreuses fois afin d'assurer leurs sécurisations. Ainsi, nous nous intéresserons dans cet article à l'interaction entre deux agents et plus particulièrement à l'identification de l'un par rapport à l'autre.  
  
Que cela soit pour la connexion à un portefeuille custodial ou lors d'un consensus dans une blockchain sans permission, il sera nécessaire pour n'importe quel acteur de pouvoir prouver son identité à un moment donné.  
  
Le protocole d'identification le plus répendu est l'authentification par mot de passe (unique ou pas), solution peu sécurisée mais simple d"application.
  
Aujourd'hui, de nombreux protocoles viennent s'ajouter à la liste, avec pour chacun, des avantages et des inconvénients. On peut par exemple y retrouver OAuth2 qui nécessite un serveur de ressources externes (conf. [RFC6749](https://www.rfc-editor.org/rfc/rfc6749.html#section-1.1)) pour fournir l'autorisation, ce qui renforce la sécurité. D'un autre côté, dans le cas d'OAuth2 le _"bearer"_ token (conf. [RFC6750](https://www.rfc-editor.org/rfc/rfc6750)) n'est pas lié au client (_sender constraining_) à la différence d'un PoP (Proof of Possession) classique et donc ne profite pas de la _"confirmation method (cnf)"_ (conf. [RFC7800](https://www.rfc-editor.org/rfc/rfc7800.html#section-3.1)).

Ainsi, chaque protocole d'authentification et/ou d'identification est propre à une situation spécifique. Dans le cas de la blockchain et de la DeFi un type de protocole en particulier a attiré mon attention, les ZK proof (pour zero knowledge) utilisé notamment pour les rollups dans la blockchain Ethereum.

Un rollup est un processus (conf. [zk proof avec ethereum](https://ethereum.org/en/zero-knowledge-proofs/)) propre au layer 2 Ethereum qui permet de réduire les temps et les ressources (dont frais de transaction) allouées aux transactions sur la blockchain. 

C’est ainsi qu’en plus d’exporter une partie du calcul et des validations en dehors de la chaîne, les informations conservées sur la chaîne sont compressées pour diminuer leur taille ainsi que les gas-fees associés. Les transactions sont exécutées à l'extérieur de la chaîne, seuls les résultats de calcul et validations y sont ajoutés après avoir été compressés, rectifiant ainsi la scalabilité (conf. [layer 2 scaling](https://ethereum.org/en/developers/docs/scaling/)) du réseau.

Cette application précise est bien loin de notre problème d'identification, mais nous y reviendrons. Ainsi, lorsqu'un nœud exécute une transaction en dehors d'Ethereum, il soumet une preuve de validité qui garantit grâce au ZK proof la légitimité de l'opération.

Commençons par expliquer la logique derrière le concept de Zero Knowlege Proof en trouvant une réponse à la question : comment prouver que j'ai une information sans avoir à la divulguer ? Un exemple simple est concret est celui de ["la grotte d'ali baba"](https://fr.wikipedia.org/wiki/Preuve_%C3%A0_divulgation_nulle_de_connaissance#Exemples) (conf. [article source](https://pages.cs.wisc.edu/~mkowalcz/628.pdf)) qui permet de comprendre le principe généralisé.

Théorisé en 1985, il n'est loin d'être considéré comme une nouveauté. C'est cependant, les protocoles qui en découlent qui innovent de part leurs ...

ZK SNARK
-------------------
→ **Zero-Knowledge Succinct Non-interactive Argument of Knowledge**.
(conf. [PDF](https://arxiv.org/pdf/2202.06877.pdf))

Succinct :
>

Non-interactive :
>

ZK STARK
-------------------
→ **Zero-Knowledge Succinct Transparent Argument of Knowledge**.
(conf. [PDF](https://eprint.iacr.org/2018/046.pdf))

Transparent :
> 

Les ZK-STARK sont "transparents", car ils peuvent fonctionner sans la mise en place d'une chaîne de référence commune (CRS). Au lieu de cela, les ZK-STARK s'appuient sur un caractère aléatoire vérifiable publiquement pour définir les paramètres de génération et de vérification des preuves.

Les ZK-STARK sont également protégés contre les ordinateurs quantiques, tandis que la cryptographie à courbes elliptiques (ECC) utilisée dans les ZK-SNARK est largement considérée comme sensible aux attaques des ordinateurs quantiques. L'inconvénient des ZK-STARKs est qu'elles produisent des preuves de plus grande taille, ce qui est plus coûteux à vérifier sur Ethereum.

```
StarkNet : "StarkNet is a permissionless decentralized Validity-Rollup (often referred to as ZK-Rollup). It operates as an L2 network over Ethereum, enabling any dApp to achieve unlimited scale for its computation – without compromising Ethereum's composability and security."
```

Solid pod protocol : webid oidc 