# Contract Intelligence API — README

## Overview
A production-ish FastAPI service that ingests contract PDFs, extracts structured fields, answers questions via RAG, and audits clauses for risk. The service runs locally inside Docker and exposes OpenAPI docs.


This repo includes:
- FastAPI app (app/)
- Prompts (prompts/)
- Eval QA set + script (eval/)
- Tests (tests/) — example unit & integration tests
- Dockerfile + docker-compose.yml



## Quick start (development)


Requirements: Docker & docker-compose (or Docker Desktop), make


1. Copy sample PDFs into `sample_pdfs/` (the repo includes 3 public sample contracts — see `sample_pdfs/README.md`).
2. Build & run:


```bash
make up
# or
docker-compose up --build
