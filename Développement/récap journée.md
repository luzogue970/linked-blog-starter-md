  

07/05:

front image fonctionnelle dans docker-compose

update sur boond client qui était pas set auto

papeline front working

06/05:

passer la journée sur le proxy angular + front to directus galère

19/04:

matin : pipeline web deployment résolue

17/04:

pipeline creation projet client carré pour le lecoal deployment + env variable

16/04:

matin : pipeline bitbucket docker push carré directus / front / back

15/04:

clarification des pipeline pour front back bdd avec déploiment optionnel vers docker hub

12/04:

matin : recherche solution claire pour le déploiement

après midi : mise en place de la solution

10/04:

matin :

requêtage api bitbucket pour créer au final projets client

après midi:

solution satisfaisante

08/04

objectifs: permettre déploiement de l’app sur différents Boond app.

puis permettre mise a jour de l’app avec persistence des données ente les mise a jour ⇒

matin

déploiement app : comment déployer une app front hebergeur classique mais back

après midi:

render test déploiement app mais pas privé donc non

déploiment bakc sans perdre data ⇒ update de l’api sans toucher au a directus/DB

  

13/03

matin : front galère essaye sur file , comprendre observable

après midi : observable pas sûr de l’application, mais tout marche ok

  

12/03

matin : pipeline fini avec changement token to connexion

après midi : perm user mauvaise : vorrection + début front

  

11/03 :

matin : essaies sur pipeline et design patern singleton

après midi, design patern bridge et pipeline ( c la merde )

  

22/02 :

bitbucket pb pipeline chaud

client fait correctement et init clean

  

21/02 : pipeline fonctionnelles ⇒ pb était fonctions directus

problème de build l’extension directus sur la pipeline, dépendances insuffisante

après midi : boondConnector pipeline

test mockito.verifyNoMoreInteractions

service des mes events

  

14/02 :

pipeline toujours galère

après docker push de mon directus

try docker compose up sur ma pipeline bitbucket avec l’image sus-dite

essaye docker compose avec image

essaye docker compose avec dockerfile et api direct

docker compose inutile ⇒ essaye definition des services a l’intérieur de la pipeline

  

12/02 : matin pipeline bitbucket test d’integration enlever, build passe

voir comment mettre en place test d’integration

  

24/01: amélioration test / création test service

  

23/01/24

matin: test d’intégration mock, difficultés mock de BoondFileClient (absolute path)

après midi : test service mock différent pour unit et integration