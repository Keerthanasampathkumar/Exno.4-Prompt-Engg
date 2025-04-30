# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:                                                                            
### REGISTER NUMBER : 212222230066
### Aim: 
To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

### Algorithm:  1. Direct Instruction Prompts
The system first identifies the scenario type (e.g., weekly sales, customer complaints, incident report) via intent detection. Based on prompt style, it formats the output using one of the following techniques:

    Straightforward Prompting: Uses direct input and outputs a plain-text summary.

    Tabular Prompting: Organizes key aspects (dates, actions, outcomes, metrics) in a structured table.

    Preceding Question Prompting: Begins by collecting missing parameters (e.g., time period, team name, metric scope), then generates a detailed report.

Behind the scenes, AI applies summarization techniques and pattern recognition to distill key details into an executive-level narrative. Techniques like entity extraction, date/time mapping, and causal linkage (e.g., what led to the incident) improve output accuracy. Tools such as GPT-based models can be instructed with explicit formatting constraints or few-shot examples.

# PROMPT:
### Straightforward Prompt:
```
“Generate a weekly report for Team A’s customer support activity from April 20 to April 27.”
```

### Tabular Format Prompting:
```
“Create a detailed report for a technical incident on April 25, showing categories like Timestamp, Event, Action Taken, and Resolution in table format.”
```

### Preceding Question Prompting:
```
“Before writing the summary, ask for any missing data: team name, scenario type, time range, and outcome. Then generate a narrative report.”
```

# OUTPUT
### Straightforward:
AI: “Between April 20 and 27, Team A resolved 152 customer queries, with an average response time of 3.4 hours. The satisfaction rating increased by 6%, and two minor escalations were addressed. No SLA violations occurred during this period.”

Tabular:
AI:
![image](https://github.com/user-attachments/assets/bce5d4a4-8255-4e16-a96b-9cf183a778b4)

### Preceding Questioning:
AI:
    “What is the name of the team or department?”

    “What timeframe should the report cover?”

    “What type of scenario (e.g., sales, incidents, feedback) is this about?”

    “Should the report include KPIs or just a summary?”

After input, AI:
“Here’s the scenario-based report for the DevOps Team covering April 20–27. During this week, two key incidents were managed. The first was a server load spike that was mitigated in under five minutes. The second involved login outages, resolved via authentication fixes. No repeat issues were observed. This proactive handling contributed to 99.98% uptime.”



# Result: 
Each technique serves a different reporting need. The straightforward prompt works well for generating a quick narrative summary and is suited for weekly digests or brief team updates. Tabular formatting is ideal for incident reports, as it clearly shows chronological steps and resolutions. Research notes that tabular reports are easier for managers to skim and compare event timelines . The preceding-question method improves personalization, especially when users omit context. It ensures the AI asks for relevant variables, resulting in higher accuracy and relevance . This method is best for complex or ad hoc reports where input data may be incomplete. In summary, choosing the right prompting technique allows AI to generate scenario reports that are fast, clear, or tailored—depending on the business need.
