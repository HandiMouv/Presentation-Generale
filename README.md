# Presentation-Generale
## Table des matières
- [Présentation](#pres)
- [Nos repositories](#repos)
- [Documentation](#docu)
- [Crédit](#cred)
- [L'Equipe](#team)
- [Contact](#contact)

## <a name="pres"/>Présentation
Ce projet est dans le cadre d'[HandiTech](https://handitech-france.fr/) et a pour vocation à fournir une normalisation et une clarification de la communication entre les projets de **controleurs** et d'**actionneurs** dont vous pouvez voir le schéma ci-dessous:<br>
> ***Figure 1:** Schéma des échanges entre les projets HandiTech<br>*
> <image width=400 height=250 src="https://github.com/HandiMouv/Presentation-Generale/blob/main/IMAGES/SchemaDesParties.png"/><br>

Pour illuster ce processus, nous avons créé un projet de **pointeur de souris piloté à distance** en tant que simple démonstrateur.<br>
> ***Figure 2:** MVP<br>*
> <image width=800 height=250 src="https://github.com/HandiMouv/Presentation-Generale/blob/main/IMAGES/MVP.PNG"/><br>

Nous utilisons un téléphone sous Android afin de commander le pointeur de souris sur un ordinateur.<br>
- Pour cela, nous avons développé une application mobile qui envoie par bluetooth des signaux pour chacune des actions effectuées par l'utilisateur sur l'application. L'utilsateur peut choisir le nombre de bouttons sur l'application et choisir les valeurs des signaux envoyés.<br> 
- Ces signaux sont réceptionnés par un serveur tournant sur un microcontroleur Raspberry PI dont le bluetooth en réception a été activé. Ces signaux sont traités et transformés en ordres. Les ordres sont transmis de la Raspbery PI à l'ordinateur par câble ethernet sous forme de socket.<br>
- L'ordinateur reçoit les ordres et les applique au curseur de souris.
## <a name="repos"/>Nos repositories
- [MobileApp](https://github.com/HandiMouv/MobileApp) : L'Application mobile sous Android.
- [RaspberryPI](https://github.com/HandiMouv/RaspberryPI) : Le code sur Raspberry PI.
- [Demonstrateur](https://github.com/HandiMouv/Demonstrateur) : Le code du démonstrateur.

## <a name="docu"/>Documentation
- **Mobile App:**<br>
*Comment télécharger et lancer notre application ? Comment l'utiliser ?*<br>
-> [README Mobile App](https://github.com/HandiMouv/MobileApp#readme)<br>
- **Raspberry PI:**<br>
*Comment formater une carte SD pour la Raspberry PI ? Vous y connecter par SSH ? Changer d'accès WIFI ?*<br>
-> [Initialisation de la Raspberry PI](https://github.com/HandiMouv/Presentation-Generale/blob/main/DOCUMENTATION/Configuration%20Raspberry%20PI.pdf)<br>
- **Démonstrateur:**<br>

## <a name="cred"/>Crédit
- Le projet [ArmBot-ECE](https://github.com/ArmBot-ECE) sous licence [GNU](https://github.com/HandiMouv/Presentation-Generale/blob/main/LICENSE) pour sa base technique.
- Notre mentor, Frederic RAVAULT, pour ses conseils.

## <a name="team"/>L'Equipe
Charles SAISON<br>
Henri PETRELLI<br>
Hugo JAOUEN<br>
Jacques POLLART<br>
Helena REVUE<br>
Romain BARRERE<br>

## <a name="contact"/>Contact
handimouv.handitech@gmail.com


