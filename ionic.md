# 1. Installation
Télecharger:
- [Node.js 6.11.4 LTS](https://nodejs.org/en/)
- [jdk-8u144-windows-x64.exe](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- [android sdk studio](https://developer.android.com/studio/index.html)
- [Git](https://git-scm.com/downloads)
- les packages android platform sdk pour android 6 et 7 à partir du Android studio
```sh
$ npm install -g ionic cordova
$ ionic start toiletadvisor
```

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

### variables environnement system
variable système | valeur
---------------- | ----------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
JAVA_HOME | C:\Program Files\Java\jdk1.8.0_144
ANDROID_HOME | C:\Users\JM\AppData\Local\Android\sdk
Path | C:\Users\JM\AppData\Local\Android\sdk\tools;C:\Users\JM\AppData\Local\Android\sdk\tools\bin;C:\Users\JM\AppData\Local\Android\sdk\platform-tools

Ajouter Android à la liste des plateformes et construire l'App
```sh
$ ionic cordova platform add android
$ ionic cordova build android
```

# 2. Créer une page et l'ajouter aux tabs 

```sh
ionic generate page tatatest
```
##### C:\Users\JM\Documents\coursionic\toiletadvisor\src\app\app.module.ts
ajouter la page, la mettre aussi dans declarations et entrycomponents
##### C:\Users\JM\Documents\coursionic\toiletadvisor\src\pages\tabs\tabs.html
##### C:\Users\JM\Documents\coursionic\toiletadvisor\src\pages\tabs\tabs.ts
modifier pour ajouter la page aux tabs


# 3. Changer une image d'une tab 

##### C:\Users\JM\Documents\coursionic\toiletadvisor\src\pages\tabs\tabs.html
repérer la tab icon

##### C:\Users\JM\Documents\coursionic\toiletadvisor\www\build\main.css
remplacer le css de la class par 
```sh
content: url('../img/horse.jpg') !important;
```

# 4. Splashscreen
```sh
$ cordova platform add android --nofetch
```
##### C:\Users\JM\Documents\coursionic\toiletadvisor\resources
Remplacer icon.png et splash.png, puis créer toutes les resources avec
```sh
$ ionic cordova resources
```


