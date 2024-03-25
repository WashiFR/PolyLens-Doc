# Ajouter des objets manipulables

***

Grâce à MRTK, il est très facile d'ajouter des objets manipulables, prenons pour exemple un cube 3D d'Unity. Faite un clique droit sur le côté gauche de Unity (là où se trouve vos objets, caméra...), puis séléctionné `3D Object` &rarr; `Cube`, cela créera alors un cube 3D sur votre scène.

<figure markdown="span">
    ![Image title](../assets/images/developpement/creer_cube.png)
    <figcaption>Création d'un Cube 3D sur Unity</figcaption>
</figure>

Ensuite il ne vous reste plus qu'à ajouter le script `Object Manipulator` sur votre cube 3D et voilà, votre objet peux maintenant être manipulé avec le casque Hololens. 

!!! warning

    Pour que le script `Object Manipulator` fonctionne, il a besoin que l'objet possède un `Collider` (peut importe le type tant que cela correspond à la forme de l'objet). Lors de la création d'un cube 3D, Unity intègre déjà un `Box Collider` mais si vous créer un objet manipulable, n'oubliez pas d'ajouter un `Collider` à votre objet.

!!! info

    L'ajout de ce script ajoutera également un script `Constraint Manager` qui permet d'ajouter des contraintes de déplacement, taille, rotations... Pour plus d'onformation, consulter la [documentation](https://learn.microsoft.com/en-us/windows/mixed-reality/mrtk-unity/mrtk3-spatialmanipulation/packages/spatialmanipulation/object-manipulator) officiel.

<figure markdown="span">
    ![Image title](../assets/images/developpement/object_manipulator_script.png)
    <figcaption>Script `Object Manipulator`</figcaption>
</figure>