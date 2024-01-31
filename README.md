# Tp-snake_POO

#Explication du code

1. Importation des bibliothèques :
   Donc,d'abord,le programme commence par importer les bibliothèques nécessaires, notamment `java.util.Random` pour générer des nombres aléatoires et les classes JavaFX pour l'interface utilisateur.

2. Définition de la classe principale :
   La classe principale `SnakeApp` est définie, et elle étend la classe `Application` de JavaFX, indiquant que c'est une application graphique.

3. Déclaration des variables :
   Plusieurs variables sont déclarées pour gérer différents aspects du jeu, telles que la position du serpent, la direction, les rectangles représentant le serpent, etc.

4. Méthode pour initialiser un rectangle :
   Une méthode `initRect` est définie pour créer et configurer un rectangle avec une taille spécifique, une couleur noire, et le rendre invisible.

5. Méthode de démarrage de l'application :
   La méthode `start` est la méthode principale appelée lors du lancement de l'application. Elle configure la scène, initialise les éléments du jeu, et démarre le thread du jeu.

6. Initialisation de la position de la tête du serpent et démarrage du thread du jeu :
   La position initiale de la tête du serpent est définie, et un thread est lancé pour gérer le déplacement du serpent, la détection de collisions, et d'autres aspects du jeu.

7. Gestion des touches clavier :
   La méthode `setOnKeyPressed` est utilisée pour détecter les touches du clavier (D, A, S, W) et ajuster la direction du serpent en conséquence.

8. Définition de la scène et affichage de la fenêtre :
   La scène est créée avec un conteneur racine, et la fenêtre graphique est configurée avec un titre, une taille minimale et maximale. Enfin, la fenêtre est affichée.

9. Méthode de déplacement du serpent :
   La méthode `move` gère le déplacement du serpent en fonction de la direction, détecte les collisions avec la nourriture, les bords et le serpent lui-même, met à jour l'affichage, etc.

10. Vérification des collisions :
    La méthode `intersects` est utilisée pour vérifier si la tête du serpent entre en collision avec son propre corps.

11. Lancement de l'application :
    La méthode `main` lance l'application JavaFX en appelant `launch(args)`.

Ce code crée un jeu Snake simple en utilisant JavaFX avec une interface utilisateur graphique. Pour lancer le programme, exécutez la méthode `main`.

Le code représente une implémentation du jeu Snake en JavaFX. Il crée une fenêtre graphique où un serpent, composé de rectangles, peut être contrôlé par l'utilisateur à l'aide des touches directionnelles. Le serpent se déplace périodiquement dans une direction, et le but du jeu est de manger la nourriture représentée par un autre rectangle. Lorsque le serpent mange la nourriture, il grandit, augmentant ainsi la longueur du serpent. Le jeu se termine si le serpent entre en collision avec lui-même. Le code utilise un thread pour mettre à jour en continu la position du serpent. La méthode `intersects` vérifie les collisions entre la tête du serpent et le reste de son corps. L'ensemble du code est encapsulé dans une classe JavaFX, avec la méthode `start` initialisant l'interface graphique et les événements clavier. La méthode `main` lance l'application. Pour exécuter le programme, je dois compiler et exécuter la classe principale.

#Comment lancer mon programme.

Pour lancer le programme Snake, vous devez suivre ces étapes simples. 
Effectivement, j'ai ajouté une information dans les instructions indiquant que le serpent grandit au fur et à mesure qu'il mange le pixel. Vous pouvez consulter la version mise à jour ci-dessous :

- Prérequis :
  Vous devez avoir un environnement de développement Java installé sur votre machine.

- Copiez le code source :
  Copiez le code Java fourni dans un fichier avec l'extension ".java", par exemple, "SnakeApp.java".

- Ouvrez l'invite de commande/terminal :
  Ouvrez une invite de commande ou un terminal dans le répertoire contenant le fichier source.

- **Compilation :**
  Compilez le code en utilisant la commande "javac SnakeApp.java". Cela générera les fichiers compilés ".class".

- Exécution du programme :
  Enfin,vous devez exécuter le programme en utilisant la commande "java SnakeApp". Une fenêtre s'ouvrira alors,vous aller voir afficher le jeu Snake.

- Touches de contrôle :
 Afin vous puisssez déplacer le serpent,vous devez utiliser les touches suivantes pour 
  - D : Déplacer vers la droite
  - A : Déplacer vers la gauche
  - S : Déplacer vers le bas
  - W : Déplacer vers le haut

- Interaction avec le jeu :
  A noter que vous devez eviter de faire entrer le serpent en collision avec lui-même ou sinon la partie se termine.
  Aussi,le serpent grandit au fur et à mesure qu'il mange le pixel.

- Note importante :
  Assurez-vous de ne pas fermer brusquement la fenêtre, car cela pourrait provoquer des erreurs.
