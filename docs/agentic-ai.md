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
