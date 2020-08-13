# Coloration-d-images
* Projet de transformation d'une image au niveau de gris en couleur.
Deux méthodes ont été utilisées : 

* Transfer Learning à partir d'un VGG16. On utilise une technique de freezing pour empecher la modification des poids. 
Ces couches serviront d'encodage. On raccomode ces couches avec le décodeur (décrit plus bas)
* La seconde se base sur un convolutional auto-encodeur entrainé en parralèle d'un resnet18 v2
Le ResNet permet essentielement de guider le modèle vu qu'il a été entrainé au préalable sur ImageNet.

Enfin le decodeur se modélise à l'aide de couche de déconvolution (UpSampling des images).

![alt text](https://raw.githubusercontent.com/baldassarreFe/deep-koalarization/master/assets/our_net.png)
