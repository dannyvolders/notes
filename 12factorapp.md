# The Twelve-Factor App

**What**: a set of principles and best practices for building modern, scalable, and maintainable software-as-a-service (SaaS) applications.

**Audience**: Developer that build applications which run as a service. Ops engineers that manage such applications.

## References
* https://12factor.net/
* https://learn.microsoft.com/en-us/dotnet/architecture/cloud-native/definition#the-twelve-factor-application
* https://www.redhat.com/architect/12-factor-app
* https://blog.sap-press.com/twelve-factor-app-principles-for-developers
* https://www.dreamfactory.com/resources/whitepapers/implementing-the-twelve-factor-app-methodology/

## Mindmap


```mermaid
mindmap
  root(Twelve factor app))
    {{1 - Codebase}}
      (1 codebase per microservice)
      (common libraries in different codebase)
      (version control)
      (same for all environments)
    {{2 - Dependencies}}
      (track your own dependencies, don't share dependencies)
    {{3 - Config}}
      (configs belongs in the environment)
    {{4 - Backing services}}
      (a backing service is a resource)
      (don't distinct local and third party services)
      (resources can be interchangeable)
    {{5 - Build, release, run}}
      (keep track of build, release and run versions)
      (enable rollbacks)
    {{6 - Processes}}
      (apps are stateless)
      (apps should support up to n instances)
      (if any, share state in a distributed cache or shared database)
      (avoid sticky sessions)
    {{7 - Port binding}}
      (isolate apps by using distinct ports)
    {{8 - Concurrency}}
      (scale horizontally = by adding instances)
      (design for concurrency)
    {{9 - Disposability}}
      (fast startup)
      (graceful shutdowns)
    {{10 - Dev/prod parity}}
      (dev env must match produdction env)
    {{11 - Logs}}
      (logs as event streams)
      (collect logs centrally)
    {{12 - Admin processes}}
      (do maintenance)
      (separate from application)
      (must come as a deliverable)


```