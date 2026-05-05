# Politique de confidentialité — TEKKIL

**Dernière mise à jour : 5 mai 2026**

TEKKIL est une application de préparation aux concours nationaux au Sénégal (Android, iOS et Web), éditée par **K-Edtech**. La présente politique décrit quelles données nous collectons, comment nous les utilisons et vos droits à leur égard.

---

## 1. Données collectées

### 1.1 Données d'inscription et de profil
- Nom et prénom
- Adresse e-mail
- Numéro de téléphone (optionnel)
- Ville de résidence (optionnelle)
- Photo de profil (optionnelle, stockée sur Cloudflare R2)
- Mot de passe (stocké sous forme hachée — jamais en clair)

### 1.2 Données d'apprentissage et de progression
- Résultats aux QCM (questions répondues, réponses choisies, score par session)
- Profil adaptatif par rubrique : taux de réussite, score de fragilité, niveau (facile / intermédiaire / difficile)
- Historique des sessions d'entraînement et d'examens blancs (date, durée, score)
- Progression dans les cours, résumés, audios et vidéos (position de lecture)
- Cartes mémo (flashcards) : score SM-2, intervalle de révision
- Statistiques de streak (nombre de jours consécutifs d'entraînement)

### 1.3 Données de paiement
- Historique des achats (packs achetés, montant, date)
- Méthode de paiement utilisée (Orange Money, Wave, carte bancaire via Stripe)
- **Aucune donnée de carte bancaire n'est stockée sur nos serveurs** — elles sont traitées directement par Stripe.

### 1.4 Données techniques et d'appareil
- Type d'appareil (mobile / web / desktop)
- Adresse IP (pour la sécurité et la prévention de fraude)
- Jeton de session (stocké de façon sécurisée, révocable à tout moment)
- Journaux de connexion (date, heure, appareil)

### 1.5 Données du chatbot IA
- Messages échangés avec le chatbot contextuel (stockés pour l'historique de conversation)
- Ces messages sont envoyés à OpenAI (GPT-4o-mini) de façon anonymisée pour générer les réponses.

### 1.6 Notifications push
- Jeton FCM (Firebase Cloud Messaging) pour recevoir les notifications — peut être révoqué depuis les paramètres de votre appareil.

---

## 2. Utilisation des données

Vos données sont utilisées exclusivement pour :

| Finalité | Base légale |
|---|---|
| Créer et gérer votre compte | Exécution du contrat |
| Vous donner accès aux packs achetés | Exécution du contrat |
| Calculer et afficher votre progression | Exécution du contrat |
| Personnaliser les sessions d'entraînement via le moteur adaptatif | Intérêt légitime |
| Afficher votre rang dans les classements | Intérêt légitime |
| Envoyer des notifications pédagogiques | Consentement |
| Prévenir la fraude et le partage de compte | Intérêt légitime |
| Améliorer nos contenus et fonctionnalités | Intérêt légitime |

Vos données ne sont **jamais vendues** à des tiers.

---

## 3. Partage des données avec des tiers

| Tiers | Rôle | Données partagées |
|---|---|---|
| **Neon (PostgreSQL)** | Hébergement de la base de données | Toutes les données applicatives |
| **Cloudflare R2 + CDN** | Stockage et diffusion des médias | Fichiers pédagogiques (PDF, audio, vidéo) |
| **OpenAI** | Réponses du chatbot IA | Contenu des messages du chatbot (anonymisé) |
| **Firebase (Google)** | Notifications push et analytics | Jeton FCM, événements d'usage agrégés |
| **Stripe** | Paiement par carte bancaire | Informations de paiement (traitées côté Stripe) |
| **Orange Money / Wave** | Paiement Mobile Money | Redirection sécurisée vers leurs plateformes |

Ces prestataires agissent en tant que sous-traitants et sont contractuellement tenus de protéger vos données.

---

## 4. Durée de conservation

| Donnée | Durée |
|---|---|
| Données de compte actif | Pendant toute la durée du compte |
| Historique de progression | 3 ans après la dernière activité |
| Journaux de sécurité | 12 mois |
| Données de paiement | 5 ans (obligation légale comptable) |
| Compte supprimé (soft delete) | 30 jours, puis suppression définitive |

---

## 5. Sécurité

- Chiffrement HTTPS sur toutes les communications
- Mots de passe hachés (bcrypt)
- Jetons JWT à courte durée de vie (15 min) avec rotation des refresh tokens
- Mécanisme anti-partage de compte (un seul appareil actif par session)
- Captures d'écran désactivées sur les contenus protégés (Android FLAG_SECURE, iOS overlay)
- Filigrane numérique (e-mail + date) sur tout le contenu pédagogique
- URLs des médias signées (TTL 15 min) — jamais accessibles sans authentification

---

## 6. Vos droits

Conformément à la réglementation applicable, vous disposez des droits suivants :

- **Accès** : obtenir une copie de vos données personnelles
- **Rectification** : corriger des données inexactes
- **Suppression** : demander la suppression de votre compte et de vos données
- **Opposition** : vous opposer au traitement de vos données à des fins d'intérêt légitime
- **Portabilité** : recevoir vos données dans un format structuré

Pour exercer ces droits, contactez-nous à l'adresse ci-dessous.

---

## 7. Cookies et stockage local

L'application mobile utilise un stockage sécurisé (`flutter_secure_storage`) pour les jetons d'authentification — jamais de stockage non chiffré. L'application web utilise des cookies `httpOnly` sécurisés pour les jetons.

---

## 8. Mineurs

TEKKIL est destiné aux candidats aux concours, généralement âgés de 18 ans et plus. Nous ne collectons pas sciemment de données concernant des mineurs de moins de 15 ans.

---

## 9. Modifications de la présente politique

Toute modification substantielle sera notifiée par e-mail et/ou notification dans l'application au moins 7 jours avant son entrée en vigueur. La date de dernière mise à jour est indiquée en tête de document.

---

## 10. Contact

Pour toute question relative à vos données personnelles :

**K-Edtech — TEKKIL**  
E-mail : ibrahimadev6@k-edtech.com  
