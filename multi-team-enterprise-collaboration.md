# 11. Multi-Team Collaboration & Enterprise Delivery

## Questions

1. How do you handle conflicting requirements between teams?
2. How do you establish coding standards across multiple Angular teams?
3. How would you manage shared Angular libraries?
4. How do you prevent breaking changes in shared libraries?
5. How would you establish API contracts between teams?
6. How do you handle dependency upgrades across 10 teams?
7. How would you introduce a new Angular version into a large enterprise application?
8. How do you handle technical debt?
9. Tell me about a time you resolved a production issue involving multiple teams.
10. How do you communicate an architectural decision to other teams?

## Enterprise Practices

### Ownership

Each domain should have a clearly identified owning team.

### Shared Libraries

Define:

- API ownership
- Versioning
- Compatibility policy
- Release process
- Deprecation policy
- Documentation
- Automated tests

### Dependency Management

Use:

- Lock files
- Automated dependency scanning
- Compatibility testing
- Incremental upgrades
- Release notes
- Shared upgrade plans

### Architecture Governance

Use lightweight:

- ADRs
- Architecture reviews
- Coding standards
- Security reviews
- Performance budgets
- CI quality gates

## Behavioral Scenario

> Fifteen teams depend on a shared Angular library. A breaking change is required. How would you introduce it?

Strong answer:

1. Assess consumers.
2. Introduce a backward-compatible API.
3. Deprecate the old API.
4. Publish migration guidance.
5. Give teams a migration window.
6. Track adoption.
7. Remove the old API in a planned major release.
