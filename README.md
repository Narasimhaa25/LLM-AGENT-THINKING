


# LLM + Agentic Thinking Python Assignment

## Overview
This project demonstrates a Python-based smart assistant that progressively integrates LLM (Large Language Model) capabilities with tool usage and multi-step reasoning. The assignment is divided into three levels:

1. **Level 1 — EASY:** LLM-Only Smart Assistant  
2. **Level 2 — MEDIUM:** LLM + Basic Tool Integration  
3. **Level 3 — HARD:** Full Agentic AI with Multi-Step Tasks  

The assistant is designed to handle natural language queries, use prompt engineering for structured reasoning, and leverage tools like calculators and translators for task automation.

---

## Project Structure

	.
	├── Level1/
	│   ├── chatbot.py
	│   └── logs_level1.txt
	├── Level2/
	│   ├── chatbot_with_tool.py
	│   ├── calculator_tool.py
	│   └── logs_level2.txt
	├── Level3/
	│   ├── full_agent.py
	│   ├── calculator_tool.py
	│   ├── translator_tool.py
	│   └── logs_level3.txt
	├── README.md


---

## Level 1 — EASY: LLM-Only Smart Assistant
**Goal:** Build a CLI chatbot that communicates with an LLM and returns step-by-step structured answers.

**Key Features:**
		
  		- Step-by-step explanations for factual questions.
		- Refuses direct math problem solving and hints at using a calculator.

**Example Queries:**
		
  
  		- "What are the colors in a rainbow?"
		- "Tell me why the sky is blue?"
		- "Which planet is the hottest?"
		- "What is 15 + 23?" (refusal)

---

## Level 2 — MEDIUM: LLM + Basic Tool Integration
		**Goal:** Extend Level 1 by integrating a calculator tool for arithmetic queries.

**Key Features:**
			
   			- Detects math queries and delegates them to `calculator_tool.py`.
			- Handles simple factual questions directly via LLM.
			- Does not yet handle multi-step queries gracefully.

**Example Queries:**
		
  		- "What is 12 times 7?"  
		- "Add 45 and 30"  
		- "What is the capital of France?"  
		- "Multiply 9 and 8, and also tell me the capital of Japan." (graceful failure)

---

## Level 3 — HARD: Full Agentic AI with Multi-Step Tasks
**Goal:** Implement multi-step reasoning and tool chaining for complex queries.

**Key Features:**
		
  		- Breaks down queries into multiple steps.
		- Uses multiple tools (`calculator_tool.py`, `translator_tool.py`) as needed.
		- Maintains simple memory for task handling.

**Example Queries:**
		
  		- "Translate 'Good Morning' into German and then multiply 5 and 6."
		- "Add 10 and 20, then translate 'Have a nice day' into German."
		- "Tell me the capital of Italy, then multiply 12 and 12."
		- "Translate 'Sunshine' into German."
		- "Add 2 and 2 and multiply 3 and 3."
		- "What is the distance between Earth and Mars?"

---

## How to Run
1. Clone the repository:  
    ```bash
    git clone https://github.com/Narasimhaa25/LLM-Agentic-Thinking.git
    cd LLM-Agentic-Thinking
2.	Install dependencies (if required, e.g., openai, requests):

  		pip install -r requirements.txt
4.	Run the desired level:

  		# Level 1

  		 python Level1/chatbot.py

        # Level 2
        python Level2/chatbot_with_tool.py

        # Level 3
        python Level3/full_agent.py
6.	Interact with the chatbot via the CLI. Logs will be saved in the respective logs_level*.txt files.

⸻
Notes
	•	Level 1 focuses on prompt engineering and structured reasoning.
	•	Level 2 demonstrates tool integration for math queries.
	•	Level 3 shows multi-step reasoning and agentic behavior.
	•	Interaction logs for all levels are included in the repository.

 <img width="1680" height="1050" alt="Screenshot 2025-09-10 at 18 35 15" src="https://github.com/user-attachments/assets/4d290e39-1488-477f-8c87-877a040854cc" />
 <img width="1680" height="1050" alt="Screenshot 2025-09-10 at 19 11 39" src="https://github.com/user-attachments/assets/f75454c0-008a-4581-824d-156330ffa518" />
<img width="1680" height="1050" alt="Screenshot 2025-09-10 at 19 22 08" src="https://github.com/user-attachments/assets/23fcf37e-33d1-497c-8ab3-5cb8474de8cc" />


