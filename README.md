
# code-frontend 
ajout du dossier /.github/workflows
This project uses Quarkus, the Supersonic Subatomic Java Framework.
This is the demo project present Qute template
If you want to learn more about Quarkus, please visit its website: https://quarkus.io/ .

# Etapes de la CI à mettre en place

## Running the application in dev mode

Compilation de l'application - Consiste à verifier que l'application compile sans bug:
```shell script
./mvnw clean compile 
```

## Realisation des tests unitaires et ensuite les tests d'intégrations

Pour executer les tests unitaires 
```shell script
./mvnw test
```

Pour executer les tests d'intégrations 
```shell script
./mvnw clean verify
```
## Realisation du build de l'artefact

Construction de l'artefact de type  _über-jar_ - le resultat est un package  `quarkus-run.jar` dans le repertoire `target/quarkus-app/`

```shell script
./mvnw clean package
```

A lire: les goals maven pour comprendre le cycle de vie de construction d'une application Java
