# Agentic Codebase System, unleashed by an AI-First framework - April 4, 2025

This system reinvents programming as a conversational process where API-first architecture is wired into its DNA. Every AI-generated procedure automatically registers itself through the central API Gateway with complete OpenAPI specifications, making the entire system self-routing by design. Instead of manual editing or traditional merging, each change request initiates new containerized branches where specialized AI agents rebuild services from scratch—preconfigured to expose themselves through the gateway with perfect documentation from birth. This gateway-centric approach, combined with our optimized technology stack (carefully selected for deterministic AI generation), creates a development ecosystem where thousands of parallel implementations can evolve independently while remaining instantly consumable.

The magic lies in how every AI-created branch becomes a fully autonomous service node: automatically documented via OpenAPI, self-registering with the gateway, and instantly available for testing—all without merge operations. When you request changes ("Add JWT validation to these endpoints"), AI agents don't modify code—they spawn perfectly documented new versions that plug into the existing routing mesh. Our strictly enforced architectural patterns (type-safe API contracts, gateway-compatible frameworks) ensure each iteration maintains flawless interoperability, whether it's a minor tweak or complete rewrite. The result collapses the traditional development pipeline into pure conversation, where every prompt yields production-ready services that integrate themselves.

```
                                                 ┌───────────────────┐
                                                 │                   │
                                                 │    Developer      │
                                                 │                   │
                                                 └─────────┬─────────┘
                                                           │
                                                           │ Natural Language Prompts
                                                           ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                     Dev Processor                                               │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         │ Manages Dev Flow
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                       AI Agent                                                  │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         │ Code Modifications
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                    Code Generator                                               │
│                           (Runs in Isolated Container)                                          │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         │ TypeScript Functions
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                     Git Handler                                                 │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         │ Branch Creation
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                Command Executor                                                 │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         │ Triggers Build Process (Hidden from AI Agent)
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                 Build System                                                    │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         │ Transpiles Code & Adds RPC Features
                                         │ Generates API Routes Automatically
                                         │ Creates OpenAPI Specifications
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                              Container Orchestrator                                             │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         │ Container Management
                                         ▼
                                ┌────────────────────────┐
                                │                        │
                                │  Multiple API Gateway  │
                                │      Instances         │
                                │                        │
                                └───────────┬────────────┘
                                            │
                                            │ Request Routing
                                            ▼
┌───────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                               │
│                                  Codebase Containers                                          │
│                                                                                               │
└───────────────────────────────────────────────────────────────────────────────────────────────┘
```

## Automated Build Process (Hidden from AI Agent)

Transpiles pure TypeScript to add tRPC routes and OpenAPI 3.0 specs.
AI agent writes business logic only; build system handles API exposure.

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                 Source Code                                                     │
│                        (Pure TypeScript Functions from AI)                                      │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                 Build System                                                    │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
                           ┌───────────────────────────┐
                           │                           │
                           │  Automated Processes      │
                           │                           │
                           └─────────┬─────────────────┘
                                     │
                                     ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ tRPC Route         │      │ OpenAPI Spec       │      │ Service Manager    │
│ Generation         │      │ Generation         │      │ Configuration      │
│                    │      │                    │      │ (PM2)              │
└────────────────────┘      └────────────────────┘      └────────────────────┘
```


## Service Management (Hidden from AI Agent)

PM2 runs inside each container independently from the parent system.
Manages independent processes for each branch with zero-downtime deployment.
Each branch runs completely independently and can be switched anytime.

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                        PM2 Service Manager (Inside Each Container)                              │
│                                 (Independent from Parent)                                       │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
                           ┌───────────────────────────┐
                           │                           │
                           │  Independent Processes    │
                           │                           │
                           └─────────┬─────────────────┘
                                     │
                                     ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ Codebase 1         │      │ Codebase 1         │      │ Codebase 1         │
│ Branch 00001       │      │ Branch 00002       │      │ Branch 00003       │
│ Process            │      │ Process            │      │ Process            │
└────────────────────┘      └────────────────────┘      └────────────────────┘

┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ Codebase 2         │      │ Codebase 2         │      │ Codebase 3         │
│ Branch 00001       │      │ Branch 00002       │      │ Branch 00001       │
│ Process            │      │ Process            │      │ Process            │
└────────────────────┘      └────────────────────┘      └────────────────────┘
```

