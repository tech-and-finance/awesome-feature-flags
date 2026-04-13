# Awesome Feature Flags [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of feature flag and feature toggle tools, services, SDKs, and resources for progressive delivery.

Feature flags (also called feature toggles) decouple deployment from release. They let you ship code to production and control who sees it — enabling gradual rollouts, kill switches, A/B testing, and instant rollback without redeployment.

## Contents

- [Platforms](#platforms)
  - [Managed Services (SaaS)](#managed-services-saas)
  - [Open Source (Self-Hosted)](#open-source-self-hosted)
  - [Vendor-Neutral Standards](#vendor-neutral-standards)
- [Language-Specific Libraries](#language-specific-libraries)
  - [JavaScript / TypeScript](#javascript--typescript)
  - [Go](#go)
  - [Python](#python)
  - [Java / JVM](#java--jvm)
  - [.NET / C#](#net--c)
  - [Ruby](#ruby)
  - [PHP](#php)
  - [Rust](#rust)
  - [Elixir](#elixir)
  - [Swift / iOS](#swift--ios)
  - [Kotlin / Android](#kotlin--android)
  - [Flutter / Dart](#flutter--dart)
- [Kubernetes & Infrastructure](#kubernetes--infrastructure)
- [Articles & Guides](#articles--guides)
  - [Introductions](#introductions)
  - [Architecture & Patterns](#architecture--patterns)
  - [Best Practices](#best-practices)
  - [Case Studies](#case-studies)
- [Books](#books)
- [Videos & Talks](#videos--talks)
- [Community](#community)

## Platforms

### Managed Services (SaaS)

- [LaunchDarkly](https://launchdarkly.com) - Market-leading feature management platform with 25+ SDKs, experimentation, and enterprise governance. MAU-based pricing.
- [Split](https://www.split.io) - Feature delivery platform with data-driven insights and experimentation analytics.
- [Statsig](https://statsig.com) - All-in-one platform for feature flags, A/B testing, and product analytics. Free up to 1M events/month.
- [Harness Feature Flags](https://harness.io/products/feature-flags) - Part of the Harness CI/CD platform with built-in pipeline integration.
- [ConfigCat](https://configcat.com) - Developer-friendly feature flag service with a simple UI and cross-platform SDKs. Free tier with 10 flags.
- [Rollgate](https://rollgate.io) - Feature flag platform with scheduled releases, instant rollback, and 13 SDKs. Free tier with 500K requests/month.
- [DevCycle](https://devcycle.com) - Feature management platform built for developers with OpenFeature support and edge computing.
- [Bucket](https://bucket.co) - Purpose-built feature flagging for B2B SaaS products.
- [Hypertune](https://hypertune.com) - Type-safe feature flags with Git-style version control, optimized for React and Next.js.
- [Tggl](https://tggl.io) - Feature flag management with release orchestration for teams shipping fast.
- [Apptimize](https://apptimize.com) - Mobile-focused A/B testing and feature management platform.
- [Molasses](https://www.molasses.app) - Feature flags and A/B testing tools for shipping code with fewer incidents.
- [Prefab](https://prefab.cloud) - Feature flags, dynamic log levels, and remote config as a service.
- [Flagship](https://flagship.io) - Feature management and experimentation platform for web and mobile.

### Open Source (Self-Hosted)

- [Unleash](https://github.com/Unleash/unleash) - Open-source feature management platform with enterprise-grade SDKs and a polished UI. Node.js backend with PostgreSQL.
- [Flagsmith](https://github.com/Flagsmith/flagsmith) - Open-source feature flag and remote config service with an API-first design. Django backend.
- [GrowthBook](https://github.com/growthbook/growthbook) - Open-source platform for feature flags and A/B testing with Bayesian statistical analysis. Connects to your data warehouse.
- [Flipt](https://github.com/flipt-io/flipt) - Self-hosted feature flag application with a clean UI and gRPC API. Single Go binary, no external dependencies.
- [FeatBit](https://github.com/featbit/featbit) - Open-source feature flag management service built with .NET. Supports 100% self-hosting.
- [GO Feature Flag](https://github.com/thomaspoignant/go-feature-flag) - Lightweight Go module for feature flagging using file-based configuration (YAML, JSON, TOML). No server needed.
- [Flagr](https://github.com/openflagr/flagr) - Open-source feature flagging and A/B testing service with a Go backend and React UI.
- [PostHog](https://github.com/PostHog/posthog) - Open-source product analytics suite that includes feature flags, session recording, and experimentation.
- [OpenFeature flagd](https://github.com/open-feature/flagd) - A lightweight, OpenFeature-compliant feature flag daemon for cloud-native applications.

### Vendor-Neutral Standards

- [OpenFeature](https://openfeature.dev) - CNCF sandbox project providing a vendor-agnostic, community-driven specification and SDKs for feature flag management. Allows switching providers without code changes.

## Language-Specific Libraries

Libraries and SDKs for implementing feature flags in specific languages without depending on a managed service.

### JavaScript / TypeScript

- [Unleash Client for Node.js](https://github.com/Unleash/unleash-client-node) - Official Unleash Node.js SDK with local evaluation and streaming support.
- [react-feature-flags](https://github.com/romaindso/react-feature-flags) - Simple React component for feature toggling using context.
- [fflip](https://github.com/FredKSchott/fflip) - Lightweight feature flagging for Node.js with Express integration.
- [feature-toggle-api](https://github.com/pqx/feature-toggle-api) - Minimal feature toggle library for JavaScript apps.

### Go

- [flipt-server-sdks](https://github.com/flipt-io/flipt-server-sdks) - Server-side SDKs for Flipt feature flag evaluation.
- [ff4g](https://github.com/pjebs/ff4g) - Minimalist feature flags for Go.
- [toggle](https://github.com/xchapter7x/toggle) - Simple feature toggles for Go using JSON config.

### Python

- [flask-featureflags](https://github.com/trustrachel/Flask-FeatureFlags) - Feature flag support for Flask applications.
- [django-waffle](https://github.com/django-waffle/django-waffle) - Feature flipper for Django with database-backed switches, flags, and samples.
- [feature-flags](https://github.com/trustrachel/feature-flags) - Generic Python feature flag library with pluggable backends.

### Java / JVM

- [FF4J](https://github.com/ff4j/ff4j) - Feature flags for Java with a web console, Spring Boot integration, audit trail, and multiple backends (Redis, MongoDB, JDBC).
- [Togglz](https://www.togglz.org) - Feature flags for Java with a management console, Spring Boot support, and JUnit integration.
- [unleash-client-java](https://github.com/Unleash/unleash-client-java) - Official Unleash Java SDK.
- [OpenFeature Java SDK](https://github.com/open-feature/java-sdk) - Vendor-neutral Java SDK for feature flag evaluation.

### .NET / C#

- [Microsoft.FeatureManagement](https://github.com/microsoft/FeatureManagement-Dotnet) - Official Microsoft library for feature flags in .NET with ASP.NET Core integration, filters, and feature gates.
- [OpenFeature .NET SDK](https://github.com/open-feature/dotnet-sdk) - Vendor-neutral .NET SDK for feature flag evaluation.
- [FeatureToggle](https://github.com/jason-roberts/FeatureToggle) - Simple, low-ceremony feature toggle library for .NET.

### Ruby

- [Flipper](https://github.com/flippercloud/flipper) - Feature flags for Ruby with adapters for ActiveRecord, Redis, Mongo, and more. Free cloud service available.
- [rollout](https://github.com/fetlife/rollout) - Fast feature flags based on Redis with percentage rollouts and user targeting.

### PHP

- [Flagception](https://github.com/bestit/flagception-sdk) - Feature flag SDK for PHP with decorator pattern and Symfony bundle.
- [Laravel Pennant](https://github.com/laravel/pennant) - First-party feature flag package for Laravel with database and in-memory drivers.

### Rust

- [feature-flags](https://github.com/auxoncorp/feature-flags) - Compile-time and runtime feature flags for Rust.

### Elixir

- [fun_with_flags](https://github.com/tompave/fun_with_flags) - Feature flags for Elixir/Erlang with Redis or Ecto backends, PubSub cache busting, and an admin UI.

### Swift / iOS

- [Vexil](https://github.com/unsignedapps/Vexil) - Feature flags for Swift with property wrappers, multiple backends, and Combine/async-await support.

### Kotlin / Android

- [Laboratory](https://github.com/nicholasgasior/laboratory) - Feature flags for Kotlin Multiplatform (Android, JVM, iOS).

### Flutter / Dart

- [feature_flags](https://pub.dev/packages/feature_flags) - Simple feature flag implementation for Flutter apps.

## Kubernetes & Infrastructure

Tools for progressive delivery and feature flagging at the infrastructure level.

- [Argo Rollouts](https://github.com/argoproj/argo-rollouts) - Progressive delivery controller for Kubernetes with canary deployments, blue-green, and experimentation.
- [Flagger](https://github.com/fluxcd/flagger) - Progressive delivery operator for Kubernetes (canary, A/B testing, blue-green) powered by Istio, Linkerd, or Envoy.
- [Iter8](https://github.com/iter8-tools/iter8) - Kubernetes-native tool for A/B testing, canary releases, and performance benchmarking.
- [Kargo](https://github.com/akuity/kargo) - GitOps-native progressive delivery for Kubernetes environments.

## Articles & Guides

### Introductions

- [Feature Toggles (Feature Flags)](https://martinfowler.com/articles/feature-toggles.html) - Martin Fowler's definitive article on feature flag categories and lifecycle management.
- [What Are Feature Flags?](https://www.atlassian.com/continuous-delivery/principles/feature-flags) - Atlassian's overview of feature flags in continuous delivery.
- [Feature Flags: The Complete Guide](https://featureflags.io) - Comprehensive resource covering feature flag types, use cases, and best practices.

### Architecture & Patterns

- [Feature Flag Best Practices](https://launchdarkly.com/blog/feature-flag-best-practices/) - LaunchDarkly's guide to naming conventions, lifecycle management, and flag debt.
- [Testing in Production with Feature Flags](https://copyconstruct.medium.com/testing-in-production-the-safe-way-18ca102d0ef1) - Cindy Sridharan on using feature flags for safe production testing.
- [Progressive Delivery](https://www.split.io/glossary/progressive-delivery/) - Definition and patterns for progressive delivery including canary releases and feature flags.
- [Feature Flags & Technical Debt](https://www.thoughtworks.com/insights/articles/managing-feature-flag-tech-debt) - ThoughtWorks on managing the lifecycle and cleanup of feature flags.

### Best Practices

- [Gradual Rollout Strategies](https://docs.getunleash.io/topics/feature-flags/gradual-rollout) - Unleash's guide to percentage-based rollouts with consistent hashing.
- [Feature Flag Driven Development](https://featureflags.io/feature-flag-driven-development/) - Using feature flags as a development methodology, not just an ops tool.
- [Kill Switches in Production](https://blog.harness.io/feature-flag-kill-switch/) - How to implement and use kill switches for instant feature disabling.

### Case Studies

- [Feature Flags at GitHub](https://github.blog/engineering/infrastructure/ship-code-faster-safely-feature-flags-at-github/) - How GitHub uses feature flags to ship code safely to millions of developers.
- [How Facebook Uses Feature Flags](https://engineering.fb.com/2024/06/14/developer-tools/gatekeeper-feature-flags-meta/) - Meta's Gatekeeper system for managing feature rollouts at massive scale.
- [Feature Flags at Netflix](https://netflixtechblog.com/feature-flagging-at-netflix-b29e46b2e821) - Netflix's approach to feature flag-driven experimentation.

## Books

- [Feature Flag Best Practices](https://launchdarkly.com/the-definitive-guide-to-feature-management/) - LaunchDarkly's free ebook on feature management strategy and implementation.
- [Accelerate](https://itrevolution.com/product/accelerate/) - Nicole Forsgren et al. — includes research on how continuous delivery practices (including feature flags) correlate with organizational performance.
- [Continuous Delivery](https://continuousdelivery.com) - Jez Humble & David Farley — foundational book on continuous delivery that covers feature toggles as a deployment pattern.

## Videos & Talks

- [Feature Flags: Do's and Don'ts](https://www.youtube.com/watch?v=BXbNsneqKHo) - Pete Hodgson at QCon on practical feature flag patterns and anti-patterns.
- [Progressive Delivery with Feature Flags](https://www.youtube.com/watch?v=EkfqgQXfEv8) - James Governor (RedMonk) on the evolution from continuous delivery to progressive delivery.
- [Feature Flags and the Science of Shipping](https://www.youtube.com/watch?v=sSQT8IEw3k4) - Edith Harbaugh (LaunchDarkly CEO) on the business case for feature management.

## Community

- [OpenFeature Community](https://openfeature.dev/community/) - CNCF sandbox project community with Slack, GitHub discussions, and monthly meetings.
- [Feature Flag Subreddit](https://www.reddit.com/r/featureflags/) - Reddit community for discussing feature flag tools and practices.

## Contributing

Contributions welcome! Read the [contributing guidelines](contributing.md) first.
