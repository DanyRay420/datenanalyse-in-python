
# Histogramm

Zeichne ein Histogramm der Lebenserwartung für das Jahr 2015. Da uns `pandas` die meiste Arbeit abnimmt, werden wir die Gelegenheit dazu nutzen, das Diagramm möglichst hübsch zu gestalten.

### Schritt 1

Da die Aufbereitung der Daten sich nicht sonderlich von der letzten Übung unterscheidet, kannst Du die Daten und den Code wiederverwenden.

Sorge dafür, daß Du die Lebenserwartung für das Jahr 2015 in einem DataFrame `lifeexp` hast.

### Schritt 2

Zeichne ein Histogramm mit den Standardeinstellungen.

    import pylab as plt

    plt.figure()
    plt.hist(lifeexp['spaltenname'])
    plt.savefig('histo.png')

### Schritt 3

Probiere unterschiedliche Werte für die Klassenanzahl aus. Wähle jeweils einen der folgenden Befehle und ersetze den vorher ausgeführten:

    plt.hist(lifeexp['spaltenname'], 5)
    plt.hist(lifeexp['spaltenname'], 10)
    plt.hist(lifeexp['spaltenname'], 20)

Entscheide Dich für einen aussagekräftigen Wert.


### Schritt 3

Nun werden wir das Diagramm verschönern.

Beschrifte das Diagramm. Verwende dazu vor dem Abspeichern die Funktionen:

* plt.title('text')
* plt.xlabel('text')
* plt.ylabel('text')


### Schritt 4

Stelle über die Funktion `plt.axis` den Bildausschnitt ein.

    plt.axis([0.0, 0.0, 150.0, 1.0)

Finde passende Zahlen und setze diese in den obigen Befehl ein.


### Schritt 5

Probiere nacheinander folgende optionale Parameter der Funktion `plt.hist` aus:

    facecolor='green',
    facecolor='#ff0000',
    alpha=0.75,
    histtype='bar',

Die Parameter werden in den Aufruf von `plt.hist` am Ende angefügt.

### Schritt 6

Lege die Auflösung beim Schreiben fest.

    plt.savefig('histo.png', dpi=150)

Probiere auch, das Diagramm als SVG-Grafik abzuspeichern, indem Du die Endung `.svg` angibst. Welche Vor- und Nachteile haben die Formate PNG und SVG?


### Schritt 7

Schreibe 3 Dinge auf, die Du noch am Histogramm verändern / verbessern möchtest. 
