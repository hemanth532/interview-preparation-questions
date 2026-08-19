# 07. System Design Interview Questions

## Question 1: Enterprise Angular Platform

> Design an enterprise Angular application used by millions of users.

Cover:

- CDN
- SSR
- Angular
- Module Federation
- API Gateway
- Backend services
- Authentication
- Caching
- Database
- Observability
- CI/CD
- Kubernetes
- Disaster recovery

## Question 2: Micro Frontend Platform

> Design a micro frontend architecture where 10 teams can deploy independently.

Cover:

- Shell/Host
- Remote applications
- Shared dependencies
- Versioning
- CI/CD
- Independent deployment
- Communication
- Authentication
- Monitoring
- Failure isolation

## Question 3: Remote Failure

> One remote application goes down in production. What happens to the entire application?

Discuss:

- Timeout
- Retry
- Fallback UI
- Graceful degradation
- Cached/static fallback
- Alerting
- Error boundaries/failure isolation

## Question 4: Performance

> An Angular application takes 8 seconds to load. How would you troubleshoot it?

Suggested flow:

```text
Measure
  ↓
Network analysis
  ↓
Bundle analysis
  ↓
JavaScript execution
  ↓
API performance
  ↓
Rendering
  ↓
Change detection
  ↓
Lazy loading
  ↓
Caching/CDN
  ↓
SSR/Hydration
```

## Question 5: Legacy Migration

> How would you migrate a large Angular monolith to micro frontends without stopping business development?

Discuss:

- Domain decomposition
- Strangler migration
- Shell introduction
- Remote extraction
- Shared dependency strategy
- Incremental rollout
- Feature flags
- Contract testing
- Rollback
- Team ownership
