# Affichage-Flipr-HomeAssistant
Code ESPHome pour LILYGO TTGO T-Display 1.14 Pouces LCD + ESP32 Module sans Fil  Permet d'afficher les relevés de Flipr

Voici la version finale aves les deux boutons exploités (code3.yaml)
![alt text](https://github.com/SocrateMobile/Affichage-Flipr-HomeAssistant/blob/main/IMG-1884.jpg?raw=true)

 
 et les autres versions sont ici: 
 
v1  
![alt text](https://github.com/SocrateMobile/Affichage-Flipr-HomeAssistant/blob/main/avecbox.jpg?raw=true)


Les pré requis sont d'avoir:
- acheté une carte LILYGO TTGO T-Display 1.14 Pouces LCD + ESP32
- acheté un Flipr et activé son compte Flipr Analysr
- installé Home Assistant, et l'intégration Flipr
- relevé et remplacé dans le code.yaml le nom des entités 1 à 6 par celles de votre intégration
- édité ou crée le fichier secret.yaml DANS le répartoir config / esphome de votre Home Assistant
et y intégrer :
```
key_display_p: "votre token API de votre ESP"
ota_display_p: "votre token OTA"
wifi_ssid: "le nom de votre réseau WIFI de la maison"
wifi_password: "la clé de votre réseau wifi de la maison"
mdp_hotspot: "la clé du hotspot de votre ESP en cas de plantage"
server_username: le login que vous souhaitez pour accéder à l interface WEB de votre ESP
server_password: le MDP que vous souhaitez pour accéder à l interface WEB de votre ESP
```
n'oubliez pas de télécharger votre font, pour ce code sfCompact ici : https://font.gooova.com/fonts/14164/sf-compact-font-family.html
le fichier sera a insérer dans home assistant , dans le repertoir de ESPHome


Ensuite, dans ESPHome, copier / coller le code présent dans le fichier code.yaml

Lorsque le code est uploadé, les "binary sensor" se mettent à jour immédiatement, les "sensors" prennent quelques secondes à afficher
par la suite, la mise à jour se fait de maniere transparente, lorsque les relevés Flipr remontent dans Home Assistant

Si toutes les valeurs sont bonnes, tout est en vert

![alt text](https://github.com/SocrateMobile/Affichage-Flipr-HomeAssistant/blob/main/view_ok.jpg?raw=true)

Si des valeurs sont en dehors des limites définies, elles apparaissent en jaune si c'est a surveiller, et en rouge si il faut agir

![alt text](https://github.com/SocrateMobile/Affichage-Flipr-HomeAssistant/blob/main/view_pb.jpg?raw=true)

Les valeurs de Chlore et pH peuvent être en rouge, avec des indications OK, c est parceque l'IA Flipr ne voit pas de problème à régler,
juste patienter et surveiller 

# si vous optez pour la version avec les logos, code2.yaml, vous devrez également mettre dans le repertoire ESPHome les deux fichiers ok_logo.jpg et pb_logo.jpg 

le code2.yaml, ajoute des logos qui remplacent aventageusement le texte OK ou PB du code initial

v2
![alt text](https://github.com/SocrateMobile/Affichage-Flipr-HomeAssistant/blob/main/aveclogo.jpg?raw=true)

Vous pouvez ensuite imprimer la boite qui va bien... 

https://github.com/Xinyuan-LilyGO/TTGO-T-Display/tree/master/3d_file

![alt text](https://github.com/Xinyuan-LilyGO/TTGO-T-Display/raw/master/image/image4.jpg)





Have fun ;-)
