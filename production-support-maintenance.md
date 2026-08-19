# 10. Production Support & Maintenance Interview Questions

## Questions

1. Your Angular application suddenly becomes slow in production. What do you do?
2. API response time increased from 200 ms to 5 seconds. How do you investigate?
3. Memory usage keeps increasing in a Node.js service. How do you troubleshoot?
4. A remote Module Federation application fails after deployment. What do you do?
5. A production deployment causes 500 errors. How do you respond?
6. How do you perform rollback?
7. How do you implement zero-downtime releases?
8. What metrics would you monitor?
9. What logs would you collect?
10. How would you implement distributed tracing?
11. What is an SLI?
12. What is an SLO?
13. What is an SLA?
14. How would you conduct a production incident investigation?
15. How do you perform root-cause analysis?
16. What should be included in a postmortem?

## Production Checklist

- Check monitoring dashboards.
- Identify when the issue started.
- Compare recent deployments/configuration changes.
- Check frontend errors and API errors.
- Check latency and throughput.
- Check infrastructure health.
- Determine blast radius.
- Mitigate first.
- Roll back if required.
- Communicate impact.
- Identify root cause.
- Add preventive monitoring/tests.
- Document the incident.

## Observability

Understand:

- Logs
- Metrics
- Traces
- Correlation IDs
- Error rates
- Latency
- Throughput
- Availability
- Resource utilization
