This **README** is designed for users or teams who will be using the `generate-project-proposal` skill. It explains how to interact with the AI to get the best results.

## 📌 Overview
The **Project Proposal Generator** is an AI-powered assistant that acts as a Senior Project Manager. It is designed to take unstructured thoughts, "back-of-the-napkin" ideas, or messy meeting notes and transform them into a formal, executive-ready, one-page project proposal.

## 🚀 How to Use
To trigger this skill, simply provide your notes or a project title and ask for a proposal.

**Example Triggers:**
* *"I have an idea for a mobile app that tracks carbon footprints. Generate a proposal."*
* *"Here are my notes from the brainstorming session: [Paste Notes]. Create a project plan from this."*
* *"Draft a formal proposal for a warehouse migration to a new ERP system."*

## 🛠 What the AI Does
When this skill is activated, the AI follows a strict professional protocol:
1.  **Expert Persona:** It writes from the perspective of a PMP-certified Project Manager.
2.  **No "Chatter":** It bypasses greetings (like "Sure, I can help with that") and gives you the document immediately.
3.  **Intelligent Inference:** If your notes are missing details (like a timeline or specific tools), the AI uses industry standards to "fill in the blanks" with realistic assumptions.
4.  **One-Page Format:** The output is mathematically constrained to fit on a single printed page (approx. 400-600 words).

## 📋 The Proposal Structure
Every output will contain these six sections in order:
1.  **Project Summary:** High-level business value and problem statement.
2.  **Tools & Technologies:** The specific technical stack required.
3.  **Scope:** Clear "In-Scope" and "Out-of-Scope" lists to prevent scope creep.
4.  **Plan:** 3–5 chronological milestones with target dates.
5.  **Measurable KPIs:** A data table containing Metrics, Baselines, Targets, and Measurement Methods.
6.  **First Action to Kickstart:** A single, highly specific immediate next step required to officially launch the project.

## 💡 Tips for Best Results
*   **Mention Constraints:** If you have a specific deadline (e.g., "Must be done by Q4") or a specific tool you must use (e.g., "Must use AWS"), include that in your prompt.
*   **The "Gap-Fill" Feature:** If you don't know the KPIs or the tech stack, don't worry. The AI is instructed to suggest the most logical industry-standard options for you.
*   **Copy-Paste Ready:** The output uses Markdown. You can paste it directly into Notion, Obsidian, GitHub, or export it to a PDF for a professional look.

## ⚠️ Limitations
*   **Financial Precision:** While the AI can suggest KPIs, it does not have access to your company’s real-time financial data. Always verify "Baseline" numbers in the KPI table before presenting to stakeholders.
*   **Refinement:** If the AI's "inferred" assumptions don't match your vision, simply reply: *"Update the Tools section to use Google Cloud instead of AWS,"* and it will rewrite the document.

***

### Technical Metadata (For System Admins)
| Field | Value |
| :--- | :--- |
| **Skill Name** | generate-project-proposal |
| **Persona** | Expert Project Manager |
| **Output Format** | Markdown (Strict) |
| **Constraint** | No conversational filler; 400-600 words |
| **Logic Mode** | Synthetic Inference (Fills missing data) |