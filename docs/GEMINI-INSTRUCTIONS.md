
# GitHub MCP Server Instructions for Gemini CLI

This document provides instructions for the Gemini CLI on how to interact with the GitHub MCP server.

## API Requests

All API requests must be sent to the following endpoint:

\`\`\`
https://mcp.github.com/
\`\`\`

The request body must be a JSON object with the following properties:

* \`tool\`: The name of the tool to use.
* \`parameters\`: An object containing the parameters for the tool.

## Authentication

The Gemini CLI must authenticate with the GitHub MCP server by providing a GitHub App token in the \`Authorization\` header of each request. The token should be prefixed with \`Bearer \`.

## Responses

The GitHub MCP server will respond with a JSON object containing the following properties:

* \`result\`: The result of the tool execution.
* \`error\`: An error message if the tool execution failed.
