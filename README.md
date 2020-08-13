# Coloration-d-images
* Projet de transformation d'une image au niveau de gris en couleur.
Deux méthodes ont été utilisées : 

* Transfer Learning à partir d'un VGG16. On utilise une technique de freezing pour empecher la modification des poids. 
Ces couches serviront d'encodage. On raccomode ces couches avec le décodeur (décrit plus bas)
* La seconde se base sur un convolutional auto-encodeur entrainé en parralèle d'un resnet18 v2
Le ResNet permet essentielement de guider le modèle vu qu'il a été entrainé au préalable sur ImageNet.
![alt text](https://raw.githubusercontent.com/Anty45/Coloration-d-images/master/Koalarization.png)

Enfin le decodeur se modélise à l'aide de couche de déconvolution (UpSampling des images).


Source du réseau de neuronnes : https://arxiv.org/pdf/1712.03400.pdf

Webographie :   
* https://medium.com/@emilwallner/colorize-b-w-photos-with-a-100-line-neural-network-53d9b4449f8d
* https://arxiv.org/abs/1712.03400
* http://cs231n.stanford.edu/reports/2016/pdfs/219_Report.pdf
