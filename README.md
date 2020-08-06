# Coloration-d-images
Projet de transformation d'une image au niveau de gris en couleur.
Le modèle est basé sur un auto-encodeur entrainé par dessus un resnet18 qui sert de backbone via les poids d'ImageNet.
L'encodeur est constitué de neuronnes à convolutions et decodeur d'une modélisation de déconvolution (UpSampling des images).
