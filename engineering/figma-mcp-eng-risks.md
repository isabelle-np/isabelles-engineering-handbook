# Engineering Concerns: Figma MCP

## 1. Security & Data Access

- Unauthorized access to Figma files or design systems
- Over-permissioned MCP servers (read/write when read-only is sufficient)
- Exposure of sensitive design data or unreleased product concepts
- Insecure handling of API tokens, credentials, or secrets
- Lack of network isolation between MCP infrastructure and production systems
- Potential data exfiltration via AI-assisted tooling
- Insufficient logging and monitoring of MCP interactions

## 2. Identity, Authentication, and Authorization

- Inconsistent identity mapping between Figma users, IDE users, and MCP services
- Lack of fine-grained role-based access control
- Difficulty enforcing least-privilege access
- Challenges integrating MCP authentication with enterprise SSO and IAM systems
- Revocation delays when users change roles or leave the organization

## 3. Compliance, Legal, and Data Governance

- Unclear data ownership and IP implications for AI-generated output
- Regulatory compliance concerns (SOC 2, ISO, GDPR, etc.)
- Retention policies for MCP logs, prompts, and outputs
- Data residency requirements not being met
- Third-party vendor risk and contractual limitations
- Inconsistent audit trails for AI-assisted actions

## 4. Architecture & Infrastructure

- MCP server reliability and uptime requirements
- Scalability constraints as adoption grows
- Single points of failure in MCP-hosted environments
- Network latency impacting IDE performance
- Environment separation (dev, staging, production) not clearly defined
- Dependency on local machines vs centralized servers
- Upgrade and versioning strategy for MCP servers

## 5. Design System Maturity & Data Quality

- Poor Figma file hygiene leading to unreliable MCP outputs
- Inconsistent naming conventions across components and tokens
- Missing or incomplete metadata in design files
- Fragmented design systems across teams
- Design debt becoming amplified by automation
- MCP outputs reflecting outdated or deprecated patterns

## 6. AI Output Quality & Reliability

- Hallucinated or incorrect design interpretations
- Misalignment between design intent and generated outputs
- Over-reliance on AI-generated recommendations
- Lack of deterministic behavior across similar prompts
- Difficulty debugging or reproducing AI-driven outputs
- Inconsistent results across IDEs or MCP clients

## 7. Engineering Workflow Integrity

- AI-generated code not aligning with internal architecture standards
- Violations of accessibility, performance, or security best practices
- Generated code bypassing existing review processes
- Increased tech debt if outputs are accepted without validation
- Difficulty integrating AI output into CI/CD pipelines
- Loss of contextual understanding by engineers

## 8. Governance & Change Management

- Lack of ownership for MCP configuration and rules
- No clear process for updating custom instructions or guardrails
- Inconsistent adoption patterns across teams
- Difficulty rolling back changes caused by MCP-assisted actions
- Shadow usage of MCP outside approved environments
- Inadequate communication of changes or best practices

## 9. Observability & Monitoring

- Limited visibility into how MCP is being used
- No clear metrics for success or failure
- Difficulty detecting misuse or anomalous behavior
- Lack of feedback loops to improve outputs
- Insufficient alerting for failures or policy violations

## 10. Vendor Lock-In & Dependency Risk

- Tight coupling to Figma-specific APIs and data models
- Limited portability of MCP workflows to other design tools
- Risk of breaking changes from Figma API or MCP updates
- Dependency on third-party IDE or AI tooling
- Long-term maintainability concerns

## 11. Performance & Cost Management

- Increased compute costs for MCP servers
- Unclear cost attribution across teams
- Inefficient usage patterns driving unnecessary load
- Performance degradation in IDEs
- Lack of usage quotas or throttling mechanisms

## 12. Human Factors & Skill Gaps

- Designers and engineers misinterpreting MCP outputs
- Insufficient training on proper MCP usage
- Erosion of design and engineering craftsmanship
- Overconfidence in AI-driven results
- Resistance to adoption due to trust concerns

## Strategic Summary

Figma MCP introduces powerful capabilities, but at enterprise scale it must be treated as:

- A platform integration, not a plugin
- A governed system, not an ad-hoc tool
- A human-in-the-loop accelerator, not an autonomous actor
