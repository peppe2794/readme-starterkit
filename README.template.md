SecDevOps Flow Template
=======================

SecDevOps Flow Template è uno strumento capace di eseguire un flusso di continuous integration/continuous deployment integrando attività di sicurezza. L’intervento degli sviluppatori consisterà nel fornire quelle che sono le caratteristiche proprie dell’applicazione sviluppata ed un limitato set-up dei tool utilizzati, senza dover per ogni nuovo progetto implementare la logica necessaria a seguire la metodologia proposta.
Il risultato è costituito da una serie di report riguardanti la valutazione dell'ambiente configurato, l'attivià testing dinamico eseguita e la qualità del codice prodotto. Tali report sono messi a disposizione in formato html, grazie ad essi è possibile realizzzare una valutazione complessiva sullo stato dello sviluppo prima di rilasciare l'applicazione in ambiente operativo.


# Fasi e Strumenti

![My image](https://i.ibb.co/qkGN3cC/Immagine2.png)

# Indice

- [Requisiti](#Requisiti)
- [Set-up Plugin in Jenkins](#set-up-plugin-in-jenkins)
- [Manutenzione](#manutenzione)
- [Licenza](#licenza)

# Requisiti
  1) Jenkins Server, con i seguenti plugin e tool installati:
      - Ansible Plugin
      - Docker Pipeline
      - GitHub
      - Kubernetes Continuous Deploy
      - SonarQube Scanner for Jenkins
      - SSH Pipeline Steps
      - Teraform Plugin
      - Docker
      - Ansible
      - Chef-InSpec
   
  2) Distro Kali-Linux

  3) Proxmox Server
      - Template da clonare con Cloud-Init abilitato
  
  4) SonarQube Server
  
  
# Set-up Plugin in Jenkins
Dalla Dashboard di Jenkins recarsi in manage Jenkins -> Global Tool Configuration per configurare i plug-in

###  SonarQube Scanner for Jenkins
![My image](https://i.ibb.co/rccGv0G/sonarqube-plugin.png)

###  Ansible Plugin
![My image](https://i.ibb.co/k110fDL/ansible-plugin.png)


###  Terraform Plugin
![My image](https://i.ibb.co/S3zQqY2/terraform-plugin.png)

### Integrazione SonarQube
Per Integrare SonarQube vi è bisogno di inserire il Server authentication token in Jenkins:
  1. Eseguire il Login nel proprio SonarQube Server e dalla barra utente Recarsi in My Account –> Security –> Generate Token
  2. Eseguire il login nel proprio Jenkins Server e recarsi in Manage Jenkins –> Configure Systems –> SonarQube Serverse:
      - Name : SonarQube
      - Server URL : indirizzo IP del sonar Server
      - Server authentication token creando delle nuove credenziali di tipo 'SecretText'
![My image](https://i.ibb.co/tLFKL41/sonarqube-token.png)


```js
console.log("Questo è un esempio di blocco di codice")
```

# Guida all'uso
Per poter utilizzare il template, una volta effettuato il Fork, bisogna inserire i parametri necessari al completamento di esso.
In particoalre i file su cui bisogna agire sono:
  - Provisioning
      - resource.tf
      - provider.tf
  - hosts
  - Microservice Files
      - Jenkinsfile
  - Jenkinsfile 
  - version.txt

### Link a documentazione esterna 

# Come contribuire

## Installare le dipendenze di sviluppo

## Struttura del progetto

## Community

### Code of conduct

### Responsible Disclosure

### Segnalazione bug e richieste di aiuto

# Manutenzione 

# Licenza 

## Licenza generale 

## Autori e Copyright

## Licenze software dei componenti di terze parti
