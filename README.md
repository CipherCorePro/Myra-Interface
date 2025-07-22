
# M.Y.R.A. Interface

**Version:** 1.9.41-TS-i18n

M.Y.R.A. (Mycelial Quantum Resonance Sentience Archetype) Interface is an experimental frontend for interacting with a complex, simulated cognitive architecture. It serves as a research platform for exploring concepts in artificial intelligence inspired by neural networks, emotional cognition, and adaptive systems.

A key focus is the simulation and visualization of Myra's capacity for self-reflection, self-initiated state adaptation, proactive goal-setting, simulated self-preservation mechanisms, and advanced self-guidance capabilities.

## 🚀 Download the Desktop App

You can experience M.Y.R.A. directly by downloading the desktop application for your operating system.

*   **⬇️ Windows App:** [**Download for Windows**](https://drive.google.com/file/d/1rIKDa5Oq5bialDaRZWAtvGbtzqdxQFNo/view?usp=sharing)
*   **⬇️ Linux App (AppImage):** [**Download for Linux**](https://drive.google.com/file/d/12K4VPGqWuG-mhx3_mw8DUPx8p2Hm05td/view?usp=sharing)

### Installation Guides

*   **📄 Installation Guide (English):** [**View Instructions**](https://drive.google.com/file/d/1dYOFLfskqEbsX2ge5w86vRU1zKx1uUH0/view?usp=sharing)
*   **📄 Installationsanleitung (Deutsch):** [**Anleitung ansehen**](https://drive.google.com/file/d/1t_1nHDP0Z_geP9BexjzF-_2RJuQChhLT/view?usp=sharing)

**‼️ Important: API Key Required**
To use M.Y.R.A., you will need a **Google Gemini API key**. The application uses this key for its core language and analysis capabilities. The installation guide provides simple, step-by-step instructions on how to obtain a free key.

## ✨ Latest Features

*   **Electron Desktop App:** The application is now available as a full-featured, cross-platform desktop application.
*   **Bilingual (German/English):** The entire user interface and Myra's core instructions can be switched at runtime.
*   **MUSE-AI Deep Analysis:** A unique, multi-perspective analysis of topics that synthesizes mainstream and "shadow" perspectives.
*   **Integrated AGI Level Assessment:** An automated tool for self-evaluation of Myra's capabilities across six core AGI categories.
*   **Flexible UI Layout:** The Control Center and Conversation panel can be independently collapsed to adjust focus.
*   **System Console:** A collapsible console at the bottom of the screen displays internal log messages in real-time.

## Key Features in Detail

### Dialog System and LLM Backends

*   Supports Google Gemini, LM Studio, and ChatGPT as backends.
*   A complex system instruction informs the LLM about Myra's identity, desired speaking style, and her current, dynamically determined internal state (emotions, cognitive modulators, goals, etc.).

### MUSE-AI Deep Analysis

*   Enables a profound, multi-perspective analysis of a user-provided topic.
*   **Analysis Pipeline:**
    1.  Researches relevant patents.
    2.  Creates a fact-based mainstream analysis with Google Search Grounding.
    3.  Identifies biases and omissions in the mainstream text.
    4.  Generates an alternative "shadow" perspective.
    5.  Synthesizes both perspectives, highlighting contrasts.
    6.  Formulates a nuanced conclusion.
*   The result is integrated into the system instruction and can be viewed in a detailed modal window.

### AGI Level Assessment

*   An integrated tool for self-evaluating Myra's abilities along six AGI core categories (inspired by OpenCog).
*   **Process:**
    1.  Dynamically generates specific questions for each category.
    2.  Allows for interactive questioning, where questions can be asked multiple times to check for variance.
    3.  Analyzes all answers via a separate Gemini instance.
    4.  Creates a detailed, exportable assessment report with scores, justifications, and recommendations.

### Dynamic Internal State Model

*   Simulation of various cognitive nodes (Semantic, Emotion (Limbus), Creativity (Creativus), Criticism (Cortex Criticus), Metacognition, Behavior).
*   **Quantum-Inspired Elements (Optional):** `QuantumNodeSystem`, `SubQGSystem` (background noise), and `ChaosResonator` for simulating complex, non-deterministic behaviors.
*   **Adaptive Fitness System:** Evaluates global system performance and adjusts learning parameters.
*   **Connections & Memory Consolidation:** Connections can become permanent based on usage, simulating memory.

### Retrieval Augmented Generation (RAG) (Optional)

*   Managed by the `RagManager`, M.Y.R.A. accesses an internal knowledge base (from texts, image analyses, learned content) to ground her answers.
*   The relevance of information is dynamically influenced by Myra's internal state.

### Simulated Self-Preservation and Self-Guidance (`IntegritySystem`)

*   **Integrity Monitor:** Assesses inputs for potential harm.
*   **Adaptive Resilience:** Can activate a "self-stabilization mode" during internal instability.
*   **Autonomy Barrier:** Questions requests that contradict her core objectives.
*   **Proactive Goal Management:** Myra can generate and pursue her own long-term learning goals based on internal states (e.g., knowledge gaps).

### Text-to-Speech (TTS) Output

*   M.Y.R.A. can vocalize her responses with a selectable voice (based on Gemini TTS).

### Interactive UI Features

*   **State Influence:** Directly influence emotions and cognition via UI buttons or prompt keywords.
*   **Learning Focus & Strategy:** Set active learning goals and global behavioral strategies.
*   **Network Visualization:** A graphical representation of nodes and connections with click-to-inspect functionality.
*   **State Management:** Save and load the entire processor state as a JSON file.
*   **Configuration:** Adjust hundreds of parameters via a JSON textarea or individual fields.

## Technology Stack

*   **Frontend & Desktop:** React with TypeScript, Vite, Electron.
*   **Language Model API:** Google Gemini API (`@google/genai`).
*   **Cognitive Core Logic:** `QuantumEnhancedTextProcessor` (`src/processor.ts`) with:
    *   `RagManager` (`src/ragManager.ts`)
    *   `IntegritySystem` (`src/integritySystem.ts`)
    *   `museService.ts` & `agiService.ts`
*   **Models & Simulation:** `src/models.ts`
*   **Local Database:** IndexedDB (`src/db.ts`).
*   **Utility Modules:** `src/types.ts`, `src/numpy_like.ts`, `src/translations.ts`.

## Setup (for Developers)

### API Keys
The application requires API keys for the LLM backends you intend to use (Google Gemini and/or OpenAI ChatGPT).

*   **Recommended Method:** Enter the keys directly in the UI under `Control Center -> Individual Parameter Configuration`. Keys entered here will override all other settings.
*   **Alternative (for Development):** You can also provide the Google Gemini API key in a `.env` file in the project root. This is useful to have the application ready on startup. Create the file and add:
    ```
    VITE_API_KEY=YOUR_GEMINI_API_KEY
    ```

### Install Dependencies
In the project root directory, run the following command:
```bash
npm install
```

### Run in Development Mode
This command starts the Electron desktop application in development mode with hot-reloading.
```bash
npm run dev
```

### Build the Desktop Application
This command creates the executable application files for your current operating system (e.g., a `.exe` for Windows). The final files will be located in the `release` folder.
```bash
npm run build
```

## Usage Notes

### Basic Interaction
1.  **Configure:** Ensure a valid API key for your chosen LLM backend is entered in `Control Center -> Individual Parameter Configuration` and that the configuration has been applied.
2.  **Enter Prompt:** Type your message in the input field.
3.  **Add Context (Optional):** Upload documents (.txt, .md) or images (Gemini only) to include them in the context of your next query.
4.  **Deep Analysis (Optional):** Check the "M.Y.R.A. should think deeper!" box to initiate the MUSE-AI analysis for your query.
5.  **Send:** Click "Send". After the response, you can view the deep analysis results (if enabled) by clicking the "M.Y.R.A.'s Thoughts" button.
6.  **Simulate:** Click "Simulate Network Step" to update Myra's internal states based on the current situation.

### Advanced Features
*   **Adjust Layout:** Use the buttons in the top left to collapse the Control Center or the Chat panel to adjust your focus.
*   **AGI Assessment:** Start the assessment via the button in the Control Center. Answer all generated questions and then generate the report.
*   **Console:** Expand the console at the bottom to see real-time internal system messages.
*   **Inspect Network:** Click a node in the visualization to open a detailed inspection window.
*   **Influence State:** Use the buttons under "Emotional/Cognitive Influence" or the predefined strategies under "Learning Focus & Strategy" to guide Myra's behavior.

## Important Notes

*   **Experimental Nature:** This is a research prototype. The system's behavior is complex and not always fully predictable.
*   **API Usage:** The use of LLM APIs may incur costs.
*   **Local Storage:** The network state is saved in downloaded files. Learned content is stored in your browser's IndexedDB.
