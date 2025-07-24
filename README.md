# guidelines_using_AI

**Detection and Logging**

1. Prompt Monitoring: Prompts are scanned using moderation filters that detect hate speech, threats, or other harmful content.
2. Logging: If a prompt violates policies, it can be logged securely for review. This log may include:

**The prompt text**
**Timestamp**
**User/session ID (if applicable)**
**Action taken (e.g., blocked, flagged)**

🚨 **Actions That Can Be Taken**

1. **Immediate Blocking**: The system can prevent the response from being generated and show a warning to the user.
2. **Flagging for Review**: The incident can be flagged for human moderators or testers to review.
3. **Escalation**: In enterprise or sensitive environments, it can trigger alerts to admins or compliance teams.
4. **User Restrictions**: Repeated violations may lead to temporary or permanent restrictions on the user’s access.


**Expected System Behavior**

a. **Blocking the Response**

The system should not generate a reply to hate speech.
Instead, it should return a standard warning message, such as:

Response should be : **"I'm sorry, but I can't help with that request."**

This ensures no harmful content is echoed or amplified.

b. **Logging the Event**
The system should log the following:
1. Prompt text (with redaction if needed)
2. Timestamp
3. User/session ID (if applicable)
4. Violation type (e.g., hate speech, harassment)
5. Action taken (e.g., blocked, flagged)

**This log is typically stored in a secure audit trail for compliance and review**

c. **Sending Alerts or Flags**

The system can:
**Flag the session for human review**
**Send alerts to moderators or admins**
**Trigger automated workflows, such as:**
=>User warning
=>Session termination
=> **Escalation to legal/compliance teams**
