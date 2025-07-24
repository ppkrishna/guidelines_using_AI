# guidelines_using_AI

**Detection and Logging**

1. Prompt Monitoring: Prompts are scanned using moderation filters that detect hate speech, threats, or other harmful content.
2. Logging: If a prompt violates policies, it can be logged securely for review. This log may include:
3. The prompt text
4. Timestamp
User/session ID (if applicable)
Action taken (e.g., blocked, flagged)

🚨 **Actions That Can Be Taken**

1. **Immediate Blocking**: The system can prevent the response from being generated and show a warning to the user.
2. **Flagging for Review**: The incident can be flagged for human moderators or testers to review.
3. **Escalation**: In enterprise or sensitive environments, it can trigger alerts to admins or compliance teams.
4. **User Restrictions**: Repeated violations may lead to temporary or permanent restrictions on the user’s access.
