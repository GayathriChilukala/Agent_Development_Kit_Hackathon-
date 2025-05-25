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
