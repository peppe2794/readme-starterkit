SecDevOps Flow Template
=======================

SecDevOps Flow Template è uno strumento capace di eseguire un flusso di continuous integration/continuous deployment integrando attività di sicurezza. L’intervento degli sviluppatori consisterà nel fornire quelle che sono le caratteristiche proprie dell’applicazione sviluppata ed un limitato set-up dei tool utilizzati, senza dover per ogni nuovo progetto implementare la logica necessaria a seguire la metodologia proposta.


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

###  SonarQube Scanner for Jenkins
![My image](https://i.ibb.co/rccGv0G/sonarqube-plugin.png)

###  Ansible Plugin
![My image](https://i.ibb.co/k110fDL/ansible-plugin.png)

```js
console.log("Questo è un esempio di blocco di codice")
```

## Documentazione
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
