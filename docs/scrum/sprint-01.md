# Sprint 1 - Découverte et validation de Node.js

## Informations générales

- Responsable : Oussema Gassara
- Branche Git : `sprint-1-nodejs`
- Date de début : 22/10/2026
- Date de fin prévue : 28/10/2026
- Date de fin réelle : 22/10/2026
- Statut : Terminé

## Objectif du sprint

Comprendre le fonctionnement de Node.js, justifier son utilisation dans
l’application de transport et produire une première API fonctionnelle,
testée et documentée.

L’objectif du Sprint 1 a été atteint.

## Sprint Backlog

| ID | Tâche | Durée estimée | Statut |
|---|---|---:|---|
| S1-T1 | Créer la branche du Sprint 1 | 15 min | Terminé |
| S1-T2 | Organiser les dossiers du projet | 30 min | Terminé |
| S1-T3 | Créer le fichier `.gitignore` | 15 min | Terminé |
| S1-T4 | Initialiser le backend Node.js | 30 min | Terminé |
| S1-T5 | Créer la route `GET /api/health` | 45 min | Terminé |
| S1-T6 | Tester l’API | 30 min | Terminé |
| S1-T7 | Préparer la présentation Node.js | 3 h | Terminé |
| S1-T8 | Documenter le test de l’API | 30 min | Terminé |
| S1-T9 | Réaliser la Sprint Review | 30 min | Terminé |
| S1-T10 | Réaliser la rétrospective | 30 min | Terminé |

## Livrables réalisés

- Backend Node.js et Express initialisé.
- Route `GET /api/health` fonctionnelle.
- Réponse HTTP 200 au format JSON.
- Test de l’API réalisé avec PowerShell.
- Capture du résultat du test.
- Présentation synthétique sur Node.js.
- Documentation Scrum du Sprint 1.
- Fichiers enregistrés sur la branche GitHub `sprint-1-nodejs`.

### Emplacement des livrables

- `backend/src/app.js`
- `backend/src/server.js`
- `docs/nodejs-presentation/api-health-test.md`
- `docs/nodejs-presentation/api-health-test.png`
- `docs/nodejs-presentation/presentation-nodejs-sprint-1.pptx`

## Critères d’acceptation

- [x] Le serveur démarre avec `npm run dev`.
- [x] La route `/api/health` retourne un statut HTTP 200.
- [x] La réponse est au format JSON.
- [x] La présentation explique le fonctionnement et le rôle de Node.js.
- [x] Le test de l’API est documenté.
- [x] L’audit npm indique 0 vulnérabilité.
- [x] Les fichiers du Sprint 1 sont enregistrés sur GitHub.

## Sprint Review

### Éléments présentés

- Structure du backend Node.js.
- Fonctionnement de Node.js et de l’event loop.
- Utilisation de npm, Express, CORS et dotenv.
- Architecture prévue entre la machine Windows et la VM Ubuntu.
- Code de la route `GET /api/health`.
- Résultat du test effectué avec PowerShell.
- Présentation Node.js du Sprint 1.

### Résultat de la démonstration

Le serveur a démarré correctement sur le port `3000`.

La commande suivante a permis de tester l’API :

```powershell
Invoke-RestMethod http://localhost:3000/api/health