# Sprint 2 — Conception UML et communication réseau

## 1. Informations générales

- Responsable : Oussema Gassara
- Branche de travail : sprint-2-uml
- Branche cible : main
- Période : à renseigner
- Statut global : En cours pour le groupe 2; groupes 1 et 3 terminés

## 2. Objectif du sprint

Concevoir l'architecture de l'application de réservation de transport interurbain (bus et louages) à l'aide de diagrammes UML, puis configurer et valider la communication entre Windows et Ubuntu Server.

## 3. Périmètre de conception retenu

- Bus interurbains et louages uniquement pour la V1.
- Trajets directs entre deux villes.
- Recherche de départs entre aujourd'hui et J+2.
- Choix du véhicule et du siège.
- Réservation avec paiement en ligne ou paiement sur place à l'embarquement.
- Plafond de 25 % de la capacité par départ pour les réservations préalables avec paiement sur place (PAY_ON_SITE).
- Vente directe en espèces à la station sans plafond de 25 %, dans la limite des sièges disponibles.
- QR Code unique et contrôle par le chauffeur.
- Réduction PMR de 6 % après validation administrative.
- Suivi GPS, estimation initiale, ETA actualisée et durée réelle.
- Départs créés et publiés par l'administrateur; le chauffeur peut proposer un départ soumis à validation.
- Chaque véhicule possède un chauffeur attitré en V1; un remplacement temporaire peut être autorisé par l'administrateur.
- Un véhicule peut effectuer plusieurs départs dans la journée si les disponibilités le permettent.

## 4. Livrables UML préparés

Les sources PlantUML et les aperçus SVG des dix diagrammes sont enregistrés dans docs/uml/ :

1. Cas d'utilisation Client et Client PMR.
2. Cas d'utilisation Chauffeur.
3. Cas d'utilisation Administrateur.
4. Diagramme de classes.
5. Séquence de recherche et réservation.
6. Séquence de scan QR et embarquement.
7. Séquence de vente directe à la station.
8. Séquence GPS, ETA et durée réelle.
9. Séquence de création et publication d'un départ.
10. Diagramme de déploiement.

Les sources, aperçus et points encore ouverts sont recensés dans docs/uml/README.md.

## 5. Bilan des activités par groupe

### Groupes 1 et 3 — activités terminées selon le bilan de sprint

- Conception de l'architecture à l'aide des diagrammes UML.
- Mise en œuvre et tests de la communication réseau.
- Installation et configuration de PostgreSQL sous Linux.
- Vérification du bon fonctionnement de la base de données.
- Configuration et test de la connexion entre Node.js et PostgreSQL.
- Pour le groupe 3, PostgreSQL a été installé sur Ubuntu dans une machine virtuelle avec `sudo apt install postgresql`.

### Groupe 2 — tâches restantes

Le groupe 2 poursuivra et achèvera les tâches restantes lors de la prochaine séance, tout en entamant les activités prévues au prochain sprint.

Les statuts de suivi restent « En cours » tant que le groupe 2 n'a pas terminé sa part. Les preuves détaillées des tests réseau et base de données (résultats ou captures) restent à joindre au dépôt pour documenter les réalisations.

## 6. Critères de validation par groupe

- [x] Les groupes 1 et 3 déclarent avoir finalisé les activités prévues du Sprint 2.
- [x] PostgreSQL installé sur Ubuntu pour le groupe 3.
- [x] Vérification de la base de données et connexion Node.js–PostgreSQL déclarées réalisées pour les groupes 1 et 3.
- [ ] Les tâches restantes du groupe 2 sont à terminer et à documenter.
- [ ] Les résultats détaillés ou captures des tests réseau et base de données sont à ajouter au dépôt.

## 7. Points à valider avant de figer la conception

Les choix détaillés concernant les stations, le délai exact d'embarquement, les remboursements, le fournisseur de paiement, le service cartographique, la fréquence GPS, le temps de préparation entre départs et la gestion des pannes restent à valider avant l'implémentation. Ils sont recensés dans docs/uml/README.md.

## 8. Conclusion du sprint

Les groupes 1 et 3 ont finalisé les activités prévues. Le groupe 2 doit encore terminer sa part lors de la prochaine séance. Le suivi global reste donc en cours jusqu'à la clôture de ces tâches et l'ajout des preuves de validation.

## 9. Objectifs du prochain sprint

**Axe de travail : validation de l'application et développement de l'API de réservation.**

Les tâches planifiées sont :

- Déployer l'application dans un environnement de travail commun pour faciliter l'intégration et les tests.
- Valider les principales fonctionnalités et identifier les anomalies.
- Concevoir et développer l'API de réservation avec Node.js.
- Documenter les endpoints, leurs paramètres et leurs réponses.
- Permettre au client de créer et soumettre une réservation.
- Permettre au chauffeur de consulter les réservations et d'en vérifier les informations.

**Livrable attendu :** une application déployée dans un environnement commun, avec une API de réservation fonctionnelle et les principales interactions entre le client, le chauffeur et le système validées.
