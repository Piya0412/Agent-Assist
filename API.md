Purpose: Document all API endpoints.

Structure:

OpenAPI specification (YAML/JSON) embedded or linked

Endpoint details (path, method, description)

Request/response schemas

Example requests and responses



# In main.py - Auto-generates docs
from fastapi import FastAPI
app = FastAPI(title="Enterprise Agent Assist", version="1.0.0")

@app.post("/v1/assist")
async def agent_assist(request: AgentRequest):
    """Real-time agent assistance endpoint"""
    # LangGraph workflow invocation
    return {"suggestions": [...], "confidence": 0.92}