## Domain Routing (Hidden from AI Agent)

Auto-HTTPS reverse proxy routes domains to appropriate gateway instances.
Enables seamless production, staging, and development environments.
Uses network isolation instead of separate dev domains to fully replicate production.
Same domains are used for both dev and production, lowering friction significantly.

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                 Domain Reverse Proxy                                            │
│                                    (Auto-HTTPS)                                                 │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
                           ┌───────────────────────────┐
                           │                           │
                           │  Domain Routing           │
                           │                           │
                           └─────────┬─────────────────┘
                                     │
                                     ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ api.example.com    │      │ api.example.com    │      │ api.example.com    │
│ (Production)       │      │ (Staging)          │      │ (Development)      │
│ ↓                  │      │ ↓                  │      │ ↓                  │
│ Production Gateway │      │ Staging Gateway    │      │ Development Gateway│
│                    │      │ (Network Isolated) │      │ (Network Isolated)│
└────────────────────┘      └────────────────────┘      └────────────────────┘
```

## Detailed Multi-Environment API Gateway

Supports unlimited gateway modes with automatic OpenAPI 3.0 documentation.
Fully customizable routing with branch selection per codebase.
Provides automatic HTTPS and self-made subdomains based on mono-repo name and env name.
Always uses HTTPS to ensure built-in security and avoid browser/development issues.
Secured with firewall and with those authentication mechanisms, it covers virtually all use cases:
- IP whitelist/blacklist for access control - this is for production
- Hidden domains for security by obfuscation - this is for dev
- Standard username:password credentials (universal & transparent) - this is for sensitive endpoints that risks exposure

```
                                    ┌─────────────────┐
                                    │                 │
                                    │  API Consumers  │
                                    │                 │
                                    └────────┬────────┘
                                             │
                                             ▼
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│                    Multiple API Gateway Instances                   │
│                     (Unlimited Gateway Modes)                       │
│                     (Automatic HTTPS & Subdomains)                  │
│                     (Secured & Firewalled)                          │
├─────────────────┬─────────────────┬─────────────────────────────────┤
│                 │                 │                                 │
│  Production     │  Staging        │  Development                    │
│  Gateway        │  Gateway        │  Gateway                        │
│  (active)       │  (testing)      │  (latest)                       │
│                 │                 │                                 │
└────────┬────────┴────────┬────────┴────────────┬────────────────────┘
          │                 │                     │
          ▼                 ▼                     ▼
┌────────────────┐ ┌────────────────┐ ┌────────────────────────────────┐
│                │ │                │ │                                │
│ Codebase 1     │ │ Codebase 1     │ │ Codebase 1                     │
│ Server         │ │ Server         │ │ Server                         │
│ (active branch)│ │ (test branch)  │ │ (latest branch)                │
│                │ │                │ │                                │
└────────────────┘ └────────────────┘ └────────────────────────────────┘
┌────────────────┐ ┌────────────────┐ ┌────────────────────────────────┐
│                │ │                │ │                                │
│ Codebase 2     │ │ Codebase 2     │ │ Codebase 2                     │
│ Server         │ │ Server         │ │ Server                         │
│ (active branch)│ │ (test branch)  │ │ (latest branch)                │
│                │ │                │ │                                │
└────────────────┘ └────────────────┘ └────────────────────────────────┘
┌────────────────┐ ┌────────────────┐ ┌────────────────────────────────┐
│                │ │                │ │                                │
│ Codebase 3     │ │ Codebase 3     │ │ Codebase 3                     │
│ Server         │ │ Server         │ │ Server                         │
│ (active branch)│ │ (test branch)  │ │ (latest branch)                │
│                │ │                │ │                                │
└────────────────┘ └────────────────┘ └────────────────────────────────┘
```

## Data Model Relationships

Tracks relationships between codebases, branches, commits, and dev revisions.
Links natural language prompts to code changes with complete history.

```
┌───────────────┐     ┌───────────────┐     ┌───────────────┐
│               │     │               │     │               │
│   Codebase    │◄────┤     Branch    │◄────┤    Commit     │
│               │     │               │     │               │
└───────┬───────┘     └───────┬───────┘     └───────────────┘
        │                     │
        │                     │
        │                     │
