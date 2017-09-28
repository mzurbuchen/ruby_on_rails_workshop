# Anleitung

Um am Ruby on Rails Workshop teilzunehmen, müssen einige Anforderungen erfüllt werden.
Hier ist eine Anleitung was es braucht und wie man es installiert.

## Vorraussetzungen

Wenn du am Ruby on Rails Workshop teilnehmen möchtest, müssen folgende Sachen vorinstalliert sein:

-Rails

-RVM

-Git

-Bundler

## Ruby

### Was ist Ruby?

Ruby ist eine objektorientierte Programmiersprache, die sich einfach andwenden und produktiv einsetzen lässt.
Die Syntax ist leicht zum Lesen und Schreiben.

## Rails

### Was ist Rails?

Ruby on Rails ist ein Web-Framework, dass auf Ruby basiert. Es wird zur Entwicklung von dynamischen und datenbankbasierten Web-Anwendungen gebraucht. Rails unterstützt Web-Entwickler bei der Entwicklung von Anwendungen mit zahlreichen Features, die für eine hohe Produktivität sorgen.

## RVM

### Was ist RVM?

RVM ist der Ruby Version Manager.
Er ermöglicht ein schnelles Wechseln zwischen verschiedenen Ruby Versionen.

### Installation

Damit du auf dem neuesten Stand bist, solltest du zuerst das System updaten.

`sudo apt update`

Public Key installieren um das Installationspaket zu überprüfen, damit die Sicherheit gewährleistet wird.

`gpg --keyserver hkp: //keys.gnupg.net --recv-Schlüssel 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB`

RVM mit Ruby installieren.

`\curl -L https://get.rvm.io | bash -s stable --ruby`

Falls der Befehl oben fehlgeschlagen ist, musst du zuerst noch den Public Key importieren.

`command curl -sSL https://rvm.io/mpapis.asc | gpg2 --import -`

Nochmals versuchen RVM mit Ruby zu installieren.

`\curl -L https://get.rvm.io | bash -s stable --ruby`

### Ruby Version installieren

Ruby Versionen anzeigen:

`rvm list known`

Die neueste Ruby version installieren:

`rvm get stable --autolibs=enable`

`rvm install ruby`

Eine bestimmte Ruby Version installieren:

`rvm install 1.9.3`

RVM installiert die verschiedenen Versionen im Homeverzeichnis.
Die Gems werden für jede Version separat im Homeverzeichnis abgelegt.

### Zwischen Ruby Versionen wechseln

Ruby Version als Standard setzen:

`rvm --default use ruby-2.4.1`

Ruby Version vom Betriebssystem als Standard setzen:

`rvm use system --default`

Eine Bestimmte Ruby Version als Standard setzen:

`rvm use 1.9.3`

Ruby Version die vom Betriebssystem zur Verfügung gestellt wird:

`rvm use system`

Ruby Version anzeigen:

`ruby -v`

Zeigt an welche Datei ausgeführt wird:

`which ruby`

## Git

### Was ist Git?

Git ist eine kostenlose Software für das versionieren und verwalten des Programmcodes.

### Installation

Git installieren:

`sudo apt install git-all`

## Bundler

### Was ist Bundler?

Bundler bietet eine Umgebung für Ruby-Projekte durch die Installation und Verfolgung der Gems und Versionen, die für das Projekt benötigt werden.

### Installation

Bundler installieren:

`gem install bundler`
