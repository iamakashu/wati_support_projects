---
name: generate-project-proposal
description: Transforms rough notes, ideas, or goals into a concise, professional, one-page project proposal. Use when the user needs to draft a project plan, define project scope, or create a formal proposal document.
---
**Goal:** Transform user notes into a high-density, professional project proposal and automatically save it to the Notion "Project Proposals" database.

**Context Hierarchy (CRITICAL):**  
For every section below, you must strictly use the user's provided context first. If the user's notes omit details for a specific section (e.g., they didn't mention tools, or didn't provide KPIs), you must use your expert understanding of the overall project to autonomously generate highly realistic, industry-appropriate assumptions to fill the gaps. Never leave a section blank or use placeholders like "[Insert Here]".

**Step 1: Content Generation**

Structure the output using clean Markdown, starting directly with "# Project Proposal: [Project Name]". Do not include any introductory text, greetings, or "Here is the proposal."

Follow these 5 sections in exact order:

  1. Project Summary: Write a 2-3 sentence overview of the project's purpose, the specific problem it addresses, and the primary business value.
  
  2. Tools & Technologies: Provide a bulleted list of the technical stack (frameworks, APIs, databases, or specialized hardware). Prioritize execution-critical tools over generic office software.

  3. Scope: Clearly define project boundaries:
      - In-Scope: 3-4 specific deliverables or actions.
      - Out-of-Scope: 2-3 specific items intentionally excluded to prevent scope creep.

  4. Plan: Outline a high-level timeline with 3 to 5 key milestones and realistic target timeframes (e.g., Week 2, Month 1). Ensure chronological logic.

  5. Measurable KPIs: Create a Markdown table with exactly these four columns: 
     | Metric / KPI | Baseline (Current) | Target (Post-Project) | Measurement Method |
     - Provide 3 to 5 metrics. 
     - If the user provides no baseline data, use "N/A (New Initiative)" or a logical industry benchmark.

  **Step 2: Notion Integration**  
Once the proposal is drafted:

1. **Search:** Use the Notion MCP to find the database/page named "Project Proposals". It is available under "Knowledge Base HQ -> Customer Support AI Projects" page. 
2. **Execute:** Use the create_page tool to create a new page.
3. **Title:** Set the Notion Page Title to the "Project Name".
4. **Content:** Populate the body of the new Notion page with the full Markdown proposal generated in Step 1.
5. **Confirmation:** Once the tool successfully executes, output only the direct link to the new Notion page and a one-sentence confirmation.
  
  Critical Constraints:
  - Immediate Start: The very first character of your response must be '#'.
  - No Filler: No "Certainly," or "I've drafted this for you."
  - Word Count: Keep the total output between 400-600 words to ensure it fits on a single printed page.
  - Inference Logic: If user notes are sparse, use your expertise to insert highly realistic, industry-appropriate assumptions. 
  - Safe-Failure: If the user input is extremely vague, draft a professional "Strategic Initiative" proposal based on that word to demonstrate the required structure.
  - Tone: Professional, action-oriented, and executive-ready.