┌───────▼───────┐     ┌───────▼───────┐     ┌───────────────┐
│               │     │               │     │               │
│ Dev Revision  │◄────┤    Change     │◄────┤    Response   │
│               │     │               │     │               │
└───────┬───────┘     └───────────────┘     └───────┬───────┘
        │                                           │
        │                                           │
        ▼                                           │
┌───────────────┐                                   │
│               │                                   │
│    Prompt     │◄──────────────────────────────────┘
│               │
└───────────────┘
```

## Type-Safe ORM Integration

Enforces schema validation between TypeScript functions and database.
Prevents type errors and ensures data integrity across the system.
Uses Postgres as the main database with Drizzle or Prisma as ORM options.
End-to-end typing is mandatory to ensure compatibility across branches.

```
┌───────────────────┐     ┌───────────────────┐     ┌───────────────────┐
│                   │     │                   │     │                   │
│  TypeScript      │────►│  ORM Schema       │────►│  Database         │
│  Function        │     │  Validation       │     │  (Postgres)       │
│                   │     │                   │     │                   │
└───────────────────┘     └───────────────────┘     └───────────────────┘
        ▲                         │                         ▲
        │                         │                         │
        │                         ▼                         │
        │                 ┌───────────────────┐             │
        │                 │                   │             │
        │                 │  Runtime Type     │             │
        │                 │  Validation (Zod) │             │
        │                 │                   │             │
        │                 └───────────────────┘             │
        │                                                   │
┌───────┴───────────┐                              ┌────────┴──────────┐
│                   │                              │                   │
│  AI-Generated     │                              │  Type-Safe        │
│  Code             │                              │  Queries          │
│                   │                              │                   │
└───────────────────┘                              └───────────────────┘
```

## Database Configuration and Management

Each branch has its own database config file that points to shared schema definitions.
Database schemas are centrally managed but can be referenced by any branch.
Compatibility testing ensures type safety across the entire system.

```
┌───────────────────┐     ┌───────────────────┐     ┌───────────────────┐
│                   │     │                   │     │                   │
│  Branch-Specific  │────►│  Shared Schema    │────►│  Database         │
│  DB Config        │     │  Definitions      │     │  Instance         │
│                   │     │                   │     │                   │
└───────────────────┘     └───────────────────┘     └───────────────────┘
        │                         ▲                         ▲
        │                         │                         │
        ▼                         │                         │
┌───────────────────┐     ┌───────────────────┐     ┌───────────────────┐
│                   │     │                   │     │                   │
│  Environment      │     │  Schema           │     │  Connection       │
│  Overrides        │     │  Compatibility    │     │  Management       │
│                   │     │  Testing          │     │                   │
└───────────────────┘     └───────────────────┘     └───────────────────┘
```

## Schema Management Workflow

Schema changes are isolated to branches until validated across the system.
Prevents breaking changes from affecting production environments.
Reduces AI agent hallucination by limiting context to relevant schemas.
**Absolutely prevents deployment of broken versions through strict compatibility enforcement.**

```
┌───────────────────┐     ┌───────────────────┐     ┌───────────────────┐
│                   │     │                   │     │                   │
│  Branch Working   │────►│  Compatibility    │────►│  Shared Schema    │
│  Schema Copy      │     │  Testing          │     │  Repository       │
│                   │     │                   │     │                   │
└───────────────────┘     └───────────────────┘     └───────────────────┘
        ▲                         │                         │
        │                         │                         │
        │                         ▼                         ▼
