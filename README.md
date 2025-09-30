🌱 Mini SOC Personnel Conscient

Un projet open source qui transforme la cybersécurité en une expérience éthique, pédagogique et consciente.


---

🚀 Qu’est-ce que le Mini SOC Conscient ?

Le Mini SOC Personnel Conscient est une solution légère de cybersécurité conçue pour :

Détecter les anomalies réseau en temps réel (routeurs domestiques, petits environnements).

Expliquer chaque alerte de manière claire et compréhensible.

Agir de façon intelligente (isoler une IP, activer un kill switch, proposer des recommandations).

Enseigner en transformant chaque détection en une leçon de cybersécurité pour l’utilisateur.



---

🔐 Philosophie

Edge-first : toutes les données restent locales (Raspberry Pi, PC personnel).

Privacy by Design : aucune donnée n’est envoyée dans le cloud.

Éthique : un outil au service de l’utilisateur, pas des grandes plateformes.

Pédagogie : chaque alerte devient une explication, un apprentissage.


> « La cybersécurité doit être humaine, éthique et consciente. » — Azizi Mahdi




---

🧠 Architecture du Pipeline



1. Trafic réseau → capturé en temps réel (Zeek, tshark).


2. Isolation Forest → filtre rapide pour détecter les anomalies évidentes.


3. Autoencoder → analyse fine des anomalies pour réduire les faux positifs.


4. Dashboard Conscient → interface simple (vert/rouge + explications + actions).




---

🎯 Cas d’usage (MVP)

Premier cas concret testé : détection de compromission d’un routeur domestique.

DNS anormal 🚨

Connexion persistante suspecte 🕵️‍♂️

Port mapping UPnP inhabituel ⚡



---

📊 Roadmap

Phase 1 : Prototype MVP → Isolation Forest + interface simple.

Phase 2 : Optimisation → ajout de l’autoencoder, réduction des faux positifs.

Phase 3 : Pédagogie → explications claires + feedback utilisateur.

Phase 4 : Communauté → ouverture open source, contributions GitHub, workshops.



---

🛠️ Stack technique

Langage : Python 3

Capture réseau : Zeek, tshark

Détection : Scikit-learn (Isolation Forest), TensorFlow Lite (Autoencoder TinyML)

Dashboard : FastAPI (backend) + React + Tailwind (frontend, PWA)

Base locale : SQLite (stockage règles et apprentissage utilisateur)



---

📦 Installation (MVP)

1. Cloner le dépôt :

git clone https://github.com/votre-compte/mini-soc-conscient.git
cd mini-soc-conscient


2. Créer l’environnement virtuel :

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt


3. Lancer le dashboard :

uvicorn src.dashboard.app:app --reload


4. Ouvrir http://mini-soc.local dans le navigateur.




---

⚖️ Licence

Ce projet est distribué sous licence GPL v3.
Vous êtes libres de l’utiliser, de le modifier, et de le partager — à condition que toutes les versions restent libres et ouvertes.

Auteur original : Azizi Mahdi (L’Élève Conscient)


---

🌍 Contribution

Les contributions sont les bienvenues !

Ouvrez une Issue pour poser une question ou signaler un bug.

Proposez une Pull Request pour ajouter une fonctionnalité.

Participez à la discussion dans l’onglet Discussions.



---

✨ Mini SOC Conscient n’est pas seulement un projet de cybersécurité, c’est un mouvement d’apprentissage.
