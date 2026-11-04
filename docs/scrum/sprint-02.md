# Sprint 2 — Conception UML et communication réseau

## 1. Informations générales

- Responsable : Oussema Gassara
- Branche de travail : sprint-2-uml
- Branche cible : main
- Période : à renseigner
- Statut : En cours

## 2. Objectif du sprint

Concevoir l'architecture de l'application de réservation de transport interurbain (bus et louages) à l'aide de diagrammes UML, puis configurer et valider la communication réseau entre les environnements Windows et Ubuntu Server.

## 3. Périmètre de conception retenu

- Bus interurbains et louages uniquement pour la V1.
- Trajets directs entre deux villes.
- Recherche de départs entre aujourd'hui et J+2.
- Choix du véhicule et du siège.
- Réservation avec paiement en ligne ou paiement sur place.
- Réservations sans paiement préalable limitées à 25 % de la capacité par départ.
- Vente directe en espèces à la station, distincte d'une réservation préalable.
- QR Code unique et contrôle par le chauffeur.
- Réduction PMR de 6 % après validation administrative.
- Suivi GPS, estimation initiale, ETA actualisée et durée réelle.
- Départs créés et publiés par l'administrateur ; le chauffeur peut proposer un départ soumis à validation.
- Chaque véhicule possède un chauffeur attitré en V1 ; un remplacement temporaire peut être autorisé par l'administrateur.
- Un véhicule peut effectuer plusieurs départs dans la journée si les disponibilités le permettent.

## 4. Livrables UML préparés

Les sources PlantUML sont enregistrées dans docs/uml/ :

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

Le détail du périmètre, les liens vers les sources et les points restant à valider sont documentés dans docs/uml/README.md.

## 5. Travail réseau restant

- Préparer la machine Windows (serveur applicatif).
- Préparer Ubuntu Server (serveur de base de données).
- Configurer les adresses et la connectivité réseau.
- Tester la communication entre les deux machines.
- Tester l'accès au service backend depuis le client distant.
- Conserver les captures et rédiger le compte rendu des tests.

## 6. Critères de validation

- [x] Première version des diagrammes UML préparée.
- [x] Sources PlantUML modifiables enregistrées dans le dépôt.
- [ ] Diagrammes relus et validés.
- [ ] Architecture réseau Windows / Ubuntu configurée.
- [ ] Connectivité entre les deux machines démontrée.
- [ ] Accès distant au backend testé.
- [ ] Compte rendu réseau et captures ajoutés.

## 7. Points encore ouverts

Les choix détaillés concernant les stations, le délai exact d'embarquement, les remboursements, le fournisseur de paiement, le service cartographique, la fréquence GPS, le temps de préparation entre départs et la gestion des pannes restent à valider. Ils sont recensés dans docs/uml/README.md.

## 8. Conclusion provisoire

La première version des diagrammes UML est préparée et publiée pour revue. Le Sprint 2 reste en cours : les diagrammes doivent être validés et la partie communication réseau Windows–Ubuntu doit encore être réalisée et documentée.
