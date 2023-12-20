# deep_learning_project
Improving Techniques for Training GANs

We will use TensorFlow as the code in the paper guide.

# What it is expected to present ?

Prend le papier, regarder la methode donée, proposed methodes : pre entrainée la reseaux avec autoeconder, contrastive learning, CNN, etc.

N = 50 000
Train : 
BASELINE para rapport a comparer au methode - 100 images
train - val

**Trouver la meilleur combination de modeles pour l'entraînement de modeles, plus de learning rate, trouver la bonne architecture.**
Contrer sur Learning Rate, Batch, Size (taille de couche latente, padding ou pooling)/depth (filters).
Compromis entre la taille de couche et le profundour. 
- METRE UN EARLY STOP, arreter l'entraînement si la performance n'avance plus. 
- REENTRAINée 5 fois, moyenne et aprées un intervale de confiance. 

METHOD : N-100 images non labelesées 
train - val

Test :
- 10 000 images labellisées

- Tuning
  - Optuna, conseil : sur le BASELINE (package pour optimizer de maniere sample le modele)
    - For "objective" metric, faire sur le train pas sur le test.
    - Grid \ RandomSearch
    - Bayesian Search : prend plus de temps, marche mieux quand le espace de research est pas trop convexe, similaire un descendt du gradient.

OJO learning rate, taille de Kernel.

- *RESULTATS* centralisée :

Compare directement le baseline de modeles, tableaux, des choses que résumée bien. 

- AJOUTE a la fin code comentée.
  - Data-processing
  - le blouce d'entrainement
  - le modele
  - la search (plotée l'accuracy selon les parameters)
  - Capturée d'essenciel, a la soutenance pas de montrer le code.



# Out next meeting will be a discussion on Saturday 23/12/2023 at 22h00.
Tasks : 
- Understand the paper : what metrics they used for evaluate the model ?
- Make questions about it and makes suggestions for improve the training.
- If it is possible reorganize the code to apply it into our problem.
