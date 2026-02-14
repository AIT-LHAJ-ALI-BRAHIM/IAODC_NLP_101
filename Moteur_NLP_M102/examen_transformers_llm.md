# Examen : Manipulation des Transformers et Exploration des LLM
## Niveau : Débutant

**Durée suggérée :** 3 heures  
**Note totale :** 100 points

---

## Partie 1 : Questions Théoriques (30 points)

### Question 1 (5 points)
Expliquez en vos propres mots ce qu'est un modèle Transformer et quelle innovation majeure il apporte par rapport aux architectures précédentes (RNN, LSTM).

### Question 2 (5 points)
Qu'est-ce que le mécanisme d'attention (attention mechanism) ? Pourquoi est-il crucial dans l'architecture Transformer ?

### Question 3 (5 points)
Définissez les termes suivants :
- **Token**
- **Embedding**
- **Context window**
- **Temperature**
- **Top-k sampling**

### Question 4 (5 points)
Quelle est la différence entre :
- Un modèle encoder-only (comme BERT)
- Un modèle decoder-only (comme GPT)
- Un modèle encoder-decoder (comme T5)

Donnez un exemple d'usage pour chacun.

### Question 5 (10 points)
Expliquez le processus de pré-entraînement et de fine-tuning d'un LLM. Pourquoi ces deux étapes sont-elles importantes ?

---

## Partie 2 : Manipulation Pratique avec Hugging Face (40 points)

### Exercice 1 : Chargement et utilisation d'un modèle (15 points)

Écrivez un script Python qui :
1. Charge le modèle `distilbert-base-uncased-finetuned-sst-2-english`
2. Analyse le sentiment des phrases suivantes :
   - "I love this movie, it's amazing!"
   - "This product is terrible and broken."
   - "The weather is okay today."
3. Affiche les résultats avec les scores de confiance

**Bibliothèques autorisées :** transformers, torch

### Exercice 2 : Génération de texte (15 points)

Créez un script qui :
1. Charge le modèle `gpt2`
2. Génère du texte à partir du prompt : "Once upon a time in a magical forest,"
3. Expérimente avec différents paramètres :
   - `temperature` : 0.7, puis 1.5
   - `max_length` : 50, puis 100
   - `top_k` : 50
4. Compare et commente les résultats obtenus avec différentes températures

### Exercice 3 : Tokenization (10 points)

Écrivez un code qui :
1. Charge le tokenizer de `bert-base-uncased`
2. Tokenise la phrase : "Transformers are revolutionizing natural language processing!"
3. Affiche :
   - Les tokens
   - Les IDs des tokens
   - Le texte décodé à partir des IDs
4. Expliquez ce qui se passe avec les mots composés ou inconnus

---

## Partie 3 : Exploration et Analyse (20 points)

### Exercice 4 : Comparaison de modèles (10 points)

Comparez les performances de deux modèles différents sur la même tâche de question-réponse :
- `distilbert-base-cased-distilled-squad`
- `bert-large-uncased-whole-word-masking-finetuned-squad`

**Contexte :** "The Eiffel Tower is located in Paris, France. It was completed in 1889 and stands 330 meters tall."

**Questions :**
1. "Where is the Eiffel Tower located?"
2. "When was it completed?"
3. "How tall is the Eiffel Tower?"

Analysez :
- La précision des réponses
- Le temps d'inférence
- Les scores de confiance

### Exercice 5 : Prompt Engineering (10 points)

Pour la tâche de génération de texte, testez différents prompts pour obtenir :
1. Un poème sur l'intelligence artificielle
2. Une explication technique du machine learning
3. Une recette de cuisine

Documentez :
- Les prompts utilisés
- Les résultats obtenus
- Les ajustements nécessaires pour améliorer la sortie

---

## Partie 4 : Mini-Projet (10 points)

### Projet : Classificateur de sentiment personnalisé

Créez une petite application qui :
1. Prend en entrée un texte de l'utilisateur
2. Utilise un modèle de votre choix pour analyser le sentiment
3. Affiche le résultat de manière conviviale
4. Permet de traiter plusieurs textes successivement

**Bonus (+5 points) :** Ajoutez une interface simple avec Gradio ou Streamlit

---

## Critères d'évaluation

### Code (50%)
- Fonctionnalité : Le code s'exécute sans erreur
- Qualité : Code propre, commenté, bien structuré
- Utilisation correcte des bibliothèques

### Compréhension théorique (30%)
- Précision des réponses
- Clarté des explications
- Utilisation appropriée du vocabulaire technique

### Analyse et réflexion (20%)
- Profondeur de l'analyse
- Pertinence des observations
- Esprit critique

---

## Ressources autorisées

- Documentation officielle de Hugging Face : https://huggingface.co/docs
- Documentation PyTorch/TensorFlow
- Vos notes de cours

**⚠️ Important :** Le plagiat de code trouvé en ligne sans compréhension est sanctionné. Vous devez être capable d'expliquer chaque ligne de votre code.

---

## Barème détaillé

| Partie | Points | Description |
|--------|--------|-------------|
| Partie 1 | 30 | Questions théoriques |
| Partie 2 | 40 | Manipulation pratique |
| Partie 3 | 20 | Exploration et analyse |
| Partie 4 | 10 | Mini-projet |
| **Total** | **100** | |
| Bonus | +5 | Interface utilisateur |

---

## Conseils pour réussir

1. **Lisez attentivement** chaque question avant de commencer
2. **Testez votre code** régulièrement
3. **Commentez** votre code pour montrer votre compréhension
4. **Gérez votre temps** : ne restez pas bloqué trop longtemps sur une question
5. **Vérifiez** vos réponses avant de soumettre

**Bonne chance ! 🚀**
