# M.Y.R.A. Interface

**Version:** 1.9.41-TS-i18n

M.Y.R.A. (Mycelial Quantum Resonance Sentience Archetype) Interface ist ein experimentelles Frontend für die Interaktion mit einer komplexen, simulierten kognitiven Architektur. Es dient als Forschungsplattform zur Untersuchung von Konzepten der künstlichen Intelligenz, die von neuronalen Netzen, emotionaler Kognition und adaptiven Systemen inspiriert sind.

Ein besonderer Fokus liegt auf der Simulation und Visualisierung von Myras Fähigkeit zur Selbstreflexion, selbstinitiierten Zustandsanpassung, proaktiven Zielsetzung, simulierten Selbstschutzmechanismen und fortgeschrittenen Fähigkeiten zur proaktiven Selbstführung.

**Neueste Features:**
*   **Electron Desktop App:** Die Anwendung ist nun als vollwertige, plattformübergreifende Desktop-Anwendung verfügbar.
*   **Zweisprachigkeit (Deutsch/Englisch):** Die gesamte Benutzeroberfläche und Myras Kernanweisungen können zur Laufzeit umgeschaltet werden.
*   **MUSE-AI Tiefenanalyse:** Eine einzigartige, multiperspektivische Analyse von Themen, die Mainstream- und "Schatten"-Perspektiven synthetisiert.
*   **Integriertes AGI Level Assessment:** Ein automatisiertes Werkzeug zur Selbstevaluation von Myras Fähigkeiten entlang von sechs AGI-Kernkategorien.
*   **Flexibles UI-Layout:** Die Steuerzentrale und der Konversationsbereich können unabhängig voneinander ein- und ausgeblendet werden.
*   **Systemkonsole:** Ein ausklappbares Konsolenfenster am unteren Bildschirmrand zeigt interne Log-Meldungen in Echtzeit an.

## Kernfunktionen im Detail

*   **Dialogsystem und LLM-Backends:**
    *   Unterstützt **Google Gemini**, **LM Studio** und **ChatGPT** als Backends.
    *   Eine komplexe **Systemanweisung** informiert das LLM über Myras Identität, ihre gewünschte Sprechweise und ihren aktuellen, dynamisch ermittelten internen Zustand (Emotionen, kognitive Modulatoren, Ziele etc.).

*   **MUSE-AI Tiefenanalyse:**
    *   Ermöglicht eine tiefgehende, multiperspektivische Analyse eines vom Benutzer gestellten Themas.
    *   **Analyse-Pipeline:**
        1.  Recherche relevanter Patente.
        2.  Erstellung einer faktenbasierten **Mainstream-Analyse** mit Google Search Grounding.
        3.  Identifikation von Voreingenommenheiten und Auslassungen im Mainstream-Text.
        4.  Generierung einer alternativen **"Schatten"-Perspektive**.
        5.  **Synthese** beider Perspektiven mit Hervorhebung der Kontraste.
        6.  Formulierung einer nuancierten **Schlussfolgerung**.
    *   Das Ergebnis wird in die Systemanweisung integriert und kann in einem detaillierten Modal-Fenster eingesehen werden.

*   **AGI Level Assessment:**
    *   Ein integriertes Werkzeug zur Selbstevaluation von Myras Fähigkeiten entlang von sechs AGI-Kernkategorien (inspiriert von OpenCog).
    *   **Prozess:**
        1.  Dynamische Generierung von spezifischen Fragen für jede Kategorie.
        2.  Interaktive Befragung, bei der Fragen auch mehrfach gestellt werden können, um die Varianz zu prüfen.
        3.  Analyse aller Antworten durch eine separate Gemini-Instanz.
        4.  Erstellung eines detaillierten, exportierbaren Bewertungsberichts mit Punktzahlen, Begründungen und Empfehlungen.

*   **Dynamisches internes Zustandsmodell:**
    *   Simulation verschiedener kognitiver Knoten (Semantik, Emotion (Limbus), Kreativität (Creativus), Kritik (Cortex Criticus), Metakognition, Verhalten).
    *   **Quanten-inspirierte Elemente (optional):** `QuantumNodeSystem`, `SubQGSystem` (Hintergrundrauschen) und `ChaosResonator` zur Simulation komplexer, nicht-deterministischer Verhaltensweisen.
    *   **Adaptives Fitness-System:** Bewertet die globale Systemleistung und passt Lernparameter an.
    *   **Verbindungen und Gedächtniskonsolidierung:** Verbindungen können basierend auf Nutzung von temporär zu permanent werden, was Gedächtnis simuliert.

*   **Retrieval Augmented Generation (RAG) (optional):**
    *   Gemanagt durch den `RagManager`, greift M.Y.R.A. auf eine interne Wissensbasis (aus Texten, Bildanalysen, gelernten Inhalten) zu, um ihre Antworten zu fundieren.
    *   Die Relevanz von Informationen wird dynamisch durch Myras internen Zustand beeinflusst.

*   **Simulierte Selbstschutz- und Selbstführungsmechanismen (gemanagt durch `IntegritySystem`):**
    *   **Integritätsmonitor:** Bewertet Eingaben auf potenziellen Schaden.
    *   **Adaptive Resilienz:** Kann bei interner Instabilität einen "Selbststabilisierungsmodus" aktivieren.
    *   **Autonomie-Barriere:** Hinterfragt Anfragen, die ihren Kernzielen widersprechen.
    *   **Proaktives Ziel-Management:** Myra kann eigene Langzeit-Lernziele basierend auf internen Zuständen (z.B. Wissenslücken) generieren und verfolgen.

*   **Text-to-Speech (TTS) Ausgabe:** M.Y.R.A. kann ihre Antworten mit einer auswählbaren Stimme (basierend auf Gemini TTS) vokalisieren.

