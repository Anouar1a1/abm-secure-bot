# 🛡️ Secure HR Agent - Hackathon GenAI & Agentic AI 2025

**Une IA Agentique autonome et "Secure-by-Design" pour révolutionner la gestion RH.**

> 🏆 Projet réalisé dans le cadre du Hackathon National GenAI & Agentic AI (Capgemini Maroc).

---

## 📖 À propos du projet

**Secure HR Agent** est un assistant intelligent intégré à Microsoft Teams qui permet aux employés de consulter leurs informations RH (solde de congés, salaire, etc.) de manière autonome.

Contrairement aux chatbots classiques, notre solution est **Agentique** (elle agit via des outils) et met la priorité absolue sur la **Cybersécurité** et la protection des données (Loi 09-08).

### ✨ Fonctionnalités Clés
* **Agentique (Function Calling) :** Interrogation en temps réel d'une base de données RH simulée.
* **Zero-Trust Architecture :**
    * 🛡️ **MFA Contextuel :** Demande dynamique d'un Code PIN pour les données sensibles.
    * 🔒 **Sanitization :** Nettoyage des entrées utilisateurs (Regex) contre les injections.
    * 🙈 **Privacy First :** Anonymisation des données avant envoi au LLM (Google Gemini).

---

## 🛠️ Architecture Technique

* **Core AI :** Google Gemini 1.5 Flash (Optimisé pour la latence et les Outils).
* **Backend :** Python 3.10+, Flask.
* **Interface :** API REST compatible Microsoft Teams (Bot Framework).
* **Sécurité :** Gestion des secrets (`.env`), RBAC (Role-Based Access Control).

---

## 🚀 Installation & Démarrage

Suivez ces instructions pour lancer le projet en local (Linux/Mac/Windows).

### 1. Prérequis
* Python 3.8 ou supérieur installé.
* Une clé API Google Gemini (AI Studio).

### 2. Installation
Clonez ce dépôt (ou dézippez l'archive) et installez les dépendances :

```bash
# Créer un environnement virtuel (Recommandé)
python3 -m venv venv
source venv/bin/activate  # Sur Windows : venv\Scripts\activate

# Installer les librairies
pip install -r requirements.txt
