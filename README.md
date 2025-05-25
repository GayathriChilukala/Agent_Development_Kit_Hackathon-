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
