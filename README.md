# Canva (canva)
APIs for the Canva design platform, enabling developers to integrate Canva's design tools and functionality into their applications.

**URL:** [Visit APIs.json URL](https://www.canva.com/developers/apis.json)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Apps, Automation, Brand Management, Collaboration, Design, Graphics, Marketing, Print, Templates, Visual Content

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-04-18

## APIs

### Canva Connect API
Enables users to create and edit Canva designs directly from your application, with support for templates, autofill, and design management.

**Human URL:** [https://www.canva.com/developers/](https://www.canva.com/developers/)

#### Tags:

 - Assets, Autofill, Brand Templates, Collaboration, Comments, Design, Design Import, Exports, Folders, Graphics, Resizes, Templates, Users, Webhooks

#### Properties

- [Documentation](https://www.canva.com/developers/docs/connect-api/)
- [OpenAPI](openapi/canva-connect-api-openapi.yml)
- [Authentication](https://www.canva.com/developers/docs/connect-api/authentication/)
- [GettingStarted](https://www.canva.com/developers/docs/connect-api/get-started/)
- [APIReference](https://www.canva.com/developers/docs/connect-api/api-reference/)
- [Quickstart](https://www.canva.dev/docs/connect/quickstart/)
- [ChangeLog](https://www.canva.dev/docs/connect/changelog/)
- [RateLimits](https://www.canva.dev/docs/connect/api-requests-responses/)
- [Security](https://www.canva.dev/docs/connect/guidelines/security/)
- [Versioning](https://www.canva.dev/docs/connect/versions/)
- [GitHubRepository](https://github.com/canva-sdks/canva-connect-api-starter-kit)
- [MCP Server](https://www.canva.dev/docs/connect/mcp-server/)
- [JSONSchema](json-schema/canva-design-schema.json)
- [JSONLD](json-ld/canva-context.jsonld)

### Canva Apps SDK
Build apps that extend Canva's editor with custom functionality, content, and integrations.

**Human URL:** [https://www.canva.com/developers/apps](https://www.canva.com/developers/apps)

#### Tags:

 - Apps, Content Publishing, Data Connectors, Design Editing, Extensions, Integrations, Intents, SDK, Tables

#### Properties

- [Documentation](https://www.canva.com/developers/docs/apps/)
- [GettingStarted](https://www.canva.com/developers/docs/apps/quickstart/)
- [APIReference](https://www.canva.com/developers/docs/apps/api/)
- [CodeExamples](https://www.canva.com/developers/docs/apps/examples/)
- [GitHubRepository](https://github.com/canva-sdks/canva-apps-sdk-starter-kit)

### Canva Print Partnerships API
Enables print service providers to integrate Canva design tools into their customer journey.

**Human URL:** [https://www.canva.dev/docs/print-partnerships/](https://www.canva.dev/docs/print-partnerships/)

#### Tags:

 - Design, E-Commerce, Partnerships, Print

#### Properties

- [Documentation](https://www.canva.dev/docs/print-partnerships/)
- [GettingStarted](https://www.canva.dev/docs/print-partnerships/tutorial/getting-started/)

### Canva Button API
Enables embedding Canva design capabilities directly into websites and applications.

**Human URL:** [https://www.canva.dev/docs/button/](https://www.canva.dev/docs/button/)

#### Tags:

 - Button, Design, Embed, Integration, Widget

#### Properties

- [Documentation](https://www.canva.dev/docs/button/)
- [GettingStarted](https://www.canva.dev/docs/button/html/getting-started/)

## Common Properties

- [DeveloperPortal](https://www.canva.com/developers/)
- [Authentication](https://www.canva.com/developers/docs/authentication/)
- [Support](https://www.canva.com/developers/support/)
- [TermsOfService](https://www.canva.com/policies/developer-terms/)
- [PrivacyPolicy](https://www.canva.com/policies/privacy-policy/)
- [Blog](https://www.canva.com/newsroom/developers/)
- [StatusPage](https://status.canva.com/)
- [GitHubOrganization](https://github.com/canva-sdks)
- [ChangeLog](https://www.canva.dev/docs/connect/changelog/)
- [Security](https://www.canva.dev/docs/connect/guidelines/security/)
- [RateLimits](https://www.canva.dev/docs/connect/api-requests-responses/)
- [CLI](https://www.npmjs.com/package/@canva/cli)
- [Events](https://www.canva.com/canva-extend/)

## Features

| Name | Description |
|------|-------------|
| Design Creation | Create and manage Canva designs programmatically from external applications. |
| Asset Management | Upload, retrieve, and manage image and video assets within Canva. |
| Brand Templates | Access and list brand templates with dataset definitions for consistent brand content. |
| Design Autofill | Automatically populate brand templates with dynamic data for bulk content creation. |
| Design Export | Export designs to PDF, PNG, JPG, GIF, PPTX, and MP4 formats. |
| Design Resize | Resize designs to different dimensions or preset types for multi-channel publishing. |
| Folder Organization | Organize designs into folders with move, list, and retrieval capabilities. |
| Comments and Collaboration | Create and manage comments on designs for team review and feedback workflows. |
| Webhooks | Receive real-time notifications for design events via webhook subscriptions. |
| Apps SDK | Build custom apps that extend the Canva editor with new functionality and content. |

## Use Cases

| Name | Description |
|------|-------------|
| Marketing Automation | Generate branded marketing materials at scale by autofilling templates with campaign data. |
| Print-on-Demand | Integrate Canva design tools into e-commerce platforms for custom product design. |
| Content Management | Build content pipelines that create, export, and distribute visual content. |
| Brand Consistency | Ensure brand compliance using locked brand templates with controlled elements. |
| Social Media Publishing | Create and export social media graphics in multiple formats and sizes. |

## Integrations

| Name | Description |
|------|-------------|
| Slack | Share Canva designs directly to Slack channels for team review. |
| Google Drive | Save and sync Canva designs with Google Drive. |
| Dropbox | Connect Canva with Dropbox for cloud storage and asset management. |
| HubSpot | Create marketing visuals within HubSpot using Canva. |
| Shopify | Design product images and marketing materials for Shopify stores. |
| WordPress | Create and embed Canva designs into WordPress posts and pages. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Canva Connect API](openapi/canva-connect-api-openapi.yml)

### JSON Schema

- [Design](json-schema/canva-design-schema.json)
- [Connect Design](json-schema/canva-connect-design-schema.json)
- [Asset](json-schema/canva-connect-asset-schema.json)
- [Folder](json-schema/canva-connect-folder-schema.json)
- [Export Job](json-schema/canva-connect-export-job-schema.json)
- [Comment](json-schema/canva-connect-comment-schema.json)
- [Brand Template](json-schema/canva-connect-brand-template-schema.json)

### JSON-LD

- [Canva Context](json-ld/canva-context.jsonld)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Canva Connect API](capabilities/shared/connect-api.yaml) -- 22 operations for designs, assets, exports, brand templates, autofill, and collaboration

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Design Management](capabilities/design-management.yaml) | Connect API | 20 | Marketing Team |

## Rules

- [Canva Spectral Rules](rules/canva-spectral-rules.yml) -- 7 rules enforcing Canva Connect API conventions

## Maintainers

**FN:** Canva

**Email:** developers@canva.com

**FN:** Kin Lane

**Email:** kin@apievangelist.com