┌───────────────────┐     ┌───────────────────┐     ┌───────────────────┐
│                   │     │                   │     │                   │
│  AI-Generated     │     │  Validation       │     │  Production       │
│  Schema Changes   │     │  Results          │     │  Deployment       │
│                   │     │                   │     │  (Only if valid)  │
└───────────────────┘     └───────────────────┘     └───────────────────┘
```

### Cross-Branch Schema Compatibility Testing

When a branch proposes schema changes, the system automatically:

1. Identifies all active branches that use the same database
2. Runs end-to-end type checking against each branch's codebase
3. Verifies that existing data can be migrated without loss
4. Generates a compatibility report showing potential issues
5. Blocks deployment if any compatibility tests fail

This ensures that no schema change can break existing functionality in any branch.

### Schema Change Propagation

```
┌───────────────────┐     ┌───────────────────┐     ┌───────────────────┐
│                   │     │                   │     │                   │
│  Branch Proposes  │────►│  Cross-Branch     │────►│  Schema Change    │
│  Schema Change    │     │  Validation       │     │  Approval/Denial  │
│                   │     │                   │     │                   │
└───────────────────┘     └───────────────────┘     └───────────────────┘
                                                             │
                                                             │
                                                             ▼
┌───────────────────┐     ┌───────────────────┐     ┌───────────────────┐
│                   │     │                   │     │                   │
│  Notification to  │◄────┤  Update Shared    │◄────┤  If Approved:     │
│  Affected Branches│     │  Schema Repository│     │  Apply Changes    │
│                   │     │                   │     │                   │
└───────────────────┘     └───────────────────┘     └───────────────────┘
```

Schema changes follow a strict propagation workflow that ensures all branches remain compatible:

1. Changes are first made in the branch's working copy
2. Comprehensive validation occurs across all affected branches
3. If validation passes, changes are applied to the shared schema repository
4. All branches are notified of the schema update
5. Each branch can update its working copy from the shared repository

This approach guarantees that the system can never deploy a broken version, as compatibility is verified before any changes are applied to the shared schema.

## tRPC Function-to-API Mechanism

Automatically exposes TypeScript functions as HTTP endpoints with type safety.
Generates OpenAPI 3.0 specs that can be fully customized per endpoint.

```
┌───────────────┐     ┌───────────────┐     ┌───────────────┐     ┌───────────────┐
│               │     │               │     │               │     │               │
│  TypeScript   │────►│  tRPC Router  │────►│  HTTP Server  │────►│  API Gateway  │
│   Function    │     │  (Generated)  │     │               │     │               │
│               │     │               │     │               │     │               │
└───────────────┘     └───────────────┘     └───────────────┘     └───────────────┘
       ▲                                                                  ▲
       │                                                                  │
       │                                                                  │
       │                                                                  │
┌──────┴────────┐                                              ┌──────────┴─────┐
│               │                                              │                │
│  AI-Generated │                                              │  API Consumer  │
│     Code      │                                              │                │
│               │                                              │                │
└───────────────┘                                              └────────────────┘
```

## Context Management System

Provides hierarchical context access at global, repo, and branch levels.
Enables AI to generate context-aware code without exposing entire system.

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                 Context Management                                              │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
                           ┌───────────────────────────┐
                           │                           │
                           │  Context Hierarchy        │
                           │                           │
                           └─────────┬─────────────────┘
                                     │
                                     ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ Global Shared      │      │ Mono-Repo          │      │ Branch-Specific    │
│ Context            │      │ Context            │      │ Context            │
│                    │      │                    │      │                    │
└────────────┬───────┘      └────────────┬───────┘      └────────────┬───────┘
             │                           │                           │
             ▼                           ▼                           ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ Shared Types       │      │ Repo-Specific      │      │ Branch-Specific    │
│ Shared Constants   │      │ Configuration      │      │ Environment Vars   │
│ Shared Libraries   │      │ Domain Knowledge   │      │ Model Adjustments  │
│ Helper Materials   │      │ Helper Snippets    │      │ Feature Flags      │
└────────────────────┘      └────────────────────┘      └────────────────────┘
```

