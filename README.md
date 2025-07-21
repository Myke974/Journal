# Myke974 Journal
📘 "All my project logs, ideas, and progress notes — one file, real time."

📝 This repository is a running log of all my automation projects, AI experiments, and coding workflows.  
It captures progress, fixes, features, and lessons learned along the way.

## 🔔 for real Time please visit : [https://t.me/+PFjc4UllBb44ZDdk](https://t.me/+PFjc4UllBb44ZDdk) 💬📢

## 🔍 What's inside

- `Myke974_Journal.log`: The main timeline of events
- Organized by timestamp, each entry logs a meaningful update in my projects

## 🛠️ Purpose

To document my creative process, technical steps, and automation experiments — especially those done with N8N, Telegram bots, and AI tools.

## 📌 Date of creation : 19 July 2025 22:00 GMT+4

## 🗓️ 20 juillet 2025 – Présentation du workflow Watch MDP_Trading_974

📡 **Bot Telegram Automatisé : Watch MDP_Trading_974** 🔥📈  
Salut la team, ici Myke974 🙋‍♂️

Je vous présente un de mes outils préférés créés avec N8N :  
👉 **Watch MDP_Trading_974** — un bot Telegram intelligent pour le trading crypto/forex.

---

🧠 **Comment ça marche ?**

Ce workflow réagit automatiquement à mes messages Telegram contenant des commandes comme `[tier1]` ou `[tier2]` :  

- **[Tier1]** déclenche une analyse visuelle de graphiques de **TradingView** (via l’API `chart-img`)  
  → Il extrait la paire + l’intervalle, capture le graphique, puis fait une vérification IA avec **GPT-4o Vision** (gratuit via Puter.js)

- **[Tier2]** va plus loin : il applique une logique d’analyse personnalisée (ex: tendance ou cassure), parfois multi-échelle, toujours avec validation IA  

📥 Chaque message lancé déclenche un sous-workflow adapté, avec délais gérés automatiquement.

---

📸 **Les images de graphiques** sont générées via `chart-img.com` — outil gratuit que j’utilise en mode API.  
🧠 **L’analyse IA** est réalisée localement à l’aide de **GPT-4o Vision** embarqué (via navigateur automatisé) — sans dépenser un centime 💰

---

📦 **Résultats ?**  
Les messages finaux (textes ou images avec légende) sont envoyés automatiquement sur Telegram.  
🔄 Tout se fait en quelques secondes, sans aucune action manuelle.

---
## 🧠 Automatisation AI TradingView → Telegram (20/07/2025)

🎯 **Objectif** : publier automatiquement deux analyses Telegram basées sur mes alarmes TradingView, avec confirmation IA via GPT-4 Vision.

### 🔧 Workflow mis en place :
1. **Création manuelle de l’analyse sur TradingView (12h TF)** :
   - Ajout d’une alarme (`alarm`) avec un message simple (ex: `[tier1] XAUUSD 1h == BUY`) ou JSON complet.
   - Alarmes créées à la main après analyse POI, RSI, MACD, etc.

2. **Déclenchement automatisé sur N8N** :
   - Parsing du message → extraction `ticker`, `interval`, `action`, `exchange`.
   - Génération d’un graphique via `chart-img`.
   - 📤 Publication Telegram du **premier message** : formaté proprement avec horodatage GMT+4.

3. **20 minutes plus tard** :
   - Nouvelle capture du graphique.
   - Analyse IA via **GPT-4 Vision gratuit** (via navigateur, pas d’API).
   - 📤 Publication Telegram du **deuxième message** : résumé de l’analyse IA (BUY / SELL confirmé ?).

### 💡 Particularité :
- Même un texte simple (non JSON) est supporté grâce à un sous-flux JS qui reconstruit un JSON valide.
- Possibilité de gérer plusieurs types d’alarms (`tier1`, etc.).
- Escaping automatique des caractères spéciaux pour Telegram Markdown.

### ⚙️ Technologies utilisées :
- **TradingView**
- **Ubuntu Server**
- **N8N privé (subflows JS, GPT-4 prompt injection)**
- **chart-img (free)**
- **GPT-4 Vision via navigateur (free)**
- **Telegram Bot**


---

📔 Ce projet fait partie de mon journal technique : [Myke974_Journal](./Myke974_Journal.md)  
Je partage mes recherches autour de l’automatisation, IA, et finance décentralisée 💸

🙏 Merci à tous ceux qui me soutiennent.  
Un like, un partage ou un message fait toujours plaisir !

💰 Faire un don (XRP) :  
Wallet : `rNxp4h8apvRis6mJf9Sh8C6iRxfrDWN7AV`  
Tag : `470785736`  
Réseau : XRP Ledger

© 2025 Myke974. All rights reserved.  
This journal is private work. Do not reuse without permission.

---

© 2025 Myke974. All rights reserved.  
This journal is private work. Do not reuse without permission.
