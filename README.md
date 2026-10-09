# Project 1 — KQL Log Analysis

## Overview
This project demonstrates hands-on log analysis using Kusto Query Language (KQL) in Azure Data Explorer with sample data.

## Objectives
- Explore log tables and their schemas.
- Count events by log level and component.
- Identify repeated message patterns.
- Analyze event counts over time.
- Practice writing and understanding KQL queries.

## Tools Used
- Microsoft Azure Data Explorer
- Kusto Query Language (KQL)
- GitHub

## Queries Practiced
- `take` — retrieve sample records.
- `getschema` — inspect table columns and data types.
- `summarize` and `count()` — aggregate event counts.
- `order by` — sort results.
- `bin()` — group timestamps into time intervals.
- `project` — select columns for analysis.

## Data Source
Azure Data Explorer sample data. The `TraceLogs` table contains application and benchmark-processing messages. This project is a KQL learning exercise, not a confirmed security incident investigation.

## Key Learning Outcomes
- Learned to explore unfamiliar tables.
- Practiced aggregating and sorting log events.
- Examined repeated messages and time-based event counts.
- Developed foundational KQL skills relevant to security operations.

## Evidence
Screenshots of the queries and their results will be added to this repository.

## Disclaimer
This project uses sample data for educational purposes. No real security incident or attack is claimed.
