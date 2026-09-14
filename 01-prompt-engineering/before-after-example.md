# Before and After Prompt Example

## Before - Weak Prompt

> Analyse these stakeholder notes and identify the requirements.

## Initial Result

The initial result would probably be incomplete or inconsistent because the prompt does not explain what type of requirements to identify, how to handle assumptions, what information should be included, or how the results should be presented. The AI may also interpret unclear statements as confirmed requirements.

## After - Structured Prompt

### C.A.R.E. Prompt

**Context:** I am a Business Analyst reviewing notes from a stakeholder discussion about improving an internal employee service request process. Employees currently submit requests by email, and the operations team is considering a central digital portal.

**Action:** Analyse the stakeholder notes and identify business requirements, user needs, constraints, assumptions, decisions, and open questions.

**Rules:** Use only the information provided in the notes. Do not invent requirements or missing details. Clearly distinguish confirmed requirements from assumptions or suggestions. Flag information that requires clarification.

**Expected Output:** Provide a short summary of the main findings, followed by a list of confirmed requirements, assumptions, and clarification questions.

## Improved Result

### Summary

The current process relies on email for employee service requests. Stakeholders are considering a central portal to make submitting and tracking requests easier.

### Confirmed Requirements

- Employees should have a central location to submit service requests.
- Employees should be able to track the status of their requests.
- The process should support the handling of requests that may contain sensitive employee information.

### Assumptions

- The proposed portal would replace or reduce the use of email for submitting requests.
- Different types of service requests may require different information.

### Clarification Questions

1. What types of service requests should be supported by the portal?
2. What request statuses should employees be able to view?
3. Which users should have access to sensitive employee information?
4. What security and access-control requirements should apply?

## What Improved?

- The improved prompt provides a clear Business Analyst context and task.
- It specifies exactly what information should be extracted from the stakeholder notes.
- The rules reduce the risk of the AI inventing requirements or treating assumptions as confirmed facts.
- The output structure makes the results easier to review and use in the requirements-gathering process.