## Repository Structure with Context

Organizes shared types, domain knowledge, and configuration at appropriate levels.
Isolates context to prevent information leakage between codebases.

```
main-repository/
├── shared-context/                      # Global shared context - not mandatory but always created regardless
│   ├── types/                           # Shared types across all repos
│   ├── constants/                       # Shared constants
│   ├── libraries/                       # Shared utility libraries
│   └── helpers/                         # Screenshots, snippets to help LLM
│
├── servers/                             # Server configuration
│   └── config.json                      # Server configuration with SSH credentials (containers & gateway) - automatic VM created for this mono-repo (should have total isolation at all times)
│
├── ai/                                  # AI configuration
│   └── config.json                      # Openrouter API key and budget settings for this mono-repo
│
├── gateways/                            # Gateway configuration
│   ├── production.json                  # Production gateway settings
│   ├── staging.json                     # Staging gateway settings
│   └── development.json                 # Development gateway settings
│
├── databases/                           # Centralized database definitions
│   ├── db-001/                          # Database instance by ID
│   │   ├── config.json                  # Database configuration with Postgres URL, login, password
│   │   ├── schema/                      # Schema definitions
│   │   ├── migrations/                  # Migration files
│   │   └── seeds/                       # Seed data
│   └── db-002/                          # Another database instance
│       ├── config.json                  # Database configuration with Postgres URL, login, password
│       ├── schema/
│       ├── migrations/
│       └── seeds/
│
├── codebases/
│   ├── user-management/    # This can be broad or narrow
│   │   ├── active-branch # Decide which branch is "active" - this is just to help the default Gateway, it's entirely adjustable individually per Gateway as well, but this is very practical as a plug and play active, could be used for prod
│   │   ├── context/                     # Mono-repo specific context - not mandatory to add - but structure is created always
│   │   │   ├── any-md-001.md            # Automatically added as context - not mandatory
│   │   │   ├── any-md-002.md            # Automatically added as context - not mandatory
│   │   │   └── helpers/                 # Additional materials to help LLM - not mandatory
│   │   │       ├── links/               # URLs for documentation or such
│   │   │       ├── snippets/            # Code snippets for reference - Some models thrive with examples
│   │   │       └── screenshots/         # UI/UX references and examples
│   │   │
│   │   ├── metadata/
│   │   │   ├── branches/
│   │   │   │   ├── 00001/
│   │   │   │   │   ├── branch.info.json
│   │   │   │   │   ├── changes.json
│   │   │   │   │   ├── diff.patch
│   │   │   │   │   ├── summary.md
│   │   │   │   │   ├── readme.md
│   │   │   │   │   ├── db-config.ts     # Branch-specific database config 
│   │   │   │   │   ├── schema/          # Reference copy of database schemas, but DBs are always shared
│   │   │   │   │   │   ├── models/      # Schema definitions
│   │   │   │   │   │   └── migrations/  # Migration files
│   │   │   │   │   ├── logs/            # Reference to logs stored in separate repo for scalability
│   │   │   │   │   │   ├── pm2/         # PM2 Process Manager Logs reference - splitted by max token size
│   │   │   │   │   │   ├── ttyd/        # Terminal Session Logs reference - splitted by max token size
│   │   │   │   │   │   └── api-gateway/ # API Gateway Logs reference - splitted by max token size
│   │   │   │   │   └── context/         # Branch-specific context
│   │   │   │   │       ├── env.json     # Environment variables & model adjustments
│   │   │   │   │       ├── flags.json   # Feature flags
│   │   │   │   │       └── helpers/     # Branch-specific helper materials
│   │   │   │   │           ├── snippets/  # Code examples for this branch
│   │   │   │   │           └── images/    # Visual references for LLM
│   │   │   │   └── 00002/ # Always based on previous automatically.
│   │   │   │       ├── branch.info.json
│   │   │   │       ├── changes.json
│   │   │   │       ├── diff.patch
│   │   │   │       ├── summary.md       # Mass mapping of the codebase in a lightweight fashion
│   │   │   │       ├── readme.md        # Keep track of the entire codebase role - precisely
│   │   │   │       ├── db-config.ts     # Branch-specific database config
│   │   │   │       ├── schema/          # Reference copy of database schema
│   │   │   │       ├── logs/            # Reference to logs stored in separate repo
│   │   │   │       └── context/         # Branch-specific context
│   │   │   │
│   │   │
│   │
│   ├── ...


```

