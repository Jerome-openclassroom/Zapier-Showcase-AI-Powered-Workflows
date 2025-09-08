# ⚡ Zapier Showcase – Automatisations par IA

## Présentation

Ce dépôt est une vitrine de compétences Zapier : deux workflows simples (résumé + tri d’emails, analyse de sentiments) démontrent ma capacité à utiliser Zapier avec des intégrations IA et Google Workspace.
Il ne s’agit pas d’un projet de production, mais d’une démonstration destinée à illustrer mes compétences dans le domaine de l’automatisation.
---

## 🔹 Workflow 1 – Tri & Résumé des Emails → Google Sheets

![Workflow](tri_resume/workflow.png)

- **Trigger** : réception d’un email (Gmail).  
- **IA** : génération d’un résumé (Zapier AI).  
- **Formatter** : ajout de la date et de l’heure.  
- **Classification (Paths)** :  
  - Bulletin météo,  
  - Activité solaire (SIDC),  
  - Messages généraux.  
- **Sortie** : insertion du résumé dans le Google Sheet correspondant.  

### Exemples de rendus
- ![Météo](tri_resume/meteo.png)  
- ![SIDC](tri_resume/SIDC.png)  
- ![Vacances](tri_resume/vacances.png)  

---

## 🔹 Workflow 2 – Analyse de Sentiments → Google Docs

![Workflow](analyse_sentiments/workflow.png)

- **Trigger** : réception d’un email (Gmail).  
- **IA** : analyse de sentiments (Positif, Négatif, Neutre, Mixte).  
- **Formatter** : ajout de la date et de l’heure.  
- **Classification (Paths)** : chaque catégorie redirige vers un document distinct.  
- **Sortie** : insertion dans le Google Doc correspondant, avec Date + Label de sentiment + Texte original.  

### Exemple de paramétrage
- ![Node IA](analyse_sentiments/node_IA.png)  
- ![Node Google Docs](analyse_sentiments/node_google_doc.png)  

### Exemple de rendu
- ![Rendu sentiment](analyse_sentiments/rendu.png)  

---

## 💾 Arborescence

```
zapier_showcase/
├── README.md                          # Version en français
├── README_en.md                       # English version
│
├── analyse_sentiments/                # Workflow analyse de sentiments
│   ├── node_google_doc.png            # Détails paramétrage node Google Docs
│   ├── node_IA.png                    # Paramétrage node IA
│   ├── rendu.png                      # Exemple de texte classé avec label
│   ├── workflow.png                   # Vue générale du workflow
│   └── system_prompt.txt              # Prompt système du node IA
│
└── tri_resume/                        # Workflow tri & résumé d’emails
    ├── meteo.png                      # Exemple rendu météo
    ├── vacances.png                   # Exemple rendu vacances
    ├── SIDC.png                       # Exemple rendu activité solaire
    ├── node_IA.png                    # Paramétrage node IA
    ├── node_google_sheet.png          # Paramétrage node Google Sheets
    ├── workflow.png                   # Vue générale du workflow
    └── system_prompt.txt              # Prompt système du node IA
```

---

👉 Ces workflows ne sont pas fournis en blueprint Zapier (limitation de la version d’essai), mais les **captures d’écran et prompts** permettent de reproduire chaque étape.
