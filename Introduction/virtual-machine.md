# Qu'est-ce qu'une virtual machine ?

Une machine virtuelle c'est une simulation logicielle d'un ordinateur physique, en particulier les VM utilise un logiciel appelé _hyperviseur_. Elle permet de faire tourner un système d'exploitation et des applications comme si c'était un vrai ordinateur, mais à l'intérieur d'un autre ordinateur.

En d'autres termes, une machine virtuelle est un environnement isolé qui fonctionne comme un vrai ordinateur, mais qui est herbergé sur une machine physique grâce à un logiciel appelé _hyperviseur_.

## Illustration :

[ Matériel physique (CPU, RAM, Disque...) ]
                ↑
[ Hyperviseur (ex: VirtualBox, VMware, KVM) ]
                ↑
[ VM 1 ]   [ VM 2 ]   [ VM 3 ]
[ OS ]     [ OS ]     [ OS ]
[ Apps ]   [ Apps ]   [ Apps ]
