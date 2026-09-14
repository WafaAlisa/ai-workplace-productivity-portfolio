# Information Processing Example

## Purpose

This example demonstrates **summarizing, extracting, restructuring, and prioritizing** unstructured stakeholder notes into a decision-ready Business Analysis brief.

## 1. Raw Input

> Service improvement meeting notes: The current employee service request process uses email and a spreadsheet to track requests. Operations reported that employees frequently ask for updates because they cannot see the status of their requests. The team discussed creating a central service portal. Wafa from Operations will provide the top five request types by 18 September. The Business Analyst will document the current process, but no deadline was agreed. IT said the portal would need to consider access controls because some requests contain sensitive information. HR wants to review the proposed process before implementation. No decision has been made on whether the portal should replace email completely. The team agreed that improving request visibility is a priority. The next meeting is scheduled for 22 September.

## 2. Prompt Used

**Context:** I am a Business Analyst converting unstructured stakeholder meeting notes into a decision-ready brief for a fictional internal service improvement project.

**Action:** Summarize the notes, extract confirmed decisions and action items, identify risks and open questions, and prioritize the items that require attention.

**Rules:** Use only the information provided. Do not invent owners, deadlines, decisions, or requirements. Clearly distinguish confirmed information from suggestions and unresolved issues. Mark missing information as `[Not Specified]`.

**Expected Output:** Provide a short summary, followed by confirmed decisions, action items, risks, and open questions. Use an action-item table with Action Item, Owner, Deadline, Priority, and Status.

## 3. AI Output - First Draft

### Summary

- The current service request process uses email and spreadsheets.
- The team will create a central service portal to replace the current process.
- The portal will allow employees to track their requests.
- Wafa will provide the top five request types by 18 September.
- IT will implement the required access controls.
- HR will approve the proposed process before implementation.

### Action Items

| Action Item | Owner | Deadline | Priority | Status |
|---|---|---|---|---|
| Provide top five request types | Wafa | 18 September | High | In progress |
| Document current process | Business Analyst | 22 September | High | In progress |
| Implement access controls | IT | 22 September | High | Planned |
| Approve proposed process | HR | 22 September | High | Pending |

## 4. Human Review

The first draft contains several unsupported assumptions:

- The notes say a central portal was **discussed**, not that the team decided to create one.
- There is no confirmed decision to replace email completely.
- The notes do not say that the portal will definitely include request tracking as a confirmed feature.
- IT identified access controls as something to consider, but no implementation deadline was provided.
- HR wants to review the proposed process, but this does not mean HR has agreed to approve it.
- The Business Analyst has no confirmed deadline for documenting the current process.
- The status of Wafa's action was not provided.

I corrected these issues and preserved the uncertainty in the final output.

## 5. Final Structured Output

### Decision-Ready Summary

The current employee service request process relies on email and a spreadsheet, which makes it difficult for employees to track request status. The team discussed a central service portal as a possible improvement, but no decision has been made to implement it or replace email completely.

Improving request visibility was identified as a priority. The main immediate actions are to understand the most common request types, document the current process, and clarify security and process requirements.

### Confirmed Information

- The current process uses email and a spreadsheet.
- Employees frequently ask for updates because they cannot see request status.
- Improving request visibility is a priority.
- Wafa from Operations will provide the top five request types by 18 September.
- HR wants to review the proposed process before implementation.
- The next meeting is scheduled for 22 September.

### Action Items

| Action Item | Owner | Deadline | Priority | Status |
|---|---|---|---|---|
| Provide the top five request types | Wafa, Operations | 18 September | High | Open |
| Document the current service request process | Business Analyst | `[Not Specified]` | High | Open |
| Review access-control requirements for sensitive requests | IT | `[Not Specified]` | High | Open |
| Review the proposed process | HR | `[Not Specified]` | Medium | Open |

### Risks and Open Questions

- **Process visibility risk:** Employees currently have limited visibility of request status.
- **Security consideration:** Some requests contain sensitive information, so access controls need to be clarified.
- **Solution decision:** It has not been decided whether a central portal will be implemented.
- **Email dependency:** It has not been decided whether the portal would replace email completely.
- **Process review:** The timing and scope of HR's review have not been specified.

### Priority Focus

1. Document the current process and identify the main pain points.
2. Gather the most common request types from Operations.
3. Clarify access and security requirements.
4. Confirm the proposed future process with relevant stakeholders.
5. Decide whether a central portal is the appropriate solution.

## Information Tasks Used and Why

- **Summarizing:** to reduce lengthy stakeholder notes to the most important business information.
- **Extracting:** to identify decisions, actions, owners, deadlines, risks, and open questions.
- **Restructuring:** to convert unstructured meeting notes into a decision-ready format.
- **Prioritizing:** to identify which business analysis activities should be addressed first.