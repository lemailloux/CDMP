#!/bin/bash
 
REP_TRACES=/var/log
UID_ROOT=0
LIGNES=50
E_XCD=66
E_NONROOT=67
clear
 
if [ $UID != $UID_ROOT ]
then
  clear
  echo "ACCES REFUSE : Vous devez étre en mode superutilisateur pour exécuter ce script intégration PHP"
  exit $E_NONROOT
 
else
  clear
<<<<<<< HEAD
  echo "Vous etes le superutilisateur"
  echo ""
=======
  echo "Vous etes le superviseur"
  

  echo "************************************************************************************************************************************************************"
  clear
  cd $REP_TRACES
  cat /dev/null > messages
  cat /dev/null > wtmp
  echo "journaux nettoyés."
fi
 
exit
