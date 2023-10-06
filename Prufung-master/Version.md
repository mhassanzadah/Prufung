# Version Control Systems (VCS)

Version Control Systems (VCS) sind Software-Tools, die entwickelt wurden, um Änderungen an Dateien über die Zeit zu verfolgen, sodass Sie zu früheren Versionen zurückkehren können, wenn etwas schief geht, und um Zusammenarbeit zwischen verschiedenen Personen in einem Entwicklungsprojekt zu ermöglichen. Es gibt verschiedene Arten von VCS, darunter **lokale, zentrale und verteilte Versionskontrollsysteme**.

## Arten von Version Control Systems:

### 1. **Lokale Version Control Systems:**
   - Speichert Änderungen an Dateien in einer Datenbank auf dem lokalen System.
   - Ein einfaches Beispiel ist das regelmäßige Erstellen von Datei-Backups.

### 2. **Zentrale Version Control Systems:**
   - Ein zentraler Server speichert alle Dateien und Änderungen.
   - Benutzer checken Dateien vom Server aus und speichern Änderungen wieder dort ab.
   - Bekanntes Beispiel: **Apache Subversion (SVN)**.

### 3. **Verteilte Version Control Systems:**
   - Jeder Benutzer hat eine lokale Kopie des gesamten Repositorys.
   - Änderungen können lokal gespeichert und dann mit anderen Repositories synchronisiert werden.
   - Bekannte Beispiele: **Git, Mercurial, Bazaar**.

## Zweck von Version Control Systems:

1. **Verlauf nachverfolgen:**
   - Verfolgung von Änderungen an Dateien im Laufe der Zeit, einschließlich wer, wann und welche Änderungen vorgenommen hat.

2. **Zusammenarbeit erleichtern:**
   - Mehrere Personen können gleichzeitig an verschiedenen Teilen desselben Projekts arbeiten, ohne sich gegenseitig zu behindern.

3. **Problemlösung erleichtern:**
   - Ermöglicht das einfache Rückgängigmachen von Änderungen, wenn Fehler auftreten oder Code nicht wie erwartet funktioniert.

4. **Branching und Merging:**
   - Ermöglicht das Erstellen von Zweigen (Branches) für die parallele Entwicklung neuer Features, die dann wieder in den Hauptzweig (Master) integriert werden können (Merge).

## Wie arbeitet man damit?

Die Grundprinzipien der Arbeit mit VCS, insbesondere mit Git, sind wie folgt:

1. **Repository erstellen:**
   - Ein zentrales Repository erstellen, in dem der Code und die Dateien gespeichert werden.

2. **Clone (Klonen) des Repositorys:**
   - Lokale Kopie des Repositorys auf dem eigenen Computer erstellen.

   ```bash
   git clone <repository-url>
   ```

3. **Branch erstellen:**
   - Einen neuen Branch erstellen, um an einer neuen Funktion zu arbeiten.

   ```bash
   git branch <branch-name>
   git checkout <branch-name>
   ```

4. **Änderungen vornehmen:**
   - Code bearbeiten oder neue Dateien hinzufügen.

5. **Änderungen erfassen (Stage) und committen:**
   - Änderungen, die für den Commit vorgemerkt wurden, commiten.

   ```bash
   git add <file>
   git commit -m "Commit-Nachricht"
   ```

6. **Zum Hauptzweig zurückkehren und Änderungen integrieren:**
   - Zum Hauptzweig (Master) zurückkehren und die Änderungen aus dem Feature-Branch integrieren.

   ```bash
   git checkout master
   git merge <branch-name>
   ```

7. **Änderungen hochladen:**
   - Die Änderungen zum zentralen Repository hochladen (pushen).

   ```bash
   git push origin master
   ```

Dies sind grundlegende Schritte, um mit Git zu arbeiten. Es gibt viele fortgeschrittenere Funktionen und Workflows, die je nach den Anforderungen des Projekts genutzt werden können.

Hinweis: Die genauen Befehle können je nach dem verwendeten VCS variieren. Die oben gezeigten Befehle sind spezifisch für Git, das eines der am häufigsten verwendeten verteilten Versionskontrollsysteme ist.
