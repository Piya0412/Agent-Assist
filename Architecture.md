Purpose: Visual and textual explanation of system architecture.

Structure:

System diagram (embed or link to a draw.io/Lucidchart diagram)

Description of main components (e.g., AWS Bedrock, LangGraph, FastAPI)

Data flow between components

Component interaction details



System Architecture

**High-Level Flow:**
1. FastAPI receives agent query → extracts context
2. LangGraph orchestrates: RAG → Bedrock inference → decision routing
3. Response streams back to agent in real-time

**Tech Stack:**
- Backend: FastAPI (ASGI), LangGraph (stateful graphs)
- AI: AWS Bedrock (Claude 3.5 Sonnet recommended)
- Storage: DynamoDB (sessions), S3 (knowledge base)
- Infra: ECS Fargate, ALB, CloudWatch
