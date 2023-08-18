# Affichage-Flipr-HomeAssistant
Code ESPHome pour LILYGO TTGO T-Display 1.14 Pouces LCD + ESP32 Module sans Fil  Permet d'afficher les relevés de Flipr

Les pré requis sont:
avoir acheté une carte LILYGO TTGO T-Display 1.14 Pouces LCD + ESP32 
avoir un Flipr et activé son compte Flipr Analysr
avoir installé Home Assistant, et l'intégration Flipr
avoir relevé et remplacé dans le code.yaml le nom des entités 1 à 6 par celles de votre intégration

Lorsque le code est uploadé, les "binary sensor" se mettent à jour immédiatement, les "sensors" prennent quelques secondes à afficher
par la suite, la mise à jour se fait de maniere transparente, lorsque les relevés Flipr remontent dans Home Assistant

Si toutes les valeurs sont bonnes, tout est en vert

![alt text](https://github.com/SocrateMobile/Affichage-Flipr-HomeAssistant/blob/main/view_ok.jpg?raw=true)

Si des valeurs sont en dehors des limites définies, elles apparaissent en jaune si c'est a surveiller, et en rouge si il faut agir

![alt text](https://github.com/SocrateMobile/Affichage-Flipr-HomeAssistant/blob/main/view_pb.jpg?raw=true)

Les valeurs de Chlore et pH peuvent être en rouge, avec des indications OK, c est parceque l'IA Flipr ne voit pas de problème à régler,
juste patienter et surveiller 

Prochaine étape pour moi, acheter une imprimante 3D et imprimer le boitier 


![alt text](https://github.com/Xinyuan-LilyGO/TTGO-T-Display/raw/master/image/image4.jpg)
