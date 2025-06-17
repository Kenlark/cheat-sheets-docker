# Qu'est-ce qu'une virtual machine ?

Une machine virtuelle c'est une simulation logicielle d'un ordinateur physique, en particulier les VM utilise un logiciel appelé _hyperviseur_. Elle permet de faire tourner un système d'exploitation et des applications comme si c'était un vrai ordinateur, mais à l'intérieur d'un autre ordinateur.

En d'autres termes, une machine virtuelle est un environnement isolé qui fonctionne comme un vrai ordinateur, mais qui est herbergé sur une machine physique grâce à un logiciel appelé _hyperviseur_.

## Illustration :

**[ Matériel physique (CPU, RAM, Disque...) ]**  
&nbsp; &nbsp; &nbsp; ↑  
**[ Hyperviseur (ex: VirtualBox, VMware, KVM) ]**  
&nbsp; &nbsp; &nbsp; ↑  
**[ VM 1 ]** &nbsp; **[ VM 2 ]** &nbsp; **[ VM 3 ]**  
**[ OS ]** &nbsp; &nbsp; &nbsp; **[ OS ]** &nbsp; &nbsp; &nbsp; **[ OS ]**  
**[ Apps ]** &nbsp; &nbsp; **[ Apps ]** &nbsp; &nbsp; **[ Apps ]**

