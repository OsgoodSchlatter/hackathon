# Comment mener à bien un hackathon

Ce site a pour objectif de regrouper toute l'expérience et le savoir acquis durant des épreuves types Hackathons effectuées par des étudiants de Kryptosphere.
Il est voué à servir de point de repère pour toute personne souhaitant se lancer dans cette aventure. 



##  Table des matières 

1. ### Introduction
2. ### Préliminaires
3. ### Pendant le hackathon
4. ### Après le hackathon
5. ###  Historique des hackathons
   
## 1. Introduction 

### 1.1 Définition 
Selon Wikipédia, la définition d'un hackathon est la suivante : "Évènement au cours duquel des spécialistes se réunissent durant plusieurs jours autour d'un projet collaboratif de programmation informatique ou de création numérique."    

### 1.2 Raison d'être
Le résultat d'un hackathon profite tant aux participants qu'à l'organisateur. En effet, l'organisateur par ses cash-prize et autres récompenses attire de nombreux candidats. Mais le travail effectué par ces derniers bénéficie également à l'organisateur. En mettant en compétition différentes équipes, la stimulation n'est que renforcée et aboutit à de nombreux projets pouvant être utiles au développement de la plateforme de l'organisateur. C'est donc un événement où tous les parties ont quelque chose à y gagner.

## 2. Préliminaires 

### 2.1 bien choisir son hackathon  
Avant de participer à un hackathon, il est intéressant de savoir à quoi vous allez avoir à faire. Quel thème, quelle technologie, quel langage, etc... Faire un hackathon sur une virtual machine Ethereum n'a rien à voir avec un hackathon sur Tezos par exemple. Les smart contracts sur les v.m. Ethereum sont écrits en Solidity lorsque les smart contracts de Tezos sont écrits en python à l'aide de la librairie Smartpy. 
Connaître les spécificités du hackathon est donc un atout car cela permet de mieux cibler les attentes par rapport à votre niveau et vos envies. Si l'objectif est d'apprendre, alors autant choisir un hackathon où les outils vous sont inconnus. Au contraire, si vous souhaitez chercher la performance, autant maximiser vos chances et participer à un hackathon qui repose sur des technologies que vous maîtrisez. 
Par ailleurs, ce que vous pouvez tirer de ce hackathon est important. Quelles sont les récompenses, quelle est la renommée de la technologie sur laquelle je travaille, quelle est l'espérance de vie des projets réalisés lors des éditions dernières...
Enfin, il faut aussi que ce dernier corresponde au temps que vous pouvez y allouer. Un hackathon risque d'être assez time-consuming, donc il faut poser les choses au plat avant de le commencer et ne pas y aller tête baissée.  

### 2.2 bien choisir son équipe   
Une fois que vous avez choisi le hackathon de vos rêves, monter une équipe performante et pertinente avec le projet est crucial. Chacun a sa propre façon de développer, ses points forts et points faibles.
Nous allons l'aborder juste après dans *répartition des tâches*, mais si l'équipe ne se compose que de développeurs back-end par exemple, alors le front-end risque d'être négligé et pourrait nuir au projet. Il est important de commencer le hackathon avec une équipe représentant le plus de profils différents. 
De plus, s'entourer de gens qu'on apprécie est évident, mais l'ambiance doit aussi se montrer sérieuse et studieuse la plupart du temps. Il faut savoir se mettre au travail et avancer dans le projet. 
Bien sûr l'équipe ne peut pas être parfaite dès le début, on fait souvent avec ce qu'on a et c'est déjà très bien ;) 

### 2.3 trouver une idée  
Pour trouver une idée, il y a plusieurs façons de faire. Vous pouvez vous réferer à quelqu'un qui a de l'expérience sur la technologie sur laquelle vous allez travailler. Avec le recul, il/elle aura surement les compétences pour vous guider vers un sujet intéressant. Vous pouvez éplucher le site organisateur du hackathon, ils proposent souvent des idées ou du moins les catégories peuvent vous permettre d'affiner votre choix. Ensuite, vous pouvez tout simplement réfléchir entre vous et parvenir par vous mêmes à votre fin

### 2.4 mettre en place un emploi du temps  
L'efficacité est clef dans un hackathon. Il est capital de mettre en place une sorte de road map, de planning qui fixe les échéances dans le temps. Vous pourrez ainsi mesurer votre avancée par rapport à ce que vous êtes fixés en amont. Organiser des calls réguliers ou des meetings pour discuter avec votre équipe est aussi important.

