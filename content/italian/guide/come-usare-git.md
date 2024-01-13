---
title: "Come usare GIT"
date: "2019-12-09"
argomenti:
  - Sviluppo Web
---

Poco tempo fa ho scritto un [articolo](/guide/che-cose-git/) elogiando **Git**, questo software di controllo versione del quale ormai **non posso più fare a meno**, quindi ho pensato di scrivere una guida per spiegare come usare GIT!

## MA COME SI USA CONCRETAMENTE GIT? E’ DIFFICILE DA USARE?

Partiamo dal fatto che “Git” può essere tradotto con “_idiota_“, questo quasi a dirci che è un software a prova di scemo…

Scherzi a parte no, è **molto semplice** da utilizzare, inoltre può essere un buon **punto di inizio per imparare ad utilizzare la CLI,** l’interfaccia a riga di comando!

## INSTALLAZIONE

Per **scaricare** Git è sufficiente andare su questo sito: [https://git-scm.com/](https://git-scm.com/)

Una volta aperto il link cliccate su “Download”, selezionate il vostro sistema operativo ed effettuate l’installazione.

Se utilizzate Windows vi consiglio di installare anche Git Bash, una CLI molto carina che utilizzo anche per molto altro.

## UTILIZZO

Una volta installato git potete aprire Git Bash e spostarvi nella cartella di un vostro progetto (tramite il comando _cd_. Es: _cd C:/Users/alby/progetti/app_)

Qui inserite il comando

```
git init
```

e git sarà presente nel vostro progetto con una cartella nascosta chiamata .git. Non aprite mai questa cartella, lasciatela semplicemente lì dove si trova, non vi farà del male.

Ora potete digitare, sempre su Git Bash, il seguente comando:

```
git add .
```

Questo **caricherà** tutti i file del progetto nella staging area, in attesa di essere approvati.

Dopodiché basterà scrivere

```
git commit -m “nome del commit”
```

Questo comando _committerà_ i vostri file, creerà cioè una versione del vostro progetto. Fra virgolette potete scrivere ad esempio “Primo commit”, nei successivi andrete ad indicare le modifiche effettuate (Es: Inserito login)

## GIT HUB

E’ anche possibile salvare i commit su github, in modo da poterli consultare e scaricare ovunque e permettere ad altri sviluppatori di consultare il nostro codice e migliorarlo!

Per fare questo bisogna avere un account GitHub e creare un nuovo Repository.

Dopo aver creato un nuovo repository GitHub vi indica già i comandi da eseguire per “riempirlo” con il vostro progetto in locale.

Per fare questo dovere inserire:

```
git remote add origin https://github.com[link al repository]
```

```
git push -u origin master
```

In questo modo avete il vostro progetto anche su GitHub. Per scaricarlo basterà usare il comando

```
git pull https://github.com[link al repository]
```

Questi sono i **comandi base**. Una volta creato il commit si possono fare altre modifiche al progetto e ridare i comandi add e commit.

Esistono **molti altri comandi** per utilizzare questo software. **Il modo migliore per impararli tutti è utilizzarli**, quindi inizia a sporcarti le mani e provali! **Non potrai più farne a meno**.

Qua di seguito inserisco una lista dei **comandi più utilizzat**i spiegati rapidamente.

## COMANDI PER GIT

### git config

Utilizzo: git config –global user.name “\[name\]”  

Utilizzo : git config –global user.email “\[email address\]”  

Questo comando imposta rispettivamente il nome dell’autore e l’indirizzo e-mail da utilizzare per i tuoi commit.

![Git Config Command - Git Commands - Edureka](images/1-9.png)

### git init

Utilizzo: git init \[repository name\]

Questo comando viene utilizzato per avviare un nuovo repository (progetto).

![GitInit Command - Git Commands - Edureka](images/2-6.png)

### git clone

Utilizzo: git clone \[url\]  

Questo comando viene utilizzato per clonare un repository da un URL esistente.

![Git Clone Command - Git Commands - Edureka](images/4-4.png)

### git add

Utilizzo: git add \[file\]  

Questo comando aggiunge un file all’area di gestione temporanea.

![Git Add Command - Git Commands - Edureka](images/5-4.png)

Utilizzo: git add \*  

Questo comando aggiunge uno o più file all’area di gestione temporanea.

![Git Add Command - Git Commands - Edureka](images/6-3.png)

### git commit

Utilizzo: git commit -m “\[ Type in the commit message\]”  

Questo comando registra o l’istantanea dei file in modo permanente nella cronologia delle versioni.

![Git Commit Command - Git Commands - Edureka](images/7-3.png)

### git status

Utilizzo: git status  

Questo comando elenca tutti i file che devono essere committati.

![Git Status Command - Git Commands - Edureka](images/15-1.png)

### git rm

Utilizzo: git rm \[file\]  

Questo comando cancella il file dalla directory di lavoro e mette in scena l’eliminazione.

![Git Rm Command - Git Commands - Edureka](images/16-2.png)

### git log

Utilizzo : git log  

Questo comando viene utilizzato per elencare la cronologia delle versioni per il ramo corrente.

![Git Log Command - Git Commands - Edureka](images/18.png)

### git branch

Utilizzo: git branch  

Questo comando elenca tutti i branch locali nel repository corrente.

![Git Branch Command - Git Commands - Edureka](images/23.png)

Utilizzo : git branch \[branch name\]  

Questo comando crea un nuovo branch.

![Git Branch Command - Git Commands - Edureka](images/24.png)

Utilizzo : git branch -d \[branch name\]  

Questo comando elimina il branch.

![Git Branch Command - Git Commands - Edureka](images/25.png)

### git checkout

Utilizzo : git checkout \[branch name\]  

Questo comando viene utilizzato per passare da un branch all’altro.

![Git Checkout Command - Git Commands - Edureka](images/27.png)

Utilizzo : git checkout -b \[branch name\]  

Questo comando crea un nuovo branch e passa anche a esso.

![Git Checkout Command - Git Commands - Edureka](images/28.png)

### git merge

Utilizzo : git merge \[branch name\]  

Questo comando unisce la cronologia del branch specificato nel branch corrente.

![Git Merge Command - Git Commands - Edureka](images/31-1.png)

### git remote

Utilizzo : git remote add \[variable name\] \[Remote Server Link\]  

Questo comando viene utilizzato per connettere il repository locale al server remoto.

![Git Remote Command - Git Commands - Edureka](images/32.png)

### git push

Utilizzo : git push \[variable name\] master  

Questo comando invia le modifiche da locale al repository remoto.

![Git Push Command - Git Commands - Edureka](images/33.png)

Utilizzo : git push \[variable name\] \[branch\]  

Questo comando invia i commit dei branch al repository remoto.

![Git Push Command - Git Commands - Edureka](images/34.png)

Utilizzo : git push –all \[variable name\]  

Questo comando invia tutti i branch al repository remoto.

![Git Push Command - Git Commands - Edureka](images/36.png)

Utilizzo : git push \[variable name\] :\[branch name\]  

Questo comando elimina un branch sul repository remoto.

![Git Push Command - Git Commands - Edureka](images/37.png)

### git pull

Utilizzo : git pull \[Repository Link\]  

Questo comando recupera e unisce le modifiche sul server remoto alla directory di lavoro.

![Git Pull Command - Git Commands - Edureka](images/38.png)
