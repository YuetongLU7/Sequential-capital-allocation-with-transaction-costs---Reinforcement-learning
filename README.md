# Allocation séquentielle de capital avec coûts de transaction

## Description
Ce projet étudie l’allocation d’un portefeuille à temps discret avec coûts de transaction.

Deux approches sont considérées :
- **Programmation dynamique (DP)** sur un modèle binomial simplifié (Value Iteration).
- **Apprentissage par renforcement (RL)** avec entraînement d’un agent PPO sur un environnement de type Gym.

## Contenu
- `notebooks/` : notebooks Jupyter (DP, PPO, visualisations)  

## Installation
Installer les dépendances principales :

```bash
pip install numpy matplotlib pandas stable-baselines3 gymnasium gym
```

Puis ouvrir les notebooks et exécuter les cellules dans l’ordre.

## Conclusion
Les résultats dépendent des graines aléatoires (seed) et des paramètres du marché.

Avec coûts de transaction, l’agent PPO ne dépasse pas toujours un actif Buy-and-Hold, mais peut mieux résister aux chocs de marché.