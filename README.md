# BoPi-HomeAssistant
Vous trouverez dans ce GitHub les informations pour ajouter BoPi dans Home Assistant et pouvoir ainsi contrôler votre piscine comme vous le souhaitez sans avoir besoin de BoPi Cloud et même créer vos propres automatisations selon vos besoins (utilisation de surplus solaire pour la pompe de filtration, thermorégulation personnalisée, mode hors gel personnalisé, ....). 

Pour vous faciliter l'installation de BoPi dans Home Assistant, commencez par connecter BoPi au réseau Wifi et récupérez l'adresse IP de celui-ci en bas du tableau de bord dans l'app :

Je vous recommande ensuite d'installer "File Editor" dans Home Assistant pour vous faciliter la modification des fichiers de configuration. 

Dans le dossier correspondant à votre modèle de BoPi, vous trouverez 3 fichiers : 
  - configuration.yaml : Contiens les appels et commandes Rest pour obtenir les infos et donner des ordres à BoPi.
  - scripts.yaml : Contiens des scripts utilisés dans le tableau de Bord par défaut pour contrôler BoPi.
  - tableaudebord.yaml : Contiens le fichier de configuration d'un tableau de bord vierge destiné à BoPi.