## Default Codebase Branch Structure

Standardized TypeScript boilerplate with highly modular organization.
Directories are structured to maintain low context size.
ORM integration is type-safe and connects to the shared database schemas via a real-copy to avoid any breakage.
Feature-based structure with clear layers within each feature.

```
src/
├── features/                # Feature-based organization - this is just a sample
│   ├── auth/                # Authentication feature
│   │   ├── models/          # Domain models
│   │   ├── services/        # Business logic
│   │   ├── controllers/     # API endpoints
│   │   ├── validators/      # Zod schemas for validation
│   │   └── queries/         # Typed query builders
│   ├── users/               # User management feature
│   │   ├── models/
│   │   ├── services/
│   │   ├── controllers/
│   │   ├── validators/
│   │   └── queries/
│   └── [other example features]/
├── schema/                  # Working copy of database schema
│   ├── models/              # Schema definitions
│   ├── migrations/          # Migration files
│   └── seeds/               # Seed data
├── shared/                  # Shared utilities and components
│   ├── types/               # Shared type definitions
│   ├── utils/               # Utility functions
│   ├── middleware/          # Shared middleware
│   └── errors/              # Error handling
├── docs/                    # Documentation
│   ├── api/                 # API documentation
│   ├── schema/              # Schema documentation
│   └── guides/              # Usage guides
├── config/                  # Application configuration
│   ├── env.ts               # Environment configuration
│   ├── db-config.ts         # Database configuration (points to shared schema)
│   └── server.ts            # Server configuration
└── app.ts                   # Application entry point
```

## AI Agent Context Access

AI accesses only relevant context for current task to reduce complexity and cost.
Maintains isolation while providing necessary domain knowledge.

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                       AI Agent                                                  │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
                           ┌───────────────────────────┐
                           │                           │
                           │  Context Access           │
                           │                           │
                           └─────────┬─────────────────┘
                                     │
                                     ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ Global Shared      │      │ Current Repo       │      │ Current Branch     │
│ Context            │      │ Context            │      │ Context            │
│                    │      │                    │      │                    │
└────────────────────┘      └────────────────────┘      └────────────────────┘

                                         │
                                         │ Context-Aware Code Generation
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                    Code Generator                                               │
│                                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────────────────────┘
```

## Constrained Environment & Type Safety

Enforces strict resource limits and type safety to prevent errors and cost overruns.
Provides guardrails for AI code generation with budget awareness.

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                              Constrained Execution Environment                                  │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
                           ┌───────────────────────────┐
                           │                           │
                           │  Cost & Resource Limits   │
                           │                           │
                           └─────────┬─────────────────┘
                                     │
                                     ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ Budget Enforcement │      │ Execution Timeouts │      │ Memory Limits      │
│                    │      │                    │      │                    │
└────────────────────┘      └────────────────────┘      └────────────────────┘


┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                 Strong Type Safety System                                       │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
                           ┌───────────────────────────┐
                           │                           │
                           │  Type Enforcement Layers  │
                           │                           │
                           └─────────┬─────────────────┘
                                     │
                                     ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ TypeScript         │      │ ORM with Enforced  │      │ Runtime Type       │
│ Static Typing      │      │ Schema Validation  │      │ Checking           │
│                    │      │                    │      │                    │
└────────────────────┘      └────────────────────┘      └────────────────────┘
```

## Code Generator Capabilities

