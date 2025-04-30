# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:                                                                            
### REGISTER NUMBER : 212222230066
### Aim: 
To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

### Algorithm:  1. Direct Instruction Prompts
Objective: Guide the chatbot to respond concisely to customer inquiries.
Prompt Pattern:
Prompt: "When a customer asks for the status of their order, reply with: 'Your order is currently being processed and will be delivered by [date].'"
2. Contextual Prompting
Objective: Incorporate specific context to provide detailed answers based on the user’s previous interaction.
Prompt Pattern:
Prompt: "If the customer previously mentioned that they haven’t received their order, say, 'I see that you mentioned your order hasn't arrived yet. Let me check the details for you and get back shortly.'"
3. Persona-Based Prompting
Objective: Design the chatbot to adopt a specific persona, making the interaction more engaging.
Prompt Pattern:
Prompt: "Pretend you are a friendly, helpful customer service representative. Use a conversational tone, such as 'Hey there! I’m here to help with any questions you might have. Let’s get your issue sorted!'"
4. Few-Shot Prompting
Objective: Teach the AI how to respond using a few examples, enabling it to generalize for similar situations.
Prompt Pattern:
Prompt: "Here are some examples of how to handle technical questions:
'My phone isn't charging.' → 'Have you tried using a different cable? If that doesn’t work, it may be an issue with the port.'
'The screen is flickering.' → 'It sounds like a display issue. Have you tried restarting the device?'
Now, respond to: 'My app keeps crashing.'"
5. Chain of Thought Prompting
Objective: Use a step-by-step reasoning approach for resolving more complex or technical issues.
Prompt Pattern:
Prompt: "When a customer reports their laptop overheating, guide them through the following steps:
Ask if they are using the laptop on a soft surface.
Suggest moving the laptop to a flat, hard surface for better airflow.
Ask if they’ve cleaned the vents recently.
Recommend restarting the device to see if the issue persists.
Now, solve: 'My laptop fan is making a loud noise.'"
6. Instruction with Constraints
Objective: Instruct the chatbot to provide assistance while adhering to specific constraints (e.g., response length or tone).
Prompt Pattern:
Prompt: "Respond to order inquiries in no more than 50 words and avoid using technical jargon. For example, 'Your order is on the way and should arrive by [date]. Feel free to reach out if you need anything else.'"
7. Reflective Prompting
Objective: Ensure that the chatbot reflects the user’s query back to them before providing a response, reducing misunderstandings.
Prompt Pattern:
Prompt: "When a customer asks for help, first reflect their question back to them. For example, if they ask 'How can I reset my password?' respond with 'You're asking how to reset your password, correct? Here’s how you can do it.'"
Result: The various types of Prompts are executed successfully.

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
