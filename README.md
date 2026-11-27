# Pramaan: AI Chatbot Truth Tester
*Pramaan* means "proof" in Hindi. Pramaan proves whether an AI chatbot tells customers the truth.


## The Problem   
Many companies now use AI chatbots to answer customer questions. The chatbot works on behalf of the company, and customers trust and act on its answers. But AI can give wrong information, and the company is responsible for every answer its chatbot gives.

In 2024, Air Canada's chatbot told a customer he could claim a discounted fare refund after booking. The airline's official policy said the opposite. A tribunal ruled that Air Canada was responsible for its chatbot's answer and ordered the airline to pay the customer.

A single wrong answer can lead to legal problems, financial loss, and loss of customer trust. That is why checking what the chatbot says is essential.

## Why It Is Hard to Test  
Normal test automation compares an actual result with a fixed expected result. This does not work for AI chatbots because:

- The chatbot gives differently worded answers to the same question, even when the meaning is correct.
- AI can "hallucinate", which means it confidently gives information that is made up.
- Company policies change on the website, but the chatbot may keep giving old answers.
- A chatbot may answer correctly in English but give wrong information in other languages.



## What Pramaan Does    

Pramaan checks whether a company's chatbot gives customers correct information, based on the company's official website, terms, and policies.

1. Reads the company's official FAQ and policy pages as the source of truth.
2. Creates realistic customer questions from those facts.
3. Asks the chatbot each question through the real website, just like a customer (using Playwright).
4. Uses AI to compare the chatbot's answer with the official information and marks it as correct, contradicting, or made up.
5. Repeats the questions in Indian languages such as Hindi and Kannada.
6. Generates a report highlighting risky answers.

*Example:** The website says returns are allowed within 7 days, but the chatbot tells a customer 30 days. Pramaan flags this as a high-risk contradiction.

## Who Will Use It  


- **QA and automation teams** testing chatbot releases
- **Developers** building chatbots, to catch problems before customers do
- **Product, compliance, and legal teams**, to make sure the chatbot follows company policy
- **Any company using a customer-facing AI chatbot**, such as banks, airlines, e-commerce, and telecom companies

## Project Status

🚧 In progress: currently in the planning and learning phase.