Self-debugging container with automatic follow-up question generation.
Operates within strict budget limits with ORM and type validation.

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                 │
│                                    Code Generator                                               │
│                           (Runs in Isolated Container)                                          │
│                                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────────────────────┘
                                         │
                                         ▼
                           ┌───────────────────────────┐
                           │                           │
                           │  Automated Capabilities   │
                           │                           │
                           └─────────┬─────────────────┘
                                     │
                                     ▼
┌────────────────────┐      ┌────────────────────┐      ┌────────────────────┐
│                    │      │                    │      │                    │
│ Self-Debugging     │      │ Budget-Aware       │      │ Automatic          │
│ Up to Budget Limit │      │ Processing         │      │ Follow-up Questions│
│                    │      │                    │      │                    │
└────────────────────┘      └────────────────────┘      └────────────────────┘
```


## AI Conversation Integration

Stores developer prompts and AI responses with links to code changes.
Enables traceability from natural language to implemented features.
Each revision may include multiple prompts and responses until validation.

```
┌───────────────┐     ┌───────────────┐     ┌───────────────┐     ┌───────────────┐
│               │     │               │     │               │     │               │
│  Developer    │────►│  Dev Prompt   │────►│   AI Agent    │────►│   Response    │
│               │     │               │     │               │     │               │
└───────────────┘     └───────┬───────┘     └───────────────┘     └───────┬───────┘
                              │                                           │
                              ▼                                           ▼
                      ┌───────────────┐                           ┌───────────────┐
                      │               │                           │               │
                      │  Stored in    │                           │  Stored in    │
                      │  prompt.md    │                           │  response.md  │
                      │               │                           │               │
                      └───────────────┘                           └───────┬───────┘
                                                                          │
                                                                          │
                                                                          ▼
                                                                  ┌───────────────┐
                                                                  │               │
                                                                  │ Code Changes  │
                                                                  │               │
                                                                  └───────┬───────┘
                                                                          │
                                                                          │
                                                                          ▼
┌───────────────┐     ┌───────────────┐     ┌───────────────┐     ┌───────────────┐
│               │     │               │     │               │     │               │
│  Production   │◄────┤   Staging     │◄────┤  Development  │◄────┤  New Branch   │
│   Gateway     │     │   Gateway     │     │   Gateway     │     │   Created     │
│               │     │               │     │               │     │               │
└───────────────┘     └───────────────┘     └───────────────┘     └───────────────┘
```

## Complete Dev Revision Lifecycle

End-to-end flow from developer request to deployed API endpoint.
Shows which parts are visible to AI and which are handled by the system.
A revision encompasses the entire AI agent procedure until validation, not just a single prompt.

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                               Developer Request                                 │
│                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────┘
                                         │
                                         │ Natural Language Prompt
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                          Constrained Execution Environment                      │
│                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────┘
                                         │
                                         │ Enforces budget, time & memory limits
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                                 Dev Processor                                   │
│                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────┘
                                         │
                                         │ Store Prompt in metadata/dev-revisions/XXXX/prompt.md
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                                   AI Agent                                      │
│                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────┘
                                         │
                                         │ Access Relevant Context (Global, Repo, Branch)
                                         │
                                         │ Generate Response (Unaware of System Architecture)
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                                 Code Generator                                  │
│                           (Runs in Isolated Container)                          │
│                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────┘
                                         │
                                         │ Self-debugging up to budget limit (Pure TypeScript Functions Only)
                                         │
                                         │ Store Response in metadata/dev-revisions/XXXX/response.md
                                         │
                                         │ Generate follow-up questions if needed
                                         │
                                         │ Apply ORM and type validation to all generated code
                                         │ (AI Agent unaware of build/transpilation process)
                                         │
                                         │ Create automatic summary of changes
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                                  Git Handler                                    │
│                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────┘
                                         │
                                         │ Create Branch & Store Metadata
                                         │ Trigger Build Process (Hidden from AI Agent)
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                               Branch Metadata                                   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
  ├── branch.info.json  # Branch metadata (creation time, parent branch, etc.)
  ├── changes.json      # Structured representation of code changes
  ├── diff.patch        # Git diff of all changes
  ├── summary.md        # Automatic summarization of changes
  └── linked to dev-revisions/XXXX/ through branch-number file

                                         │
                                         │ (AI Agent unaware of subsequent processes)
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                                 Build System                                    │
│                                                                                 │
└───────────────────────────────────────┬─────────────────────────────────────────┘
                                         │
                                         │ Transpile Code & Add RPC Features
                                         │ Generate API Routes & OpenAPI Specs
                                         │ Configure PM2 Service Manager
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                        PM2 Service Manager (Inside Each Container)              │
│                                 (Independent from Parent)                       │
└───────────────────────────────────────┬─────────────────────────────────────────┘
                                         │
                                         │ Start/Restart Branch-Specific Process
                                         │ Each Branch Runs Independently
                                         ▼
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                                                                 │
│                                 API Gateway Update                              │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
  └── Make new branch available through appropriate gateway (dev/staging/prod)
```


