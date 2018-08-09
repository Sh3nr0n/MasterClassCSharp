# Instructions

- Installer le package Mono qui permet d'utiliser .NET sur une machine linux

      sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
      sudo apt install apt-transport-https
      echo "deb https://download.mono-project.com/repo/ubuntu stable-xenial main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list
      sudo apt update
      sudo apt install mono-devel

 - Vérifier la version de mono installée

       mono --version

 - Commandes à entrer dans la console si dotnet n'est pas installé
 
       dotnet new
       dotnet new console
       dotnet pack


 - Installer le plugin C# dans VSCODE depuis la barre de recherche de plugins

 - Dézipper le projet WebApplication5.zip

  - Se placer à la racine du projet et ajouter la bibliothèque suivante qui permet d'utiliser une API pour interroger une de données de films (https://github.com/LordMike/TMDbLib)

       dotnet add package TMDbLib --version 1.3.0-alpha

 - Aller dans l'outil de débuggage VSCODE (icone insecte) et cliquer sur la flèche verte en face de **DEBOGUER** (sur la configuration .NET)

 Le site se lance en local dans le navigateur sur le port 5000.
