# Chiffrement de Mots Passe
#!/bin/bash

echo -e '\E[1;31;40m'
echo "             ***** premier chiffrement *****           "
read -p " tapez le nombre de caractere que vous voulez : " nombre
read -p "tapez une phrase ou lettre chiffre caractere speciaux : " pass
mdp=</dev/urandom tr -dc "$pass" | head  -c$nombre
echo
echo -e '\E[1;34;40m'  "$mdp" 
echo
echo "             ***** deuxième chiffrement *****           "
 
read -p " tapez le nombre de caractere que vous voulez : " nombre2
echo "INFO ! "
echo "recuperer votre premier chiffrement en copiant collant la ou votre curseur clignotent  pour effectuer le double chiffrage, puis appuyez (entrée). " 
read -p "  copie ton premier chiffrement . ici --> : " pass2
mdp1=</dev/urandom tr -dc "$pass2" | head  -c$nombre2
echo " "
echo " "
echo " "
echo $mdp1
echo
echo
echo "TERMINER"




