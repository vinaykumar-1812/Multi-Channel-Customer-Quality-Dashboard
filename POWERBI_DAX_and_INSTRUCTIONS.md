Power BI DAX Measures (copy into New Measure):

Avg Handle Time (sec) = AVERAGE(interactions_for_powerbi[handle_time_seconds])

FCR Rate = AVERAGE(interactions_for_powerbi[first_call_resolution])

Avg CSAT = AVERAGE(interactions_for_powerbi[csat])

Compliance Violations = SUM(interactions_for_powerbi[compliance_violation])

Resolution Rate = AVERAGE(interactions_for_powerbi[resolved])

Quality Score = AVERAGE(interactions_for_powerbi[quality_score])

Notes:
- Create 'Month' column in Power BI: FORMAT(interactions_for_powerbi[timestamp], "YYYY-MM")
- Format percentage measures appropriately.
- Use slicers for Channel and Agent.
