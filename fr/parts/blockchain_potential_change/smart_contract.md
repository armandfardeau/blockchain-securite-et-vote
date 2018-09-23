## Qu'est ce que les smart contracts?
---

### Principe 

La blockchain Ethereum dispose d'une capacité singulière vis à vis des autres blockchains,
Elle peut ètre programmée à l'aide d'un langage spécifique : Solidity. c’est un langage de programmation « complet » ( turing-complete ), plus précisement il permet d’exécuter l’ensemble des fonctions utilisés pour développer une application moderne. 

Cela permet de programmer des engagements sur la blockchain Ethereum. Ceux ci peuvent simple, comme engager une transaction ou plus complexe, car constitué de plusieurs actions en série ou parrallèle. 

Lorsque les conditions d’exécution de ces engagements sont réunies, ces contrats s’exécutent automatiquement sur la blockchain, en prenant en compte l’ensemble des conditions et des limitations programmés à l’origine.

Un contrat de prestation de service entre deux entitées peut aisément se modéliser sous la forme d'un smart-contract.

La première souhaite rémunerer la seconde en paiement de la prestation, ce contrat erst formalisé dans la blochain Ehthereum par la création d'un engagement de type smart-contract. La somme correspondante est alors mise en gage sur la blockchain, lorsque la prestation est réalisée, l'engagegement vérifie automatiquement que les conditions fixées ont bien été remplies et le cas échéant, verse la somme gagée. En cas de manquement aux stipulations du contrat, la partie gageante se voit restituer la somme.

les transactions effectuées sont publiques, il s'agit du principe du publicité. La bonne exécution du contrat peut ainsi ètre vérifié, n’importe quelle partie qui dispose du code source du contrat peut vérifier que le contrat a bien été enregistré.

La blockchain prodigue une sécurité élevée, l'une de ses limites est la vulnérabilité à l'attaque des 51%. Voir [sécurité de la blockchain](./blockchain_securite.md/).

Les données qui sont enregistrées dans la blockchain y sont enregistrées de ma,ière immuable : l’historique est conservé depuis l’origine. Un engagement est irrémédiablement enregistré dans la blockchain.

Mettre hors ligne une blockchain nécessiterait d'arréter simultanément tous les noeuds de celle-ci, c'est virtuelllement impossible. C'est un système que l'on peut considérer comme fiable.

En résumé les smart-contrats permettent d'engager des accorfs envers deux parties sans que l'une ne puissent entraver son exécution, mais également des applications décentralisées.

### Limites

Se pose alors la question de la validation des conditions d'executions, pour cela deux possibilités :

* Condition d'exécution interne :

    Liées à des écritures dans la blockchain, dès lors le contrat est executé lorsque ces écritures existent et que la date d'exécution est atteinte.

* Condition d'exécution externe : 
   Lorsque les conditions d'executon sont exterieures à la blockchain comme par exemple la réalisation d’une prestation, survenance d’un événement… etc. Dès lors, le recours à un tiers de confiance, appellé  « oracle » auquel est délégué l'écriture des conditions dans la blockchain.

La principale limitation inhérente à la technologie blockchain est la lenteur du réseau, contrepartie de sa sécurité. 

### Dans le cadre du vote : 
Exemple avec l'utilisation d’un service d’Oracle : 

Nécessite un nombre important de participants. Chaque protagoniste vote pour le résultat qu'il juge exact et le résultat est confié au consensus. On peut citer en la matière le projet Oraclize. Dans le cadre du vote cela sous-entend de confier un nombre de propositions au consensus qui détermine les éléments valides.

Une proposition est dans ce cas de figure un smart-contract classique dont les conditions fixent le cadre d'application. Une fois ces conditions validées, le contrat voit son exécution programmée.

Ce système présente une limite nécessite une vigilance particulière, en effet l'interruption du contrat (et donc de l'exécution de la proposition) est en pratique impossible, sauf si cette condition d'intteruption a été prévue dès l'origine.