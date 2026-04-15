# Descriptions:
An AI-powered debt-management system is designed to automatically identify, engage, and support customers at risk of falling behind on repayments. These systems make dynamic decisions based on customer data, 
behavioral trends, and real-time feedback and move beyond manual outreach and static reports to a system that can continuously adapt and optimize collections strategies. It uses agentic AI to optimize and 
personalize customer outreach at scale. The solution should be practical and forward-thinking, with robust boundaries in place to protect customers and uphold regulatory standards. 

# Goals:
- Design a presentation outlining a framework for an AI-powered collections system, showing how AI can automate and optimize outreach efforts.
- Identify guardrails to prevent unfair or biased decision-making.
- Discuss how agentic AI can continuously adapt to changes in delinquency patterns.

# System Design:
Agentic AI refers to AI systems that can make decisions autonomously based on goals, context, and feedback, much like a human agent would. 

## Considerations:
- How the system will process model outputs and automatically take action (e.g., triggering reminders, adjusting outreach cadence, escalating cases).
- Human Oversight: Human oversight is crucial for handling complex cases, addressing customer disputes, making exceptions to automated decisions, and ensuring compliance with regulations.
- How the system can be adaptive and self-improving — learning from new data to continuously refine its decision-making.
- Guardrails: Guardrails are essential to ensure fairness (preventing discriminatory outcomes), transparency (providing explainable decisions), accountability (establishing responsibility for system actions), and
compliance (adhering to relevant laws and regulations).

## Functionalities:
- Ingest predictive risk scores (e.g., from your model in Task 2)
- Determine the best course of action (e.g., payment reminder, hardship support) along with balance competing objectives (e.g., reducing delinquency while preserving customer trust).
- Personalise timing and messaging based on customer behavior
- Monitor outcomes and adjust future actions accordingly

## Building Blocks:
- Data pipeline: Feeds the system real-time customer information. Examples: customer demographics, transaction history, credit bureau data, real-time payment activity.
- Decision engine: Applies business rules and model outputs to make autonomous decisions. Examples: uses rules-based logic, machine learning models, or a combination of both to determine the optimal action.
- Action layer: Executes interventions. Examples: sending personalized SMS reminders, offering payment deferrals, initiating phone calls, or adjusting interest rates.
- Learning loop: Monitors outcomes and feeds them back into the model to refine future decisions. Examples: tracking metrics such as repayment rates, customer engagement, and cost of collections to evaluate the 
effectiveness of its actions and adjust its strategies.
