# chatbot-IA
Charles BEUZET  
Corentin BLANCHARD  
  
  ## Sujet
  L'objectif de ce projet est de réaliser un chatbot avec lequel on peut intéragir en lui posant certaines questions.  
  Ce bot répondra aux questions sur des sujets du quotidien que l'on retrouve dans cette base de données : https://www.kaggle.com/kausr25/chatterbotenglish  
    
  ## Implémentation
  
  - Téléchargement des bases de données et stockage sur un drive. Afin de pouvoir jouer avec notre bot, il faut d'abord demander accès à ses bases de données en nous le demandant.  
  - Récupération des questions/réponses de bases pour les stocker dans des tableaux.
  - Préprocessing des questions dans un dictionnaire : 
    - Suppression de la ponctuation.
    - Enlever les majuscules et tout mettre en minuscules.
    - Réduction des mots à leur racine.
  - Création du Bag of Words avec le dictionnaire des mots préprocessés.
  - Vectorisation des questions sous la forme du Bag of Words.
  - Préprocessing/Vectorisation de la question de l'utilisateur sous la forme du Bag of Words.
  - Recherche de la question se rapprochant le plus de la question de l'utilisateur (méthode de calcul utilisé : calcul de la cosine distance).
  - Si plusieurs réponses possibles alors choix aléatoire entre elles.
  - Possibilité de quitter la conversation en envoyant le mot "goodbye".
  
  ## Résultat  
  
  - Le chatbot répond aux questions de l'utilisateur en trouvant la réponse adaptée. (Bag Of Words/Préprocessing/Cosine distance fonctionnels).
  - Les bases de données ne sont pas toutes créées de la même manière ce qui pose problème dans certains cas.
  - Si nous avions eu 1 mois de plus nous nous serions penchés sur l'utilisation de GloVe qui effectue une vectorisation différente.(basé sur les probabilités)
  
  
  
  
  
