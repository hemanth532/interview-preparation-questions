# 01. Angular Core & Advanced Interview Questions

## Questions

1. Explain Angular architecture for a large-scale enterprise application.
2. What is the difference between standalone components and NgModules?
3. How does Angular change detection work?
4. Explain `OnPush` change detection. When would you use it?
5. What causes unnecessary change detection cycles?
6. How would you optimize a slow Angular application?
7. Explain Angular lifecycle hooks and their practical use cases.
8. What is the difference between `ngOnInit`, `ngAfterViewInit`, and `ngAfterViewChecked`?
9. What are Angular Signals? How are they different from RxJS Observables?
10. When would you use Signals vs BehaviorSubject vs Observable?
11. Explain dependency injection in Angular.
12. What are hierarchical injectors?
13. What is the difference between `providedIn: 'root'`, component providers, and module providers?
14. Explain Angular route guards.
15. Difference between `CanActivate`, `CanActivateChild`, `CanMatch`, and `CanLoad`.
16. How would you implement role-based route authorization?
17. How do you handle token expiration and refresh in Angular?
18. How do HTTP interceptors work?
19. How would you implement global error handling?
20. How do you prevent RxJS subscription memory leaks?
21. Explain `takeUntil`, `async` pipe, and `DestroyRef`.
22. What is the difference between `Subject`, `BehaviorSubject`, `ReplaySubject`, and `AsyncSubject`?
23. Explain RxJS `switchMap`, `mergeMap`, `concatMap`, and `exhaustMap`.
24. How would you implement search with debouncing?
25. How would you cancel an in-flight HTTP request?
26. How would you handle large forms in Angular?
27. Reactive Forms vs Template-driven Forms?
28. How would you build reusable form controls?
29. Explain `ControlValueAccessor`.
30. How do you create reusable Angular components/design systems?

## Senior-Level Follow-Ups

- How would you structure an Angular monorepo for multiple teams?
- How do you prevent shared services from becoming a global-state bottleneck?
- How would you measure Angular performance in production?
- How would you introduce a major Angular version upgrade with minimal risk?


# 02. Angular SSR Interview Questions

## Questions

1. What is Server-Side Rendering (SSR)?
2. SSR vs CSR vs SSG — explain the differences.
3. Why would an enterprise application use Angular SSR?
4. How does Angular SSR work internally?
5. What is Angular hydration?
6. What problems can occur during hydration?
7. What is a hydration mismatch?
8. How do you handle browser-only APIs such as `window`, `document`, and `localStorage` during SSR?
9. How do you determine whether code is running on the browser or server?
10. How would you optimize Angular SSR performance?
11. How would you handle authentication with SSR?
12. Where should authentication tokens/cookies be stored in an SSR application?
13. How would you make API calls during SSR?
14. How do you prevent duplicate API calls between server rendering and browser hydration?
15. What is `TransferState` and why is it useful?
16. How would you debug an SSR application?
17. What happens if an Angular component depends on browser-specific libraries?
18. How would you implement SEO-friendly Angular pages?
19. How does SSR affect caching?
20. How would you deploy an Angular SSR application to Kubernetes?

## Scenario

> Your Angular application works perfectly in the browser but crashes during server rendering with `window is not defined`. How would you troubleshoot and fix it?

### Expected Discussion

- Identify browser-only API usage.
- Separate browser and server execution paths.
- Use Angular platform/browser checks where appropriate.
- Replace or isolate SSR-incompatible libraries.
- Avoid executing browser-specific logic during server rendering.
- Add SSR-specific tests and production monitoring.


# 03. Module Federation Interview Questions

## Questions

1. What is Webpack Module Federation?
2. Why would you use Module Federation in an enterprise Angular application?
3. What is a micro frontend?
4. Micro frontend vs monolithic Angular application?
5. Explain Host, Remote, and Shared Dependencies.
6. How does an Angular application load a remote module?
7. What is the difference between remote entry and host application?
8. How do you share Angular dependencies between micro frontends?
9. Why is `@angular/core` commonly configured as a singleton?
10. What happens if two micro frontends load different Angular versions?
11. How would you manage version compatibility between micro frontends?
12. How do you share authentication between micro frontends?
13. How do micro frontends communicate with each other?
14. How would you handle routing in a Module Federation architecture?
15. How do you handle global state across micro frontends?
16. How would you implement error handling if a remote application is unavailable?
17. What happens if a remote deployment fails?
18. How would you implement fallback UI for a failed remote?
19. How would you independently deploy micro frontends?
20. How would you perform versioning of remote applications?
21. How do you secure remote JavaScript?
22. How would you monitor Module Federation applications in production?
23. What are the disadvantages of Module Federation?
24. When would you not use Module Federation?

## Architecture Scenario

> Design a large enterprise Angular application using Module Federation where five teams independently develop and deploy different business domains.

Discuss:

- Shell/Host application
- Remote applications
- Shared dependencies
- Authentication
- Routing
- State management
- API Gateway
- CI/CD
- Independent deployment
- Version compatibility
- Failure isolation
- Observability
- Security
