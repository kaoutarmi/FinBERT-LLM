# FinBERT Sentiment Analysis 📊💼

Bienvenue dans ce projet d'analyse de sentiment sur les textes financiers utilisant **FinBERT**, un modèle pré-entraîné spécialement conçu pour l'analyse de données financières. Ce dépôt contient deux fichiers **notebooks** Jupyter principaux :

- **FineBert-demo.ipynb** : Démonstration de l'utilisation de FinBERT pour l'analyse de sentiment.
- **finetune.ipynb** : Fine-tuning du modèle FinBERT sur un jeu de données personnalisé.

## 📑 1. **FineBert-demo.ipynb**

### 🎯 **Objectif** :
Ce notebook est une démonstration pratique de l'utilisation de **FinBERT** pour l'analyse du sentiment dans les textes financiers. Il montre comment charger un modèle pré-entraîné et l'utiliser pour classer et analyser les sentiments dans les textes financiers.

### 🔍 **Sections principales** :
1. **Installation des dépendances** 🛠️ :
   - Ce notebook commence par l'installation des bibliothèques nécessaires comme `transformers` et `torch`, qui sont essentielles pour utiliser FinBERT.
   
2. **Chargement du modèle FinBERT** 🚀 :
   - Utilisation du modèle pré-entraîné `yiyanghkust/finbert-tone` disponible sur Hugging Face pour analyser les sentiments dans les textes financiers.

3. **Analyse des sentiments** 💬 :
   - Une fonction simple permet d'analyser le sentiment d'un texte financier donné (positif, négatif ou neutre).

4. **Interface utilisateur** 🖥️ :
   - Une interface interactive est créée pour permettre à l'utilisateur de saisir des textes financiers et d'obtenir instantanément l'analyse du sentiment.

5. **Classification des textes financiers** 📈 :
   - Les textes financiers sont classifiés en différentes catégories telles que "Risque", "Opportunité" et "Neutre".

6. **Extraction d'entités nommées (NER)** 🏦 :
   - Cette section montre comment extraire des entités financières, comme des noms d'entreprises ou d'actions, et analyser leur sentiment associé.

7. **Résumé des textes financiers** ✍️ :
   - Une fonction génère un résumé des textes financiers basé sur les sentiments analysés, pour permettre une compréhension rapide des points clés.

8. **Réponses aux questions spécifiques** ❓ :
   - Ce bloc définit une fonction permettant de répondre à des questions spécifiques posées à propos des textes financiers.

### 🚀 **Points clés** :
- Ce notebook est conçu pour être interactif et permet à l'utilisateur d'interagir avec FinBERT en temps réel pour analyser des sentiments et classer des textes financiers.
- Il est une excellente introduction pour ceux qui veulent comprendre et utiliser FinBERT pour des tâches de traitement du langage naturel dans le domaine financier.

---

## 📑 2. **finetune.ipynb**

### 🎯 **Objectif** :
Ce notebook est destiné à fine-tuner (affiner) le modèle **FinBERT** pour l'adapter à un jeu de données financier spécifique. Il guide à travers le processus de préparation des données, d'entraînement du modèle et d'évaluation des performances sur un ensemble de test.

### 🔍 **Sections principales** :
1. **Installation des dépendances** 🔧 :
   - Comme pour le premier notebook, ce fichier commence par l'installation des bibliothèques nécessaires pour le fine-tuning, notamment `transformers`, `torch`, et `datasets`.

2. **Chargement des données** 📂 :
   - Le fichier utilise un jeu de données personnalisé, ici un fichier CSV nommé `analysttone.csv`, qui contient des phrases financières étiquetées avec leurs sentiments (positif, négatif, neutre).

3. **Préparation des données** 🛠️ :
   - Les données sont divisées en ensembles d'entraînement, de validation et de test. Cette étape est cruciale pour évaluer correctement la performance du modèle.

4. **Chargement du modèle pré-entraîné FinBERT** 🏋️‍♂️ :
   - Le modèle FinBERT pré-entraîné est chargé à partir de Hugging Face (`yiyanghkust/finbert-pretrain`).

5. **Préparation des datasets** 📑 :
   - Cette section montre comment tokeniser les données pour les rendre compatibles avec le modèle FinBERT. C’est une étape indispensable avant l’entraînement.

6. **Définition des options d'entraînement** ⚙️ :
   - Les hyperparamètres de l’entraînement sont définis, y compris le taux d'apprentissage, la taille des lots et le nombre d'époques, pour optimiser la performance du modèle.

7. **Entraînement du modèle** 🏃‍♂️ :
   - Le modèle est entraîné sur les données d'entraînement, et son efficacité est évaluée à chaque époque en utilisant l'ensemble de validation.

8. **Évaluation sur l'ensemble de test** 📊 :
   - Après l'entraînement, le modèle est évalué sur un ensemble de test séparé afin de mesurer sa capacité à généraliser à de nouvelles données.

9. **Sauvegarde du modèle** 💾 :
   - Enfin, le modèle fine-tuné est sauvegardé, ce qui permet de l'utiliser pour des prédictions futures sans devoir le réentraîner.

### 🚀 **Points clés** :
- Ce notebook est plus technique et se concentre sur l'adaptation du modèle FinBERT à un jeu de données spécifique, ce qui est essentiel pour des cas d’utilisation personnalisés.
- Il montre comment fine-tuner un modèle pré-entraîné pour qu'il soit plus performant sur des données spécifiques.
- Il nécessite un environnement avec un GPU pour accélérer l'entraînement, surtout pour les grands jeux de données.

---

## 🚀 **Prérequis**

Avant d'exécuter ces notebooks, assurez-vous que les bibliothèques suivantes sont installées :

pip install transformers torch datasets
