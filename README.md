
# Kafka Ingestor Pipeline (Python)

Este projeto consome mensagens de um Kafka, salva em Azure Blob Storage, envia para RabbitMQ e emite alertas via Slack.

## Como usar

1. Configure seu `.env` com base no `.env.example`
2. Rode com Docker:

```
docker build -t kafka-ingestor .
docker run --env-file .env kafka-ingestor
```
