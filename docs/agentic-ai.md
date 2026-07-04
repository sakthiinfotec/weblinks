MCP vs ADK

## MCP
- Standard prorocol and interface used by AI Agent (or an LLM Host) to communicate with the external resources via JSON-RPC
- External resources like
  * PostgresSQL DB
  * Web Scrap
  * Local Filesystem

MCP is an open protocol that standardizes how AI agents interact with their environment. The AI agent hosts an MCP client, and the tools and resources it interacts with are MCP servers. The MCP client can communicate with the MCP server over two distinct transport types:

- Server Sent Events (SSE) or Streamable HTTP
- Standard Input/Output (stdio)

 **MCP Client** is an AI Agent (or an LLM Host)
 **MCP Server** is the one expose tools and data to the client
 
### Agentic AI
<img width="985" height="460" alt="image" src="https://github.com/user-attachments/assets/b668b96c-79f3-4847-9bdb-a6ee34ccbd64" />


### Usecases
- [Gem - AI recruiting agents](https://www.gem.com/product/recruiting-ai)
  - **AI Sourcing Agent** — Finds top candidates across 800M+ profiles, flags past interactions, and personalizes outreach to help recruiters build relationships.
  - **AI Fraud Detection Agent** — Evaluates risk across multiple signals and flags suspicious applications with no added friction, so recruiters focus on real candidates.
  - **AI Inbound Agent** — Processes thousands of incoming applications, assigns explainable match scores, and surfaces the best fits instantly while the recruiter makes final decisions.
  - **AI Talent Rediscovery** — Surfaces past applicants and silver medalists from your ATS and CRM, showing complete interview history and engagement so conversations can resume seamlessly.
  - **AI Talent Insights** — Breaks down talent pools by role, location, company, and tenure to help recruiters set expectations with hiring managers using data.
  - **AI Outreach Personalization** — Crafts authentic sequences across email, InMail, and SMS based on candidate profiles, with automated follow-ups that achieve 30-40% higher response rates.
