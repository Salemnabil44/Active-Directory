### Création d'une GPO

## Étape 1

Lancer Active Directory puis cliquez sur "outil" > "Gestion des stratégies de groupe"

<img width="1004" alt="Capture d’écran 2024-07-14 à 18 24 21" src="https://github.com/user-attachments/assets/08f48b57-172a-4c8c-837f-3f6234ad1ab2">


<img width="1005" alt="Capture d’écran 2024-07-14 à 18 24 32" src="https://github.com/user-attachments/assets/bd3b475a-6eb3-4763-aa25-6c90f56381ab">

## Étape 2

Cliquez droit sur le nom de votre domaine, puis cliquez sur "Créer un objet GPO dans ce domaine, et le lier ici..."

<img width="1005" alt="Capture d’écran 2024-07-14 à 18 39 49" src="https://github.com/user-attachments/assets/f52032dd-f0d3-4c6d-9bd3-6a839ec11861">

## Étape 3

Pour modifier la GPO pour que les utilisateurs du groupe Wilders_Students ne puisse pas avoir accès au panneau de configuration de Windows.

- Èditez la GPO

<img width="1009" alt="Capture d’écran 2024-07-14 à 19 06 35" src="https://github.com/user-attachments/assets/40466138-3224-417f-a537-0dcdcbd81c33">

- Cliquez sur "User Configuration" > "Policies" > "Administrative Templates" > "Control panel" > puis cliquez sur "Prohibit access to Control Panel and PC settings"

<img width="1006" alt="Capture d’écran 2024-07-14 à 19 09 14" src="https://github.com/user-attachments/assets/2f1a0424-b48c-4fc9-bd0c-33ec65274cf6">

- Puis cliquez sur "Enabled" , puis "Apply" et terminez par "OK"

<img width="1003" alt="Capture d’écran 2024-07-14 à 19 11 39" src="https://github.com/user-attachments/assets/abfc8a56-6cd5-449d-b842-12a3d270b7c7">

## Étape 4

Pour vérifier que la configuration est bien mise en place, cliquez sur la GPO et allez dans "Settings"

<img width="1004" alt="Capture d’écran 2024-07-14 à 19 13 11" src="https://github.com/user-attachments/assets/fcedd2d2-d865-48a8-bfe5-5f67327c7adb">

## Étape 5

Retournez à la console de gestion des stratégies de groupe.
Faites un clic droit sur la GPO "Wilders" et sélectionnez "Modifier".
Dans le panneau de droite, cliquez sur l'onglet "Délégation" puis Cliquez sur "Ajouter" et ajoutez le groupe ou l'utilisateur que vous souhaitez restreindre.

<img width="782" alt="Capture d’écran 2024-07-14 à 21 11 25" src="https://github.com/user-attachments/assets/8dbd12d0-9ecd-4ff2-871b-3d1f873660c4">

<img width="781" alt="Capture d’écran 2024-07-14 à 21 11 53" src="https://github.com/user-attachments/assets/df5ff79e-8cf4-42d1-aeb9-dcfbff8d8043">

<img width="782" alt="Capture d’écran 2024-07-14 à 21 12 23" src="https://github.com/user-attachments/assets/0ea944b7-5bc0-44c1-bba1-7685d26735fa">

## Étape 6 : Vérification de la configuration

Connectez vous avec un compte appartenant au groupe "Wilders_Students". Essayez d'ouvrir le panneau de configuration via le menu démarrer ou la boîte de dialogue "Exécuter". Vous devriez recevoir un message indiquant que l'accès est interdit, ce qui confirme que la GPO est correctement appliquée.







