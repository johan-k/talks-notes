# Devoxx France 2025

## Mercredi

09:00 -> 09:45 : l'intelligence artificienne n'existe pas 
livre de luc julia : l'intellogence artificielle n'existe pas
voir : avocat de new york qui a généré une plaidoirie pour un cas d'un avion
pourquoi ne peut on pas refroidir un datacenter avec l'eau salé ?
les images générés par IA sont watermarquées pour ne pas qu'elles entrainent les IA à l'avenir comme c'est des images nulles

TP kubernetes : 
essayer de le refaire avec minikube

jep : 
dans openjdk
un niveau pour recevoir les mail : participant
un niveau contributeur 
openjdk member
openjdk lead

author / committer / reviewer / project lead (4 status par projet)

13:30 -> 17h Full stack Java, du dev à la prod en passant par l'infra :
c'est le mec qui a fait la présentation picocli ? :o https://philippart-s.github.io/blog/articles/dev/java/discover-picocli/

voir le plugin continue pour aovir la completion de l'IA 
aller voir le talk de l'année dernière de guillaume laforge sur le RAG
easyRAG facilite la partie rag
pgvector pour les vector
test container à voir 
qute à voir, c'est un moteur de compléting pour quarkus
pulumi : ils ont une infra as code - code first, et ont une version java (en beta)

JEP 330 et 448 ou 458 et 445
Jbang la seule alternative en Java, permet de faire des scripts et des CLI (mais picocli est mieux pour ca)
Max rydahl Andersen qui faut ce talk

12h35 demain pour l'install de JBang

le _ dans jenkinsfile est un sucre syntaxiuue me permettant de .. à vérifier

penser à Fabric 8 qui est un client Kubernetes pour manipuler les ressources

il utilise k3s 

jib permet de construire une image docker sans dockerfile

ovh a octavia en service de load balancing

son travail : https://github.com/johan-k/java-full-stack-devoxx25/tree/talk


17:00 -> 17:30 ça marche dans mon .devcontainer

un conteneur c'est une sortie d'un processus de build
voir ce qu'est J env
il faut : 
-docker
-vscode
-extention devcontener

voir la doc .devcontainer
bmoussaud / devcontainer_random_api : https://github.com/bmoussaud/devcontainer_random_api

dans vscode : reopen dans container, dans doceker on voir que l'on a le devcontainer/python3.12 qui vient de démarrer (dans command palette)
on peut aussi clone repository in a container et la on le trouvera dans la partie volume du docker desktop

on peut ajouter des container feature par vscode pour avoir par exemple la lib Vegeta

codespace peut héberger son environnement github


17:50 -> 18h20
exegol : onstallation, la taille des image peux etre volumineuse

COMMAND Burpsuite, une sorte de proxy sous steroide, intercepter des requetes et les envoyer
plugin chrome wappanalyser
command exegol shellerator
nc -lnvp 1337 (c'était le port)

## Jeudi
10:30 -> 11:15 : Architecture
qu'est ce qu'un diagramme de contexte C4 ?
-On doit penser d'abord problème avant solution
-négocier l'architecture, et éduquer 
-Penser modulaire
-toute solution amène de nouveau problème, les solutions distribuées en amènent plus
-preagmatic but not naive 
voir pubSub, (et les autres) 
-prévoir des options pas cher pour éviter les décisions irreversibles
-On sait que ca ne marche pas, c'est génial ! surtout quand c'est très tot
-Reconnaissez les problèmes difficiles et déléguez les à d'autres (fournisseurs de service par exemple)
-art du tradeoffs (compromis)
-idempotence = important
-architecture est dynamique
-contract: on ne veut pas de breaking change, et si l'api est publiée, elle n'est plus à nous 
-garder trace des décisions (par une ADR)
-Tester son architecture (comme ArchUnit)
-Timeboxer les décision d'archi
-Aller au tableau
-alterner le résonnement individuel et collectif : exemple chacun prend 15 min pour voir sa solution, sans la justifier, et on met en commun
phillipe bordeau (à voir l'orthographe)
-penser baby steps pouf apprendre beaucoup et petit 
regarder ce qu'est mcp

11:35 -> 12:20 booster démarrage des app java
-Lazy initialization
voir servlet, AOP et reflection
voir hibrenate sur jarvis ?
voir ce que c'est que le staging / canary

voir jpbempel (son github)
google/kube-startup-cpu-boost

13:30 -> 14:15 : Dans les coulisses des licornes géantes de la tech !
-efficiency without learning is waste, motion != progress
regarder how might wwe et Opportunity solution tree
Data Insight Believe Best (DIBB)
-learning pipeline != delivery pipeline
-système nerveux, systeme immunitaire et système respiratoire
-discovery + delivery = one flow, one team
-one refacto a day, keeps doctor at bay
delivery -> dibb - business kpi - business case
OKR c'est ?
-delivery = experimentation, not implementation


15:40 - 16:25 : Et si on parlait de malware craftmanship ?
Dev#Popper

matrice de .. qui fait TTP : tactique techniques et procedures

hybrid analysis, virustotal ou malwares.com sont des sites qui détectent des antivirus

pour faire son propre lab : flare vm et REMux
on peut utiliser PE studio

process explorer et process monotor idspo sur windows pour voir ce qui se passe

de4dot permet de desobfusqué du code


17:00 - 17:30 : Spark4 et iceberg

17:50 - 18:20 : {Cloud || Container} Development Environment
C2 sur du cloud vs C2 container 
C2 distant (cloud development environment - CDE) : aucune conf en local, plus vite opérationel 
C2 distant : zenika-open-source/the-duck-gallery
github.com -> github.dev, et la on a un env vscode distant, c'est ouf !!!!!
CDE : google va arrêter google CDX, mais Firebase studio va remplacer
ca se base sur le fichier .idx/dev.nix
autre possibilité : gitpod
ou sinon ... jetbrains gateway !
ou devpod

==
CDE : Container development environment (meme nom ??)
faut installer l'extension devcontiner (au moins pour vscode, voir pour intellij)


il est possible aussi d'utiliser la solution google Cloud Workstation
