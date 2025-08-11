# Deep Research Agent

## 📌 Short Description

Deep Research Agent is an AI-powered multi-agent system that conducts iterative, citation-backed research, consolidating findings into well-structured long-form reports.

---

## 📖 Detailed Explanation

Deep Research Agent is an advanced AI-driven research framework designed to mimic a skilled researcher’s approach to complex topics. Unlike single-pass tools, it divides research into specialized tasks, coordinated by multiple sub-agents.

**Key Features:**
- **Planner Agent:** Orchestrates the process by analyzing queries, creating a list of focused research tasks, and assigning each task to a sub-agent with specialized tools (ArXiv for academic papers, Tavly API for web searches, and a Web Scraper for targeted extraction).
- **Iterative Cycles:** The system reviews initial findings to determine if further research is needed. It can refine the plan and run additional sub-agents (up to 5 loops) for deeper insights.
- **Final Report:** Delivers a citation-rich markdown report featuring a compelling title, 200–300 word abstract, structured sections and tables, and verified references.

This design minimizes hallucination risks, ensures depth, and produces professional-grade research outputs.

![NotebookLM Mind Map](NotebookLM%20Mind%20Map.png)

---

## ⚙️ How It Works

1. **Form Input:** User submits a query.
2. **Planner Agent:** Designs a research strategy and creates sub-agents.
3. **Iteration Node:** Executes each sub-agent’s task.
4. **Sub-Agents:** Use specialized tools to gather detailed, cited information.
5. **Writer Agent:** Consolidates findings into a long-form markdown report.
6. **Condition Node:** Checks if further research is needed.
7. **Loop Node:** Refines and repeats research (up to 5 iterations).
8. **Direct Reply:** Sends the final report to the user.

---

![NotebookLM Mind Map (1)](NotebookLM%20Mind%20Map%20(1).png)

## 🧪 Example Run

**Query:**  
"The differences between OpenAI, Meta, and Anthropic in how they approach training models and their target markets."

**Process:**
- Generated sub-agents for each company.
- Researched using Tavly API, Web Scraper, and ArXiv.
- Compiled into a structured, cited report with a comparison table.

**Final Report Highlights:**
- Abstract & Introduction.
- Sections on training methodologies & target markets.
- Detailed comparison table.
- Citations from trusted sources.

---

## 📚 References

- ArXiv.org
- Tavly API
- Web Scraper
