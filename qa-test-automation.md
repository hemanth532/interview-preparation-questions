# 09. QA & Test Automation Interview Questions

## Questions

1. Unit testing vs integration testing vs E2E testing?
2. How do you test Angular components?
3. Jasmine/Karma vs Jest?
4. How do you mock HTTP requests?
5. How do you test Angular services?
6. How do you test route guards?
7. How do you test HTTP interceptors?
8. How do you test RxJS code?
9. How do you test an Angular application using Playwright/Cypress?
10. What should be covered by unit tests vs E2E tests?
11. How would you test a payment workflow without actually charging a customer?
12. How do you integrate automated tests into CI/CD?
13. How do you prevent flaky tests?
14. What code coverage percentage would you target?
15. Does high code coverage guarantee good quality?
16. How would you test Module Federation remotes?
17. How would you perform contract testing between frontend and backend?

## Testing Pyramid

```text
             E2E
          /-------\
       Integration
      /-------------\
          Unit
    /-------------------\
```

Prefer many fast unit tests, a useful integration layer, and fewer high-value E2E tests.

## Production Quality

Test:

- Functional behavior
- Accessibility
- Performance
- Security
- Browser compatibility
- API contracts
- Error scenarios
- Authentication/authorization
- Deployment and rollback paths
