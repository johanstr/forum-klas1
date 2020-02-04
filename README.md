# PHP Lessen voor niveau 4 AO Klas 1
  
## Inleiding
Deze git-repository is bedoeld voor de lessen PHP voor niveau 4 AO klas 1. Hier vind je dus de bestanden waarmee je bijvoorbeeld kunt beginnen om een forum te bouwen in standaard PHP. Je kunt via een knop op deze pagina alles downloaden in een ZIP-bestand, maar beter is het op de volgende manier te doen:  
  
### Voor Windows systemen
* Download en installeer Git Bash van [Git Bash Link](http://git-scm.com/downloads)  
  
* Download en installeer XAMPP van [XAMPP (Webserver en Databaseserver)](http://apachefriends.org)  
  
* Start Git Bash  
Je krijgt dan een venster met een terminal (command-line omgeving) die lijkt op een Linux omgeving.  
  
* Tik in deze terminal de volgende opdracht  
Wanneer je XAMPP op de standaard manier hebt geïnstalleerd:  
```bash
cd /c/xampp/htdocs
```
  
Wanneer je XAMPP ergens anders hebt geïnstalleerd moet je het pad in bovenstaande opdracht aanpassen.  
  
* Tik daarna de volgende opdracht in de terminal in  
```bash
git clone https://github.com/johanstr/forum-klas1 forum
```
  
Met deze opdracht trek je alle code/bestanden binnen van de online repository op je eigen schijf en wordt de map **forum** aangemaakt voor je in de root van je webserver. In deze map vind je dan nog weer twee submappen met de namen **design** en **dev**  
  
* Start xampp-controlpanel en start via de panel de servers Apache en MySQL  
  
* Start je browser (bij voorkeur Firefox) en tik in de adresbalk het onderstaande adres in  
  
localhost/forum/design  
  
Hiermee krijg je de startpagina van het ontwerp te zien. Maar let op, dit is nog niet je werkende forum.  
  
### Hoe kun je steeds de updates van de lessen weer binnenhalen van GitHub?  
Om dat te doen ga je eerst naar de map **forum** op je lokale webserver (htdocs) en tik je daar de opdracht:  
```bash
git pull
```  

## Hoe zie je dan je echte forum?  
Je echte forum (die natuurlijk nog niet werkt, omdat je nog moet beginnen) zie je steeds door in de adresbalk van je browser het volgende adres in te tikken:  
  
localhost/forum/dev  
  
LET OP! Voorwaarde is wel dat je je lokale webserver (Apache) hebt draaien.  
  


## De mappen in deze repository
* design  
Bevat alle HTML, CSS en JavaScript bestanden die nodig zijn om ons forum vorm te geven in een browser. Maar de bestanden hier zijn niet bedoeld om hier met PHP je forum te gaan programmeren. De bestanden zijn het resultaat van voorwerk (namelijk je user interface klaar hebben staan voordat we gaan programmeren).  
  
* dev  
Alleen in deze map gaan we programmeren. Ook deze map heeft weer submappen, ieder met hun eigen doel/nut. In de map **dev** gaan we alle zichtbare pagina's in PHP bouwen. We maken hier geen **.html** bestanden meer, maar uitsluitend **.php** bestanden. Ook al zal een **.php** bestand uitsluitend HTML code bevatten.  
  


## Submappen in de map forum
* app  
In deze map maken tijdens het ontwikkelen van ons forum mappen aan en **.php** bestanden. Het zal tijdens de lessen duidelijk worden welke mappen we hier steeds aanmaken en welke PHP-bestanden in deze map geplaatst zullen worden. In deze map programmeren we heel veel.  
  
* css  
Hier plaatsen we alle CSS-bestanden uit de map design in.  
  
* fonts  
Hier plaatsen we alle fonts uit de map design in.  
  
* img  
Hier plaatsen we alle afbeeldingen uit de map design in.  
  
* js  
Hier plaatsen we alle JavaScript bestanden uit de map design in.  
  

## De database
In de repository (repo) vind je ook het bestand forum_klas1.sql. Met dit bestand kun je een database vullen met dummy data, zodat we tijdens het ontwikkelen van onze applicatie ook 
resultaten op het scherm zien.  
  
Start XAMPP, en dus start Apache en MySQL in XAMPP. Open daarna in de browser phpMyAdmin (dit is een beheerpaneel van de databaseserver) en maak hier een database aan met de naam **forum**.  
  
Importeer nu het bestand forum_klas1.sql.