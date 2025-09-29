# ELK Stack with Docker Compose

This repository provides a simple setup to run the ELK Stack (Elasticsearch, Logstash, Kibana) using Docker Compose.

📦 Services

Elasticsearch – stores and indexes logs

Logstash – processes and ships logs into Elasticsearch

Kibana – visualizes data from Elasticsearch

🚀 Getting Started
# 1. Prerequisites

Docker
 (Linux, macOS, or Windows with WSL2 recommended)

Docker Compose
 (v1 or v2 both work)
 ⚠️ Make sure you’ve allocated at least 2–4 GB RAM in Docker Desktop for Elasticsearch.

# 2. Clone the Repository
gh repo clone RISHI-1704/elk-docker-compose
cd 

# 3. Start the Stack
docker compose up -d

# 4. Access the Services

- Elasticsearch → http://localhost:9200

- Kibana → http://localhost:5601

📂 Logs Input

Place your log files inside the ./logs directory.

Configure Logstash pipelines inside ./logstash/pipeline/*.conf.

🔄 Managing the Stack

Stop services:

- docker compose down   # (or docker-compose down)

View logs:

- docker compose logs -f   # (or docker-compose logs -f)