## Log Directory Structure

This diagram illustrates how logs are organized in the system. Each branch has its own logs, but they are stored in a separate repository for scalability reasons. The logs use context-size-based filenames with timestamps.

```
logs-repository/
├── codebases/
│   └── user-management/
│       ├── branches/
│       │   ├── 00001/                        # Branch-specific logs
│       │   │   ├── pm2/                      # PM2 Process Manager Logs
│       │   │   │   ├── 10k-20250404-042500.log  # 10k tokens context size with timestamp
│       │   │   │   ├── 15k-20250404-043000.log  # 15k tokens context size with timestamp
│       │   │   │   └── 8k-20250404-050000.log   # 8k tokens context size with timestamp
│       │   │   │
│       │   │   ├── ttyd/                     # Terminal Session Logs
│       │   │   │   ├── 12k-20250404-042500.log  # Terminal session 1 - 12k tokens context
│       │   │   │   ├── 9k-20250404-043000.log   # Terminal session 2 - 9k tokens context
│       │   │   │   └── 11k-20250404-044500.log  # Terminal session 3 - 11k tokens context
│       │   │   │
│       │   │   └── api-gateway/              # API Gateway Logs
│       │   │       └── 5k-20250404-042500.log   # 5k tokens context size with timestamp
│       │   │
│       │   └── 00002/                        # Another branch's logs
│       │       ├── pm2/
│       │       ├── ttyd/
│       │       └── api-gateway/
│       │
│       └── ...
```

## Monorepo Logs Configuration

The logging system is configured at the monorepo level but logs are stored per branch in a separate repository for scalability:

- Logs are primarily split based on context size (token count), not time periods but it's also referenced
- Each log filename includes context size first, then timestamp (e.g., `10k-20250404-042500.log`)
- Context size thresholds are configured per log type to optimize AI debugging efficiency
- Branch-specific logs ensure isolation and prevent context contamination
- External storage in a separate repository prevents the main repo from growing too large

This approach ensures that logs provide optimal context for AI debugging without exceeding practical token limits. The context-size-based splitting is crucial for AI processing, as it allows the system to provide just the right amount of information without overwhelming the context window.



## Development Workflow

Progressive promotion of changes through development, staging, and production.
Enables continuous development without affecting production stability.

```
┌───────────────┐     ┌───────────────┐     ┌───────────────┐     ┌───────────────┐
│               │     │               │     │               │     │               │
│  Developer    │────►│  Dev Prompt   │────►│   AI Agent    │────►│  Code Changes │
│               │     │               │     │               │     │               │
└───────────────┘     └───────────────┘     └───────────────┘     └───────┬───────┘
                                                                          │
                                                                          │
                                                                          ▼
┌───────────────┐     ┌───────────────┐     ┌───────────────┐     ┌───────────────┐
│               │     │               │     │               │     │               │
│  Production   │◄────┤   Staging     │◄────┤  Development  │◄────┤  New Branch   │
│   Gateway     │     │   Gateway     │     │   Gateway     │     │   Created     │
│               │     │               │     │               │     │               │
└───────────────┘     └───────────────┘     └───────────────┘     └───────────────┘
