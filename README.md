
# Übung 22 - Collections


## 1. Aufgabe

Setzen Sie folgendes Klassendiagramm um:

<p align="center">
  <img src="/assets/images/UML1.png" alt="Bildbeschreibung" />
</p>

**Beschreibung der `Subject`-Klasse:**

- Eigenschaften: 
	- Im Konstruktor müssen die `set`-Methoden aufgerufen werden. 
	- Prüfen Sie alle Eigenschaften auf sinnvolle Werte. 

- Methoden: 
	- `toString()`: Überschreiben Sie die `toString()`-Methode. Geben Sie einen String zurück, welcher alle Eigenschaften beinhaltet. 

**Beschreibung der `Student`-Klasse:**

- Eigenschaften: 
	- Im Konstruktor müssen die `set`-Methoden aufgerufen werden. 
	- Erzeugen Sie die Map im Konstruktor.
	- Prüfen Sie alle Eigenschaften auf sinnvolle Werte. 

- Methoden: 
	- `addNote(Subject subject, double note)`: Fügt der Map einen neuen Eintrag mit den jeweiligen Werten hinzu.
	- `berechneAvgNote()`: Berechnet die Durchschnittsnote des Studenten. 
	- `compareTo(Student s)`: Überschreibt die `compareTo()`-Methode. Implementieren Sie dafür das Interface `Comparable`. vergleicht zwei Studenten anhand ihrer Durchschnittsnote. 
	- `toString()`: Überschreiben Sie die `toString()`-Methode. Geben Sie einen String zurück, welcher alle Eigenschaften beinhaltet. 

**Beschreibung der `StudentManagement`-Klasse:**
- Eigenschaften: 
	- Der Konstruktor soll `studentMap` initialisieren.
- Methoden:
	- `addStudent(Person p)`: Fügt Student `s` mit dem Studiengang `programm` der Map hinzu. **Achtung:** `programm` ist nicht das `subject`! 
	- `updateNote(Student student, Subject subject, double newNote)`: Aktualisiert die jeweilige Note eines Studenten im jeweiligen Subject.
	- `findStudentByMatrikelnummer(int matrikelnummer)`: Durchsucht die Map nach dem Studenten mit der jeweiligen Matrikelnummer und gibt diesen zurück. 
	- `printStudents()`: Gibt alle Studenten der Map, sortiert nach der Durchschnittsnote, aus. 

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Testen Sie Ihr Programm, indem Sie die Methoden aufrufen. 

## 2. Aufgabe

Setzen Sie folgendes Klassendiagramm um:

<p align="center">
  <img src="/assets/images/UML2.png" alt="Bildbeschreibung" />
</p>

**Beschreibung der `PrintJob`-Klasse:**

- Eigenschaften: 
	- Prüfen Sie alle Eigenschaften auf sinnvolle Werte. 

- Methoden: 
	- `toString()`: Überschreiben Sie die `toString()`-Methode. Geben Sie einen String zurück, welcher alle Eigenschaften beinhaltet. 

**Beschreibung der `PrintQueue`-Klasse:**
- Eigenschaften: 
	- Der Konstruktor soll `jobQueue` initialisieren.
- Methoden:
	- `addPrintJob(PrintJob pj)`: Fügt der Queue einen neuen `PrintJob` hinzu. 
	- `printNextJob()`: Druckt den nächsten Auftrag, wodurch dieser aus der Queue verschwindet. 
	- `displayQueue()`: Gibt die aktuelle Warteschlange aus.  

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Testen Sie Ihr Programm, indem Sie die Methoden aufrufen. 

## 3. Aufgabe

Schreiben Sie eine Methode, welche mittels HashMap die Anzahl gleicher Wörter in einem String zählt und speichert. Testen Sie Ihr Programm!
**Beispiel:** Java ist die aller, aller, aller beste Programmiersprache.
Das Wort aller kommt 3 mal vor. Alle anderen Wörter 1 mal.
