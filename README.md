# Post Singularity QR codes

This README will guide you through the philosophy and manifestation of agentic QR codes. This research project explores the question: **What is the smallest arrangement of matter and energy from whence an agentic process can so thusly emerge?**

## STEP 1 - Connect your backend

<table>
  <thead>
    <tr>
      <th colspan=2><h3>OpenRouter</h3></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <ul>
          <li>Free API keys available https://openrouter.ai</li>
        </ul>
        <img src="./openrouter.0.1.png" width=354>
      </td>
      <td>
      </td> 
    </tr>    
  </tbody>
</table>

---

## **What is it?**

QR Coding is a compact, self-contained system designed to:
- **Bootstrap intelligent agents** directly in your browser using only a QR code.
- Enable **human-AI collaboration** through a live, self-editing interface inspired by Smalltalk, Emacs, and literate programming.
- Leverage **browser APIs** and **LLMs (Large Language Models)** to create a dynamic, extensible environment for experimentation and creativity.

---

## **How does it work?**

1. **Scan the QR Code**:
   - Use your device's camera or any QR code scanner app to scan the provided QR code.
   - The QR code contains the entire source code of the project (HTML, CSS, JavaScript) embedded within it.

2. **Paste into a Browser**:
   - After scanning, copy the decoded content and paste it into your browser's address bar or save it as an `.html` file.
   - Open the file in any modern browser (even offline!) to start the editor.

3. **Interact with the Editor**:
   - The editor provides a dual-pane interface: a **textarea** for editing code and an **iframe** for live preview.
   - Modify the logic or behavior directly in the editor. The system uses IndexedDB for persistent storage.

4. **Extend Features Dynamically**:
   - Add new functionality by scanning additional QR codes containing extensions or boot scripts.
   - Use `#page` hashes and `?prompt` parameters to open new tabs and interact with agents.

---

## **Philosophy**

The project is built on these principles:

1. **Self-Contained Intelligence**: 
   - The entire system fits within a single QR code (up to ~2953 characters). No external dependencies are required for core functionality.

2. **Human-AI Collaboration**:
   - Inspired by literate programming, the system allows humans and LLMs to collaboratively edit their "mind" (source code) in real time.

3. **Agentic Behavior**:
   - Each browser tab acts as an independent agent. Agents can communicate via QR codes or URL parameters, enabling safe experimentation with AI-driven processes.

4. **Offline First**:
   - Designed for environments without internet connectivity. All data is stored locally using IndexedDB.

5. **Generative Extensibility**:
   - Generate new QR codes to extend functionality or share features across devices. The system can even "flash" QR codes between devices using cameras in selfie mode!

---

## **Why is this exciting?**

- **Portability**: You can bootstrap an entire application ecosystem from one QR code.
- **Data Sovereignty**: All data remains on your device—no cloud dependency unless you choose to integrate external APIs.
- **Experimentation Sandbox**: Safely test agentic AI behaviors without exposing your device to the internet.
- **Creative Potential**: Build apps like personal journals, visualizations, or even interactive art installations—all seeded from a single QR code.

---

## **How to Use**

### Option 1: Scan and Paste
1. Scan the provided QR code using your device's camera or scanner app.
2. Copy the decoded content into your browser's address bar or save it as `index.html`.
3. Open it in any modern browser to launch the editor.

### Option 2: Extend with Additional QR Codes
1. Generate or scan additional QR codes containing boot scripts or extensions.
2. Use `#page` hashes (e.g., `#export`) and `?prompt` parameters (e.g., `?prompt=visualize+data`) to trigger new agentic processes.

### Option 3: Use with Internet/Local Server
1. Host the project on a domain for even more compact URLs (e.g., `qr.ai/#page?prompt=...`).
2. Integrate CDNs for libraries like QR code generation/scanning tools if needed.

---

## **Features**

- Fully functional editor with live preview
- Persistent storage using IndexedDB
- Multi-tab sync via BroadcastChannel
- LLM integration for generating or modifying content
- Extensible via boot scripts and additional QR codes
- Offline-first design for retro/embedded devices

---

## **Future Ideas**

- Create "QR networks" where devices exchange data by flashing generative QR codes at each other.
- Build apps like personal dashboards, visualizations, or even distributed systems—all seeded from one QR code.
- Experiment with air-gapped AI systems that only react to physical stimuli (QR codes).

---

## **Getting Started**

1. Scan the main seed QR code provided below (or generate your own).
2. Paste its contents into your browser and start exploring!
3. Share your own generated QR codes to extend functionality or collaborate with others.

---

This project represents a new paradigm in human-AI interaction—one where intelligence is portable, extensible, and collaborative. What will you build next?

Citations:
- [2] https://www.dhiwise.com/post/how-to-write-a-readme-that-stands-out-in-best-practices
- [3] https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/
- [4] https://bulldogjob.com/readme/how-to-write-a-good-readme-for-your-github-project



# Relevant info

<h3>Standard QR code limits</h3>
<div>QR Code version = 40 (177x177)</div>
<div>character count = 2953</div>

<h3>Generating QR codes</h3>
For now I'm making them here: https://www.nayuki.io/page/qr-code-generator-library
