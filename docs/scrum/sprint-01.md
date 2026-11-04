# Sprint 1 — Découverte et validation de Node.js

## 1. Informations générales

- Responsable : Oussema Gassara
- Branche de travail : `sprint-1-nodejs`
- Branche d'intégration : `main`
- Pull Request : [#1 — Sprint 1: initialize Node.js API and documentation](https://github.com/oussema-gassara/application_transport_devabaselog/pull/1)
- Date de début : 22/10/2026
- Date de fin prévue : 28/10/2026
- Date de fin réelle : 22/10/2026
- Statut : Terminé

## 2. Objectif du sprint

Comprendre le fonctionnement de Node.js, justifier son utilisation dans l'application de transport et produire une première API fonctionnelle, testée et documentée.

L'objectif du Sprint 1 a été atteint : le backend Node.js/Express a été initialisé, la route de contrôle de santé a été créée et testée, puis les preuves et la présentation ont été publiées sur GitHub.

## 3. Sprint Backlog

| ID | Tâche | Durée estimée | Statut |
|---|---|---:|---|
| S1-T1 | Créer la branche du Sprint 1 | 15 min | Terminé |
| S1-T2 | Organiser les dossiers du projet | 30 min | Terminé |
| S1-T3 | Créer le fichier `.gitignore` | 15 min | Terminé |
| S1-T4 | Initialiser le backend Node.js | 30 min | Terminé |
| S1-T5 | Créer la route `GET /api/health` | 45 min | Terminé |
| S1-T6 | Tester l'API | 30 min | Terminé |
| S1-T7 | Préparer la présentation Node.js | 3 h | Terminé |
| S1-T8 | Documenter le test de l'API | 30 min | Terminé |
| S1-T9 | Réaliser la Sprint Review | 30 min | Terminé |
| S1-T10 | Réaliser la rétrospective | 30 min | Terminé |

## 4. Réalisations et livrables

- Backend Node.js et Express initialisé.
- Séparation de l'application (`app.js`) et du démarrage du serveur (`server.js`).
- Configuration de CORS et du middleware JSON.
- Route `GET /api/health` créée.
- Test de l'API réalisé avec PowerShell.
- Capture du résultat du test publiée.
- Présentation synthétique sur Node.js publiée.
- Documentation du test et documents Scrum publiés.

### Emplacement des livrables

- `backend/src/app.js`
- `backend/src/server.js`
- `backend/package.json`
- `docs/nodejs-presentation/api-health-test.md`
- `docs/nodejs-presentation/api-health-test.png`
- `docs/nodejs-presentation/presentation-nodejs-sprint-1.pptx`
- `docs/scrum/product-backlog.md`
- `docs/scrum/action-tracking.csv`

## 5. Test et critères d'acceptation

La route `GET /api/health` a été testée sur le port `3000` avec PowerShell. Le résultat documenté est une réponse HTTP 200 au format JSON.

Commande de démarrage :

```powershell
cd backend
npm run dev
```

Commande de test :

```powershell
Invoke-RestMethod http://localhost:3000/api/health
```

Critères d'acceptation :

- [x] Le serveur démarre avec `npm run dev`.
- [x] La route `/api/health` retourne un statut HTTP 200.
- [x] La réponse est au format JSON.
- [x] La présentation explique le fonctionnement et le rôle de Node.js.
- [x] Le test de l'API est documenté et accompagné d'une capture.
- [x] Le résultat de l'audit npm est indiqué à 0 vulnérabilité dans le bilan du Sprint 1.
- [x] Les livrables sont enregistrés sur GitHub et la Pull Request #1 a été fusionnée dans `main`.

Preuve du test : [api-health-test.png](../nodejs-presentation/api-health-test.png).

## 6. Sprint Review

### Éléments présentés

- Structure du backend Node.js.
- Fonctionnement de Node.js et de l'event loop.
- Utilisation de npm, Express, CORS et dotenv.
- Architecture envisagée entre la machine Windows et la VM Ubuntu.
- Code de la route `GET /api/health`.
- Résultat du test réalisé avec PowerShell.
- Présentation Node.js du Sprint 1.

### Résultat

Le serveur a démarré sur le port `3000`. La route de contrôle de santé a retourné une réponse HTTP 200 au format JSON. La présentation, la documentation et la capture du test ont été ajoutées au dépôt. La Pull Request #1 a été fusionnée dans `main` le 22/10/2026.

## 7. Rétrospective

### Points positifs observables

- Le backend dispose d'une première structure claire avec une séparation entre la configuration Express et le démarrage du serveur.
- La première route API a été testée et une preuve du test a été conservée.
- Les livrables techniques et la présentation ont été intégrés dans GitHub.
- Le travail a été livré avec une Pull Request dédiée et fusionnée dans `main`.

### Points à améliorer pour les prochains sprints

- Renseigner la durée réelle de chaque action dans le fichier de suivi.
- Maintenir les statuts du Product Backlog, du Sprint Backlog et du fichier de suivi synchronisés.
- Définir les critères de validation et les preuves attendues avant de commencer chaque tâche.

Aucune durée réelle détaillée ni difficulté technique précise n'avait été consignée dans le suivi initial du Sprint 1 ; ces informations ne sont donc pas estimées rétroactivement.

### Actions retenues pour le Sprint 2

- Concevoir les diagrammes UML du système.
- Décrire l'architecture client-serveur.
- Préparer et tester la communication entre Windows et Ubuntu Server.
- Documenter les résultats et conserver les preuves des tests.

## 8. Conclusion

Le Sprint 1 est terminé. Il a permis de valider le démarrage d'un backend Node.js/Express et une première route API de contrôle de santé, ainsi que de produire la présentation et les preuves associées. Le Sprint 2 portera sur la conception UML et la validation de la communication réseau.
