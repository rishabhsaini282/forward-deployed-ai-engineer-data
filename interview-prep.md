# FDE Interview Prep: 50 Questions & Case Frameworks

FDE interviews screen for problem-structuring and integration thinking, not LeetCode. Expect a 3-stage loop: Behavioral/Posture (45m), Technical Deep Dives (2x 60-75m), and the Decomposition Case Study.

## Part 1: The Decomposition Case Study
You will be handed a highly vague enterprise problem. You are evaluated on discovery hygiene and MVP isolation.

### Case Example: Fortune 100 Bank Compliance
**Prompt:** "A Fortune 100 bank wants an AI agent to automate internal portfolio compliance audits. Data is trapped across three legacy mainframes, and parameters change quarterly based on multi-state regulations. Design the deployment strategy."

**Step 1: Ask Discovery Questions Unprompted**
1.  "What is the baseline latency threshold for an individual compliance audit report generation?"
2.  "How are regulatory updates currently ingested and verified by the human compliance team?"
3.  "Do we have direct access to place a secure API proxy layer over the legacy mainframes, or must we work via intermediate batch exports?"

**Step 2: Propose the MVP Framework**
*   Propose a localized, read-only document extraction pipeline targeting a single regulatory framework first.
*   Build a validated eval dataset using historical reports before expanding to multi-state processing.

---

## Part 2: Core Question Bank

### API Composition & Data Pipelines
1.  Design an ingestion pipeline processing 50,000 multi-format documents per hour into a vector DB. How do you handle mixed tables and text?
2.  How do you build a secure, HIPAA-compliant proxy layer between a healthcare stack and a third-party LLM API? Detail consent-revocation logic.
3.  Construct a PySpark pipeline to enforce a clean target ontology on highly unstructured ERP data exports.
4.  Architect a real-time retrieval pipeline using an MCP server. What are the latency bottlenecks?
5.  How do you handle rate-limiting and token throttling across multiple downstream API keys?

### Infrastructure & Cloud IAM
6.  Configure cross-account AWS IAM roles for secure agentic tool access without exposing root privileges.
7.  Detail mitigation strategies against prompt injection targeting backend storage via user input.
8.  Defend against training data poisoning in an active production feedback loop.
9.  Establish isolated staging and production environments inside a regulated financial stack.
10. What are the infrastructure trade-offs of an on-premise deployment versus a managed cloud API?

### RAG & Model Evaluation
11. Design an automated eval suite to catch subtle model regressions before shipping to production.
12. Detail mathematical differences between recall@k, Mean Reciprocal Rank (MRR), and hit-rate analysis.
13. Build a deterministic and cost-effective LLM-as-a-Judge pipeline at enterprise scale.
14. Construct baseline datasets to validate that an enterprise chatbot does not leak proprietary data.
15. Wire an automated rollback gate into CI/CD after a compliance team flags a hallucination pattern.
16. Optimize context window usage for long, multi-turn conversational histories.
17. What are the benefits of hybrid search (sparse + dense) over dense embeddings alone?
18. Resolve the "lost in the middle" phenomenon when passing long contexts to LLMs.
19. Dynamically adjust chunk sizes based on document metadata filters.
20. Manage vector database index fragmentation during thousands of daily real-time updates.

### Advanced Agentic Workflows
21. Architect a deterministic routing layer to prevent multi-agent infinite loop states.
22. Implement safeguards for an agent granted direct write access to a production CRM.
23. Log and audit agentic execution paths for compliance tracking in regulated industries.
24. Optimize state management when workflows span asynchronous, long-running human approval steps.
25. Identify failure modes when relying on dynamic, model-generated tool schema definitions.

### Global Compliance (E-E-A-T)
26. Adjust deployment strategies to comply with the geographical boundaries of the EU AI Act.
27. Ensure applications strictly adhere to localized SOC 2 Type II data handling requirements.
28. Prevent PII from leaking into shared foundational model caching layers.
29. Build a verifiable audit trail for an AI-generated decision within insurance claims.
30. Handle data governance when utilizing public APIs for private enterprise workflows.

### Behavioral & Client Posture
*(Note: Not a culture-fit screen—evaluates if you can hold ground with hostile stakeholders while protecting the relationship)*
31. Tell me about a time you discovered the SOW problem was completely different from the actual bottleneck.
32. Respond to a client CTO who insists on custom fine-tuning when simple RAG solves the business goal.
33. Describe a critical technical mistake during a live deployment. How did you handle remediation?
34. Balance writing clean production code with intense timeline pressures of an on-site pilot.
35. Establish trust when a client's data engineering team views you as an outsourced threat.
36. Translate a complex system regression metrics shift into a clear ROI metric for a corporate sponsor.
37. Identify a contract expansion opportunity proactively during integration.
38. Manage scope creep when a customer requests out-of-bounds custom platform enhancements.
39. What metrics prove an AI deployment has moved from pilot to production readiness?
40. Handle a scenario where internal security completely blocks your cloud architecture due to legacy policies.
