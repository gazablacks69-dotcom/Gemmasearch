---
name: web-search
description: Search the web for current information, news, facts, or anything the user asks to look up. Trigger on phrases like "search for", "look up", "find", "what is", "who is", "latest news on".
secrets:
  - name: GOOGLE_API_KEY
    description: Your Google Custom Search API key
  - name: SEARCH_ENGINE_ID
    description: Your Programmable Search Engine ID
---

# Web Search

## Instructions
When the user asks you to search for something or find information:

1. Extract the search query from the user's message
2. Call the run_js tool with:
   - script name: index.html
   - data: a JSON string with this field:
     - query: String. The search terms to look up
3. Present the results clearly with titles, snippets, and links
4. Summarize what you found in a helpful response
---