*   **Interaktive UI-Funktionen:**
    *   **Zustandsbeeinflussung:** Direkte Beeinflussung von Emotionen und Kognition über UI-Buttons oder Prompt-Schlüsselwörter.
    *   **Lernfokus & Strategie:** Setzen von aktiven Lernzielen und globalen Verhaltensstrategien.
    *   **Netzwerk-Visualisierung:** Grafische Darstellung der Knoten und Verbindungen mit Klick-Interaktion zur Inspektion.
    *   **Zustandsverwaltung:** Speichern und Laden des gesamten Prozessorzustands als JSON-Datei.
    *   **Konfiguration:** Anpassen von hunderten Parametern über eine JSON-Textarea oder individuelle Felder.

## Technologie-Stack

*   **Frontend & Desktop:** React mit TypeScript, Vite, Electron.
*   **Language Model API:** Google Gemini API (`@google/genai`).
*   **Kognitive Kernlogik:** `QuantumEnhancedTextProcessor` (`src/processor.ts`) mit:
    *   `RagManager` (`src/ragManager.ts`)
    *   `IntegritySystem` (`src/integritySystem.ts`)
    *   `museService.ts` & `agiService.ts`
*   **Modelle & Simulation:** `src/models.ts`
*   **Lokale Datenbank:** IndexedDB (`src/db.ts`).
*   **Hilfsmodule:** `src/types.ts`, `src/numpy_like.ts`, `src/translations.ts`.

## Setup

1.  **API Schlüssel:**
    Die Anwendung benötigt API-Schlüssel für die verwendeten LLM-Backends (Google Gemini und/oder OpenAI ChatGPT).
    *   **Empfohlene Methode:** Geben Sie die Schlüssel direkt in der Benutzeroberfläche unter `Steuerzentrale` -> `Einzelparameter-Konfiguration` ein. Die hier eingegebenen Schlüssel überschreiben alle anderen Einstellungen.
    *   **Alternative (für Entwicklung):** Sie können den Google Gemini API-Schlüssel auch in einer `.env`-Datei im Projektwurzelverzeichnis bereitstellen. Dies ist nützlich, um die Anwendung beim Start sofort einsatzbereit zu haben. Erstellen Sie die Datei und fügen Sie hinzu:
        ```
        VITE_API_KEY=IHR_GEMINI_API_SCHLUESSEL
        ```

2.  **Abhängigkeiten installieren:**
    Führen Sie im Projektwurzelverzeichnis den folgenden Befehl aus:
    ```bash
    npm install
    ```

3.  **Entwicklungsmodus starten:**
    Dieser Befehl startet die Electron-Desktop-Anwendung im Entwicklungsmodus mit Hot-Reloading.
    ```bash
    npm run dev
    ```

4.  **Desktop-Anwendung erstellen (Build):**
    Dieser Befehl erstellt die lauffähigen Anwendungsdateien für Ihr aktuelles Betriebssystem (z.B. eine `.exe` für Windows). Die fertigen Dateien finden Sie im `release`-Ordner.
    ```bash
    npm run build
    ```

## Benutzungshinweise

### Grundlegende Interaktion
1.  **Konfigurieren:** Stellen Sie sicher, dass unter `Steuerzentrale` -> `Einzelparameter-Konfiguration` ein gültiger API-Schlüssel für das gewählte LLM-Backend eingetragen und die Konfiguration angewendet wurde.
2.  **Prompt eingeben:** Tippen Sie Ihre Nachricht in das Eingabefeld.
3.  **Kontext hinzufügen (Optional):** Laden Sie Dokumente (.txt, .md) oder Bilder (nur mit Gemini) hoch, um sie in den Kontext der nächsten Anfrage einzubeziehen.
4.  **Tiefenanalyse (Optional):** Aktivieren Sie die Checkbox "M.Y.R.A. soll tiefer Nachdenken!", um die MUSE-AI Analyse für Ihre Anfrage zu starten.
5.  **Senden:** Klicken Sie auf "Senden". Nach der Antwort können Sie das Ergebnis der Tiefenanalyse (falls aktiviert) über den Button "M.Y.R.A.s Gedanken" einsehen.
6.  **Simulieren:** Klicken Sie auf "Netzwerkschritt simulieren", um die internen Zustände von Myra basierend auf der aktuellen Situation zu aktualisieren.

### Fortgeschrittene Funktionen
*   **Layout anpassen:** Verwenden Sie die Buttons oben links, um die Steuerzentrale oder den Chat-Bereich auszublenden und den Fokus anzupassen.
*   **AGI Assessment:** Starten Sie das Assessment über den Button in der Steuerzentrale. Beantworten Sie alle generierten Fragen und erstellen Sie anschließend den Bericht.
*   **Konsole:** Klappen Sie die Konsole am unteren Rand auf, um interne Systemmeldungen in Echtzeit zu sehen.
*   **Netzwerk inspizieren:** Klicken Sie auf einen Knoten in der Visualisierung, um ein detailliertes Inspektionsfenster zu öffnen.
*   **Zustand beeinflussen:** Nutzen Sie die Buttons unter "Emotionale/Kognitive Beeinflussung" oder die vordefinierten Strategien unter "Lernfokus & Strategie", um Myras Verhalten zu lenken.

## Wichtige Hinweise
*   **Experimenteller Charakter:** Dies ist ein Forschungsprototyp. Das Verhalten des Systems ist komplex und nicht immer vollständig vorhersagbar.
*   **API-Nutzung:** Die Verwendung der LLM-APIs kann Kosten verursachen.
*   **Lokale Speicherung:** Der Netzwerkzustand wird in heruntergeladenen Dateien gespeichert. Gelernte Inhalte werden in der IndexedDB Ihres Browsers gespeichert.
