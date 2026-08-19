# 12. Scenario-Based Interview Questions

These scenarios combine Angular, SSR, Module Federation, Node.js, Kubernetes, testing, architecture, and production support.

## Scenario 1 — Module Federation

> You have 8 Angular micro frontends. Each team deploys independently. After an Angular upgrade, three remotes stop loading. How would you identify and solve the issue?

Discuss:

- Angular version compatibility
- Shared dependency configuration
- Singleton dependencies
- Remote/host compatibility
- Lock files
- Build artifacts
- Deployment versions
- Rollback strategy

## Scenario 2 — SSR

> SSR works locally but fails in production Kubernetes pods. How would you troubleshoot it?

Discuss:

- Server logs
- Environment variables
- Node.js runtime
- Browser-only APIs
- SSR-compatible dependencies
- Network/API access
- Health probes
- Container configuration

## Scenario 3 — Performance

> An Angular application has a 12 MB JavaScript bundle and takes 7 seconds to become interactive. How would you optimize it?

Discuss:

- Bundle analysis
- Lazy loading
- Code splitting
- Tree shaking
- Dependency reduction
- OnPush
- Signals
- Image optimization
- CDN
- SSR/hydration
- Caching

## Scenario 4 — Memory Leak

> Users report that the browser becomes slower after keeping the application open for several hours. How would you investigate?

Discuss:

- Chrome DevTools
- Heap snapshots
- Detached DOM nodes
- RxJS subscriptions
- Event listeners
- Timers
- Large caches
- Global references

## Scenario 5 — Production Incident

> A new deployment causes 20% of requests to fail. What is your immediate response?

Discuss:

1. Assess severity and blast radius.
2. Check dashboards/logs/traces.
3. Compare deployment versions.
4. Stop further rollout.
5. Roll back if appropriate.
6. Communicate status.
7. Investigate root cause.
8. Add preventive controls.

## Scenario 6 — Architecture

> You need to migrate a 10-year-old Angular monolith to micro frontends without stopping business development. How would you approach the migration?

Discuss:

- Domain boundaries
- Strangler pattern
- Shell application
- Incremental remote extraction
- Shared dependencies
- API boundaries
- Feature flags
- Independent deployment
- Rollback

## Scenario 7 — Kubernetes

> Your Angular SSR pod keeps restarting. What commands, metrics, logs, and configuration would you check?

Discuss:

- Pod status
- Logs
- Events
- Previous logs
- OOMKilled
- CPU/memory limits
- Probes
- Environment variables
- Secrets
- Deployment configuration

## Scenario 8 — Large Data

> An API returns 500,000 records and the Angular UI becomes unresponsive. How would you redesign the solution?

Discuss:

- Server-side pagination
- Filtering
- Sorting
- Virtual scrolling
- Streaming where appropriate
- Compression
- API limits
- Caching
- Background processing

## Scenario 9 — Authentication

> Multiple Module Federation applications need to use the same enterprise authentication system. How would you design it?

Discuss:

- Central identity provider
- OAuth 2.0/OIDC
- Access tokens
- Secure cookies where appropriate
- Token lifecycle
- Shared authentication state
- Authorization
- Logout propagation
- Avoiding token duplication

## Scenario 10 — Team Scaling

> Fifteen teams are working on the same frontend platform. How do you prevent dependency conflicts and inconsistent coding practices?

Discuss:

- Shared engineering standards
- Monorepo or controlled package strategy
- Shared libraries
- Versioning
- Automated CI checks
- Dependency management
- Architecture governance
- ADRs
- Code ownership
- Automated security and quality checks

## Final Interview Exercise

> Design an enterprise Angular platform using SSR and Module Federation, deployed on Kubernetes, backed by Node.js services, with automated testing and production observability.

Your answer should cover:

```text
Users
  ↓
CDN / WAF
  ↓
Load Balancer / Ingress
  ↓
Angular Shell + SSR
  ↓
Module Federation Remotes
  ↓
API Gateway
  ↓
Node.js Services
  ↓
Databases / External Services

Cross-Cutting:
- Authentication
- Authorization
- CI/CD
- Testing
- Monitoring
- Logging
- Distributed tracing
- Security
- Caching
- Feature flags
- Disaster recovery
```
