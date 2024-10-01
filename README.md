# BoPi-HomeAssistant
Vous trouverez dans ce GitHub les informations pour ajouter BoPi dans Home Assistant et pouvoir ainsi contrôler votre piscine comme vous le souhaitez sans avoir besoin de BoPi Cloud et même créer vos propres automatisations selon vos besoins (utilisation de surplus solaire pour la pompe de filtration, thermorégulation personnalisée, mode hors gel personnalisé, ....). 

Pour que cela fonctionne, il fous faut un BoPi que vous pouvez trouver ici : https://meetbopi.com/fr/
<br><br>
<img width="1512" alt="BoPi - HA - TDB BoPi" src="https://github.com/user-attachments/assets/c19474d1-7674-400b-a183-cc03b6d1d36a">
<br><br>
Pour vous faciliter l'installation de BoPi dans Home Assistant, commencez par connecter BoPi au réseau Wifi et récupérez l'adresse IP de celui-ci en bas du tableau de bord dans l'app :
<br><br>
<img width="49%" alt="BoPi - HA - Reglages réseau" src="https://github.com/user-attachments/assets/dabff5f0-27c9-4751-bf1a-9a4ae82c67a8">
<img width="49%" alt="BoPi - HA - Adresse IP" src="https://github.com/user-attachments/assets/18ec3d3e-0935-48a9-8bd2-4b00f8d9e64f">
<br><br>
Je vous recommande ensuite d'installer "File Editor" dans Home Assistant pour vous faciliter la modification des fichiers de configuration. 
<br><br>
<img width="1512" alt="BoPi - HA - Configuration" src="https://github.com/user-attachments/assets/e9009115-d4db-44aa-ac02-ece0f2682f7e">
<br><br>
Dans le dossier correspondant à votre modèle de BoPi, vous trouverez 3 fichiers : 
  - configuration.yaml : Contiens les appels et commandes Rest pour obtenir les infos et donner des ordres à BoPi.
  - scripts.yaml : Contiens des scripts utilisés dans le tableau de Bord par défaut pour contrôler BoPi.
  - tableaudebord.yaml : Contiens le fichier de configuration d'un tableau de bord vierge destiné à BoPi.

Pour faire simple, commencez par ajouter le contenu au fichier configuration.yaml, ensuite il faudra redémarrer HA pour que les changements soient pris en compte. 

<b>PENSEZ A CHANGER L'ADRESSE IP DE BOPI AVANT DE REDEMARRER HA!</b>
<br><br>
<img width="1512" alt="BoPi - HA - Redemarrage" src="https://github.com/user-attachments/assets/f3f6e864-4bbd-4206-9cd8-15a1817d06a8">
<br><br>
Une fois cela fait, si tout se passe bien, vous pourrez voir les entités de BoPi
<br><br>
<img width="1512" alt="BoPi - HA - Entites" src="https://github.com/user-attachments/assets/cdcf9be7-1180-4937-a031-65e6c0af5c8b">
<br><br>
Et en cliquant sur l'une des températures (par exemple), vous pourrez voir la valeur actuelle. 
<br><br>
<img width="1512" alt="BoPi - HA - Entites - detail" src="https://github.com/user-attachments/assets/db1639f0-ec0a-4ea3-8eca-bc0909502eec">
<br><br>
Si cela fonctionne, vous pouvez maintenant ajouter les scripts au fichier scripts.yaml puis redémarrer HA pour prendre en compte les changements. 
<br><br>
<img width="1512" alt="BoPi - HA - Scripts" src="https://github.com/user-attachments/assets/19d01e31-9e03-4d29-9cba-87081f9ae1f4">
<br><br>
Maintenant nous allons ajouter un tableau de bord pour BoPi. Commencez par créer un nouveau tableau de bord vierge. 
<br><br>
<img width="50%" alt="BoPi - HA - Ajouter un TDB 1" src="https://github.com/user-attachments/assets/4dfaf7e1-58e9-4136-9585-d284e6a58472"><img width="50%" alt="BoPi - HA - Ajouter un TDB 2" src="https://github.com/user-attachments/assets/3184ddac-9fb4-4c90-9326-1ddd1efe00dc">
<br><br>
Ensuite rendez vous dans le nouveau tableau de bord et editez le fichier de configuration.
<br><br>
<img width="323" alt="BoPI - HA - Editer TDB" src="https://github.com/user-attachments/assets/21d91dd2-0a01-46ca-83a2-cd5c97d0346b">
<br><br>
Copiez le contenu du fichier TableauDeBord dans le dossier correspondant à votre modèle dans la configuration du tableau de bord Home Assistant. 
<br><br>
<img width="1512" alt="BoPi - HA - editer TDB 2" src="https://github.com/user-attachments/assets/a87b19f7-691a-43c6-8bab-4165b4f0e332">
<br><br>
Enregistrez et vous avez maintenant BoPi dans Home Assistant. Selon votre modèle, cela ressemblera à l'un des deux écrans ci-dessous (BoPi et BoPi Max à gauche et BoPi Basic à droite).
<br><br>
<img width="50%" alt="BoPi - HA - TDB BoPi" src="https://github.com/user-attachments/assets/db7ad708-c23e-49df-8b94-3907c7955e98"><img width="50%" alt="BoPi - HA - TDB BoPi Basic" src="https://github.com/user-attachments/assets/892b73b5-f33a-4a69-90b3-b1204c6efbc6">
<br><br>
Si vous avez plus de questions au sujet de BoPi, n'hésitez pas via le site https://meetbopi.com/fr/



