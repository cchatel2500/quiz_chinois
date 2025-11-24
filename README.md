# 🀄 Quiz Chinois

Application web d’apprentissage interactif du chinois (caractères, pinyin, traduction) avec gestion de score, historique, coloration dynamique et options configurables.

---

## 🚀 Fonctionnalités principales
### 🔤 Modes d’apprentissage

  -	Chinois → Pinyin (mode par défaut)

  - Chinois → Français

  -	Pinyin → Chinois

  -	Français → Chinois

### 📁 Import de fichiers CSV

Le fichier CSV doit comporter au minimum 3 colonnes :

  1.	Chinois

  2. Pinyin

  3. Français

Contraintes :

  -	Les colonnes supplémentaires sont ignorées

  -	Les lignes avec moins de 3 colonnes sont écartées

  -	Encodage UTF-8 recommandé


### 🎯 Quiz intelligent

  -	Présentation aléatoire des mots

  -	Score total + score par question

  -	Nombre de tentatives affiché

  -	Coloration dynamique du pinyin pendant la saisie

  -	Coloration caractère ↔ syllabe

  -	Traduction optionnelle

  -	Bouton Vérifier

  -	Bouton Suivant

  -	Bouton Devine (aide pénalisante)

### 🎨 Coloration dynamique

  -	Zone de saisie :

  -	vert si correct

  -	rouge dès divergence

  -	Affichage caractère → pinyin avec couleur syllabe par syllabe

### 📜 Historique des 10 dernières réponses

  -	Réponses OK / KO

  -	Chinois / Pinyin / Français

  -	Clic : afficher / replier (sans effacer)

### 📊 Statistiques

  -	Score global

  -	Pourcentage

  -	Nombre d'essais

  -	Réinitialisation via les options

---

### ⚙️ Options (panneau latéral coulissant)

  -	Afficher / masquer la traduction

  -	Activer / désactiver la coloration dynamique

  -	Définir le séparateur pour les traductions françaises

  -	Définir le guillemet CSV

  -	Réinitialisation du score et des statistiques

  -	Imposer le rechargement d’un fichier CSV

---


## 💾 Format CSV attendu
### Exemple valide

```csv 
Chinois,Pinyin,Français

你好,nihao,Bonjour

因为,yinwei,Parce que

天气,tianqi,Temps; météo
```

### Notes

  -	Format UTF-8 conseillé

  -	Une colonne peut contenir plusieurs sens (ex : météo; temps)

  -	Les guillemets CSV "..." sont supportés

  -	Colonnes supplémentaires ignorées

  -	Une option permet de choisir :

    - le séparateur du français

    - le caractère de guillemet

---

### 📱 Optimisé pour smartphone / tablette

  -	Interface lisible

  -	Boutons tactiles

  -	Fonctionne offline

  -	Aucun serveur requis

---

### 🛠️ Installation

Aucune installation :

### ➡Ouvrir simplement quiz_chinois.html dans un navigateur moderne.

Compatibilité :

  -	Chrome

  -	Firefox

  -	Edge

  -	Safari

---

### 🧩 Fonctionnement interne
Structures :

  -	data[] → contenu du CSV

  -	stats[] → { shown, correct }

  -	history[] → 10 dernières réponses

Correspondances :

  -	1 syllabe pinyin ⇄ 1 caractère chinois

  -	Comparaison progressive

---

### 📌 Améliorations prévues

  -	🧠 Système SRS complet (type Anki)

  -	🔁 Mode répétition ciblée

  -	📈 Difficulté calculée automatiquement

  -	🗂 Export / import des stats

  -	🧭 Historique étendu

  -	📱 Version PWA installable

---

### 🤝 Contributions

Suggestions, rapports de bugs, ajouts de fonctionnalités : bienvenus !

---

### 📄 Licence

MIT (modifiable selon besoins).

---

### 👤 Auteur

Projet initié par cchatel2500, enrichi avec l’aide de ChatGPT pour la logique JavaScript, l’ergonomie mobile et le design pédagogique.
---
