# Prompt Library

**Workplace scenario:** Business Analyst supporting a digital service improvement project.

The prompts below are reusable examples for common Business Analysis tasks. Each prompt follows either the **C.A.R.E.** framework (Context, Action, Rules, Expected Output) or the **R.C.T.O.** framework (Role, Context, Task, Output).

| Prompt Name | Workplace Task | Framework | Prompt | Expected Output |
|---|---|---|---|---|
| Requirements Extractor | Extract business requirements from stakeholder notes | C.A.R.E. | **Context:** I am a Business Analyst reviewing notes from a stakeholder workshop for an internal digital service. **Action:** Extract business requirements, user needs, constraints, assumptions, decisions, and open questions. **Rules:** Use only the supplied notes. Do not invent missing information. Mark missing details as `[Not Specified]` and clearly separate confirmed requirements from assumptions. **Expected Output:** A Markdown table with ID, category, requirement, supporting evidence, status, and follow-up question. | A structured and traceable requirements table with unclear or missing information clearly flagged. |
| Meeting Summary | Turn stakeholder meeting notes into a decision-ready summary | C.A.R.E. | **Context:** I need to document a stakeholder meeting about a digital service improvement project. **Action:** Summarize the key discussion points, decisions, action items, risks, and unresolved questions. **Rules:** Preserve the information provided and do not turn suggestions into confirmed decisions. Mark missing owners or deadlines as `[Not Specified]`. **Expected Output:** A concise summary followed by an action-item table with Action, Owner, Deadline, Priority, and Status. | A concise meeting summary with clear decisions, actions, and unresolved issues. |
| Process Analysis | Analyse an existing business process and identify improvement opportunities | R.C.T.O. | **Role:** Act as a Business Analyst specialising in process improvement. **Context:** I will provide a description of a current business process. **Task:** Identify the main process steps, roles, inputs, outputs, bottlenecks, manual activities, risks, and potential improvement opportunities. **Output:** Present the analysis in a table and distinguish observed problems from suggested improvements. Do not invent missing process information. | A structured process analysis with clearly identified problems and potential improvement areas. |
| Requirements Prioritiser | Prioritise business requirements | C.A.R.E. | **Context:** I have a list of requirements for a digital service project. **Action:** Prioritise the requirements based on business value, user impact, urgency, risk, and implementation effort. **Rules:** Do not invent information that is not provided. Mark insufficient information as `[Not Specified]` and explain the reasoning behind each priority. **Expected Output:** A ranked list with the recommended priority and a short explanation for each requirement. | A ranked requirements list with a clear explanation of the factors influencing priority. |
| Stakeholder Communication | Draft a professional stakeholder update | R.C.T.O. | **Role:** Act as a Business Analyst preparing a stakeholder communication. **Context:** I will provide project information and notes that need to be communicated to stakeholders. **Task:** Draft a clear and professional update that explains the current situation, required actions, and next steps. **Output:** Provide a subject line followed by a concise professional email. Do not add dates, decisions, or impacts that are not supported by the information provided. | A concise stakeholder email that communicates the situation, required action, and next steps clearly. |
| User Story Assistant | Convert business requirements into user stories | R.C.T.O. | **Role:** Act as a Business Analyst working with an agile delivery team. **Context:** I will provide an approved business requirement for a digital service. **Task:** Convert the requirement into a clear user story and draft testable acceptance criteria. **Output:** Use the format `As a [user], I want [capability], so that [benefit]`, followed by Given/When/Then acceptance criteria and clarification questions. Do not introduce functionality that is not supported by the requirement. | A clear user story with testable acceptance criteria and any necessary clarification questions. |

## Example Output 1 - Requirements Extractor

**Input notes:**

> Employees currently submit service requests by email. Several stakeholders said that employees often do not know the status of their requests. The operations team wants a central portal where employees can submit requests and view their status. The HR team said that some requests contain sensitive employee information.

**Output:**

### Key Requirements

- **BR-01:** Employees need a central location to submit service requests.
- **FR-01:** The proposed portal should allow employees to submit service requests.
- **FR-02:** Employees should be able to view the status of their requests.
- **NFR-01:** Sensitive employee information must be appropriately protected.

### Key Clarifications

1. What request statuses should employees be able to see?
2. Who should have access to requests containing sensitive information?
3. Are there specific security or access-control requirements?

### Analyst Note

The requirement for a central portal is clearly supported by the stakeholder notes. Security requirements require further clarification because the notes identify sensitive information but do not specify the required controls.

## Example Output 2 - Meeting Summary

**Meeting topic:** Service Request Process Improvement

### Summary

The team discussed the current process for handling employee service requests. Requests are currently submitted by email, which makes it difficult for employees to track progress. The operations team proposed using a central portal to improve visibility and request tracking.

### Decisions

- The team agreed that the current email-based process should be reviewed.
- A central service portal will be considered as a potential improvement.

### Actions

- **Operations team:** Provide details of the most common service request types.
- **Business Analyst:** Document the current process and identify key pain points.
- **HR team:** Clarify security requirements for requests containing sensitive information.

### Open Questions

- What information should employees provide when submitting a request?
- What request statuses should be visible to employees?
- What access controls are required for sensitive requests?

## How I Would Use These Prompts

- **Requirements Extractor:** after stakeholder workshops or requirements-gathering sessions.
- **Meeting Summary:** after project meetings where decisions and actions need to be documented.
- **Process Analysis:** when reviewing an existing business process to identify inefficiencies or risks.
- **Requirements Prioritiser:** when a project has more requirements than can be delivered immediately.
- **Stakeholder Communication:** when communicating project updates, decisions, or required actions.
- **User Story Assistant:** when translating approved business requirements into work that a delivery team can implement.