### 2.5 mettre en place un repository GitHub  
Cette étape est inévitable. Que vous soyez seul ou en groupe, vous devrez utiliser un repository GitHub. C'est un endroit ou vous pouvez partager votre code développé en local et le fusionner avec celui des autres sans bavure ni erreur. Si vous êtes seul, il vous sera quand même utile pour rendre votre projet en ligne. 
Cette section est destinée à vous initier aux bonnes pratiques à connaître sur github (avec l'aide de git). Attention à bien différencier git et github. Git est un logiciel de gestion de versions alors que github (mais aussi gitlab par ex) est une sorte de google doc destiné à l'hébergement et la gestion de versions, s'appuyant sur git. 

1. __créer son compte github__    
Avant toute chose rendez vous sur [github.com](https://github.com/) et créer votre compte.

2. __créer une organisation et un repository__  

Une fois votre compte crée, allez sur votre profil et créez une organisation. Une organisation vous permet de travailler à plusieurs, ce qui va être intéressant dans notre cas. Ajoutez également les comptes github de vos collègues. Vous pouvez maintenant créer un repository pour commencer votre travail. Souvent on différe le repo utilisé pour le front de celui utilisé pour les smart contracts par ex. 

3. __le connecter à votre dépôt local__    
Créer un répertoire de travail en local `mkdir nom_du_depot` et dirigez-vous à l'intérieur. Vous pouvez ensuite faire ` git init` puis `git remote add origin https://github.com/votre_organisation/votre_repo.git` pour lier votre repository de votre organisation sur github à votre dépôt en local. Autrement, sans passer par les deux commandes précédentes, vous pouvez `git clone https://github.com/votre_organisation/votre_repo.git` dans un dossier et votre dépôt s'effectuera. 

4. __faire son premier commit__  
Ensuite, vous pouvez créer un fichier en local, votre premier code : `contract.sol` par ex. Vous y inscrivez quelques lignes de codes. Pour le mettre en ligne sur le repo, faîtes d'abord `git add contract.sol`. Vous pouvez en ajouter plusieurs de cette manière. Ce fichier est donc "suivi", "indexé". Maintenant, vous pouvez réaliser votre premier commit, qui est l'empaquetage en quelque sorte de tous les fichiers que vous voulez pousser sur le repo github. `git commit -m "message qui décrit votre commit"`. Puis vous poussez : `git push `. Il y a bien sûr plein de cas de figures particuliers que l'on abordera au fur et à mesure, mais voici le "happy path" de git. Pour récupérer les données sur le repo à distance, faîtes `git pull`.  

5. __ressources pour continuer à s'entraîner sur git__  
[git_ressource_1](https://www.labri.fr/perso/renault/working/teaching/projets/git.php)   
[learn_git](https://learngitbranching.js.org/?locale=fr_FR)

## 3. Pendant le Hackathon.

### 3.1 Développement du code  
Le développement du code est la partie la plus dure. Il y a souvent 3 grandes étapes : le front, le back et connecter les deux. Sur les Dapp s'ajoute souvent les smart contracts qui PEUVENT remplacer le back mais back != smart contracts. Ces 3 grandes étapes se font souvent de concert. 
#### librairie 
Vous pouvez vous aider de nombreuses librairies en ligne reliées aux différentes blockchains par ex qui expliquent comment mener à bien le développement d'une Dapp par ex. Une myriade de ressource existe aussi sur youtube à travers des tutos etc.
Voici quelques ressources : 
- solidity (langage pour coder des smart contracts pour des Ethereum Virtual Machine) 
1. [solidity_docs](https://docs.soliditylang.org/en/v0.8.11/)
2. [cryptozombies](https://cryptozombies.io/fr/)
3. [buildspace](https://buildspace.so/) nécessite quelques connaissances en solidity
- smartpy (librairie python pour Tezos) 
1. [smartpy_docs](https://smartpy.io/docs/)
2. [cryptoverse_wars](https://cryptocodeschool.in/tezos/)


#### debugging 
Vous allez forcément rencontrer des difficultés pendant votre code, des choses qui à vos yeux devraient fonctionner et qui ne fonctionnent pas. Servez vous d'internet et de nombreux sites types stackoverflow etc sur lesquels bon nombre de vos problèmes ont déjà été résolus. 
#### tests
Tester vos smart contracts est important pour le bon fonctionnement du code. Il arrive très souvent de croire que notre code remplit toutes les conditions qu'on souhaite qu'il remplisse alors qu'il ne fonctionne que pour un cas bien particulier. 

### 3.2 Readme, Roadmap, Whitepaper & Yellowpaper

#### 3.2.1 Readme
Un [readme.md](https://www.ionos.fr/digitalguide/sites-internet/developpement-web/fichier-readme/) est un document, traditionnellement écrit en langage [markdown](https://www.markdownguide.org/getting-started/), qui permet aux personnes inspectant votre projet de comprendre comment interagir avec. Typiquement il regroupe les commandes à entrer dans le terminal si besoin pour lancer votre projet par ex.
#### 3.2.2 Roadmap
Une roadmap est une sorte de ligne de conduite qui définira les prochaines étapes de votre projet.

#### 3.2.3 Whitepaper
Un whitepaper est un papier apportant des informations décrivant le processus de votre projet de manière précise et concise. C'est un readme amélioré qui va inspecter les moindres détails techniques du code. Il est souvent écrit en [latex](https://www.latex-project.org/). 

#### 3.2.4 Yellowpaper


## 4 Anciens hackathons :

### Hashi : Mathis GD et Pierre-Antoine A


### Tezbet : Enguerrand D, Victor L, Jean-François D, Eloi B
