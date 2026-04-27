Viene allestito un ambiente per arrivare a provare una versione didattica semplificata di IaC, usando OpenTofu e Docker.

## Ambiente
Installare/verificare il SW necessario.  

'OpenTofu'  

Da PowerShell:  
~$ winget install --exact --id=OpenTofu.Tofu  

Chiudere e riaprire PowerShell:  
~$ tofu version  

'Docker' gia installato  

## Esecuzione
Clonare il repository in locale.

Struttura del progetto:  

opentofu-uvicorn/  
│  
├─ app/  
│  ├─ main.py  
│  └─ requirements.txt  
│  
├─ Dockerfile  
├─ main.tf  
└─ outputs.tf  

Il progretto ha un branch.

In questa fase si lancia l’app main.py con OpenTofu.  
Spostarsi nella cartella opentofu-uvicorn, eseguire i comandi:  
~$ tofu init  
~$ tofu plan  
~$ tofu apply  

