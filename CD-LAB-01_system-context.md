My exact KC7 username: **PIEDELEEUW**

Date I finished How to Play KC7: **10 November 2026**

Investigation: A Rap Beef: An Intro to Security Investigations

Date I finished the investigation: **10 November 2026**

<img width="656" height="748" alt="image" src="https://github.com/user-attachments/assets/61dab9bb-73c2-4ed7-bedc-a793c2b5e126" />
<img width="660" height="851" alt="image" src="https://github.com/user-attachments/assets/3f51f299-44ec-4714-a312-d62e087c00a1" />

My first prediction and how sure I was (0–100%): **100%**

People who use this service: **Learners and Staff**.

**Data and systems we need to protect:** 

| Data Source | Potential data |
| --- | --- |
| Learner’s web request | Question, selected program, and any identifiers or contact details the form requests |
| Free-text question | Personal or sensitive information the learner includes, even if the form does not request it |
| Browser and network | IP address, request time, browser details, and authentication information, depending on implementation |
| Approved information sources / Repositories | Program descriptions, dates, fees, policies, document references and versions |
| Staff | Corrections, review decisions, notes and task updates |
| AI provider | Generated reply and response metadata |

**Parts I included in my design:**

1. Learner

2. Web client

3. API

4. AI provider

5. Approved knowledge source

6. Logging service

7. Staff console

**Parts I left out of my design:**

1. Physical and/or Virtual hosting infrastructure and/or Cloud Service(s) (IaaS, SaaS, Paas)

2. DNS Service Provider(s) + Defence service(s)

3. Security Controls (Administrative, Technical, Physical) related to the omitted design components 


What this service should help people do:

The service should help learners get accurate answers about BBR Academy’s programs and reach staff when they need personal assistance or help.

It should help:
- Learners: Submit questions and receive clear answers based on approved program information.

- Staff: Review questions, check AI-drafted replies and handle cases requiring human judgment.

- Staff: Track follow-up tasks so learner questions are resolved.

- Service administrators: Identify mistakes or misuse through minimal, privacy-conscious logs.

- The AI’s role is to assist with drafting. Authorised staff remain responsible for decisions requiring approval.

What could go wrong for learners or staff:

The main risks are incorrect advice, exposed personal information and missed support.

| What could go wrong? | How learners or staff could be harmed |
| --- | --- |
| **Incorrect or outdated answers** | Learners misunderstand requirements or miss deadlines. Staff spend time correcting mistakes. |
| **Personal information is exposed** | Questions or staff notes reach another learner, unauthorised staff or the AI provider unnecessarily. |
| **A document manipulates the AI** | Hidden instructions cause misleading replies, unsafe links or inappropriate task suggestions. |
| **Unauthorised access or changes** | Someone reads private cases, changes approved information or alters staff tasks. |
| **Questions or follow-ups are lost** | Learners receive no help, while staff believe another person is handling the case. |
| **Staff rely too heavily on AI drafts** | An inaccurate answer is approved without checking its sources or understanding the learner’s situation. |
| **Offensive or biased replies** | Learners feel dismissed, receive unequal support or lose trust in the academy. |
| **Outages, spam or excessive requests** | Learners cannot access help, and staff face growing queues and additional manual work. |

Data I would keep out of AI tools and public files:

These categories align well with OWASP’s guidance on preventing sensitive information disclosure in AI applications.

| Data to keep private | Examples |
| --- | --- |
| **Learner identifiers** | Names, email addresses, phone numbers, home addresses and learner numbers |
| **Sensitive personal information** | Health conditions, disability details, government ID numbers, financial difficulties and payment details |
| **Private learner records** | Grades, complaints, support histories and identifiable questions or conversations |
| **Staff-only information** | Internal case notes, private contact details and confidential review discussions |
| **Passwords and security secrets** | Passwords, API keys, access tokens, session cookies, encryption keys and database credentials |
| **Confidential academy documents** | Unpublished policies, internal investigations, contracts and restricted program material |

We would also need to keep raw logs, database exports and unredacted screenshots out of public files and AI uploads. They can contain personal information or credentials. Logs themselves should exclude secrets and unnecessary sensitive data.
