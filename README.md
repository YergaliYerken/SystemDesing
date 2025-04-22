# SystemDesing
# Microservice Rate Limiting with Redis

This repo demonstrates how to implement a Token Bucket rate-limiting mechanism in a FastAPI microservice using Redis for tracking request counts.

## Features
- Token Bucket algorithm
- Per-IP rate limits
- Configurable via `.env`
- Returns `429 Too Many Requests` when limit exceeded

## Configuration
Set the following env vars:
- `RATE_LIMIT`: Max requests per user/IP
- `REFILL_RATE`: Tokens added per second
- `BUCKET_SIZE`: Max tokens per bucket

## Running Locally
```bash
docker-compose up --build
