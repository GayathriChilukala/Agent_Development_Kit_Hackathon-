# Agent_Development_Kit_Hackathon-


```
bq load \
--autodetect \
--source_format=CSV \
--skip_leading_rows=1 \
--max_bad_records=10 \
support_tickets.tickets_full \
gs://support-tickets-bucket/aa_dataset-tickets-multi-lang-5-2-50-version.csv
```
```
bq load \
--autodetect \
--source_format=CSV \
--skip_leading_rows=1 \
--max_bad_records=100 \
--allow_quoted_newlines \
support_tickets.tickets_4k \
gs://support-tickets-bucket/dataset-tickets-multi-lang3-4k.csv
```

```
bq load \
--autodetect \
--source_format=CSV \
--skip_leading_rows=1 \
--max_bad_records=10 \
support_tickets.tickets_20k \
gs://support-tickets-bucket/dataset-tickets-multi-lang-4-20k.csv
```


#1. Data Ingestion and Storage
Dataset: Utilize the Multilingual Customer Support Tickets Dataset.

Storage: Upload the dataset to Google Cloud Storage (GCS).

BigQuery: Import the data into BigQuery for structured querying and analysis.

#2. Agent Development with ADK
Framework: Use the Agent Development Kit (ADK) to define and orchestrate agents.

Agent Communication: Implement inter-agent communication using ADK's built-in protocols.

Deployment: Deploy agents using Cloud Run for scalability.
Google GitHub
+1
Google GitHub
+1

#3. Integration with Google Cloud Services
Vertex AI: Employ Vertex AI's language models for sentiment analysis and response generation.

BigQuery: Query the knowledge base to fetch relevant information for responses.

Cloud Functions: Trigger workflows based on events, such as the arrival of a new ticket.


Key Features:

Agent 1: Ticket Classifier – Categorizes incoming tickets (e.g., billing, technical support).

Agent 2: Sentiment Analyzer – Assesses the sentiment of the customer's message.

Agent 3: Knowledge Base Querier – Retrieves relevant information from a BigQuery-powered knowledge base.

Agent 4: Response Generator – Crafts a personalized response using Vertex AI's language models.

Agent 5: Escalation Manager – Determines if the ticket should be escalated to a human agent.
