# 08. Kubernetes Interview Questions

## Questions

1. What is Kubernetes?
2. What is a Pod?
3. Deployment vs Service?
4. What is an Ingress?
5. ConfigMap vs Secret?
6. What is a ReplicaSet?
7. How does Kubernetes perform scaling?
8. What is Horizontal Pod Autoscaler?
9. Liveness vs readiness probes?
10. How would you deploy an Angular SSR application to Kubernetes?
11. How would you deploy a Node.js API to Kubernetes?
12. How would you perform zero-downtime deployment?
13. Rolling deployment vs blue-green deployment?
14. How would you troubleshoot a pod that keeps restarting?
15. How would you troubleshoot a service that is unreachable?
16. How do you manage environment-specific configuration?
17. How do you monitor applications running in Kubernetes?

## Scenario

> Your Angular SSR pod keeps restarting in production. How would you investigate?

Check:

- Pod status
- Container logs
- Previous container logs
- Events
- Readiness/liveness probes
- CPU and memory limits
- OOMKilled status
- Environment variables
- Secret/configuration issues
- Node/SSR runtime errors
- Dependency failures

## Important Concepts

`Pod → Deployment → Service → Ingress`

Also understand:

- Rolling updates
- Autoscaling
- Health probes
- Resource requests/limits
- Secrets
- ConfigMaps
- Namespaces
- Logs and metrics
