1/ Lire le livre blanc: https://bitcoin.org/bitcoin.pdf, cherchez une version française si vous avez du mal avec l'anglais. (Mais dans ce cas vous risquez d'avoir du mal avec la Blockchain tout court).

2/ Un arbre de merkle nécessite une paire de hashes pour produire un nouveau hash parent. Il faut donc a absolument que le nombre de transactions qui produiront le Merkle root soit pair.
Comment est géré le cas ou le nombre de transactions dans le Block à valider est impair pour générer un Merlke root ?

Lorsque le nombre de transactions à valider est impair, le dernier noeud es dupliqué et haché avec lui-même.

3/ Dans le réseau bitcoin, Comment un nouveau noeud arrive t'il à retrouver ses pairs et ainsi rejoindre le réseau ? Expliquer le processus avec vos propres mots.

Une personne qui souhaite rejoindre le réseau et contribuer au système Bitcoin télécharge Bitcoin Core. A partir de ce moment, il commence à se synchroniser les uns avec les autres noeuds existants.
Ce processus se répète à chaque nouveau noeud ajouté au réseau.

4/ Pouvez vous nommer au moins une personne qui a ou aurait pu influencer directement ou indirectement la création de Bitcoin par ses travaux (une personne qui n'a pas été nommée dans le cours)?

Hal Finney

5/ Avec vos propres recherches et grâce aux compétences acquises en cours pouvez vous expliquer comment une Blockchain crée un lien entre ses différents Blocks?

Les blocs sont liés entre eux à partir d'un premier bloc de référence (genesis block), de sorte à former une chaîne, la chaîne de blocs.
Le lien se fait par des règles de consensus (horodatage et preuve) définies par le réseau. 

6/ Quelle structure de données informatique peut représenter le mieux cette chaine de Block: https://en.wikipedia.org/wiki/List_of_data_structures ?

2–3–4 tree

7/ Si je souhaite modifier une transaction de 10 bitcoin que j'ai effectué il y a 6 mois en une transaction de 1 Bitcoin, que dois je modifier dans la Blockchain et que dois je mettre en oeuvre pour que cette modification persiste ?
Est ce possible selon vous ?

A mon avis, dans un premier temps serait de retrouver cette transaction dans le bloc dans laquelle elle inscrite.
Par la suite, avoir les ressources nécessaires (puissance matérielle), la faculté à savoir modifier cette transaction qui à été enterinée par un horodatage et une signature électronique.
Quand bien même, cela est possible le contenu de la transaction inscrit dans le block header du merkle root ne sera plus valide et rendrait cela inutile.




