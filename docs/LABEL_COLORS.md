# Label Organization Guide

## Label Categories

| Label Name | Category | Description |
|------------|----------|-------------|
| bug | issue-type | Something isn't working; use for defects and regressions. |
| enhancement | issue-type | Request for a new feature or improvement. |
| documentation | issue-type | Documentation additions, corrections, or organization tasks. |
| question | issue-type | Information is requested or clarification needed. |
| duplicate | status | Indicates this issue/PR already exists and duplicates another. |
| has repro | status | A reliable reproduction has been provided or confirmed. |
| platform:macos | platform | macOS-specific issues, fixes, or behavior. |
| platform:linux | platform | Linux-specific issues, fixes, or behavior. |
| platform:windows | platform | Windows-specific issues, fixes, or behavior. |
| area:core | area | Core functionality, runtime, and foundational components. |
| area:tools | area | Built-in tools, utilities, and tool integrations. |
| area:ide | area | IDE integrations, status line, UI/UX in IDE terminals. |
| area:mcp | area | Model Context Protocol (MCP) integrations and behavior. |
| area:api | area | API surface, requests/serialization, and external API behavior. |
| area:tui | area | Terminal UI/interaction, rendering, and keybindings. |
| area:security | area | Security model, permissions, sandboxing, and authz. |
| area:packaging | area | Packaging, installers, distribution, and release artifacts. |
| area:model | area | Model behavior, outputs, selection, and routing. |
| area:auth | area | Authentication, keys, profiles, and identity flows. |
| memory | performance | Memory-related incidents, usage, and leaks. |
| perf:memory | performance | Memory performance degradations and optimizations. |
| external | meta | External factors, upstream dependencies, or third-party changes. |

## Usage Guidelines

- issue-type
  - bug: Use for confirmed defects or regressions with expected vs actual behavior.
  - enhancement: Use for adding new capabilities or improving existing ones.
  - documentation: Use for documentation work including guides, READMEs, and examples.
  - question: Use for clarification, support questions, or information requests.

- platform
  - Apply alongside other labels when a problem or feature is specific to macOS, Linux, or Windows.
  - Use multiple platform labels if it affects more than one platform in distinct ways.

- area
  - Choose the area that best matches the code or system affected (core, tools, ide, mcp, api, tui, security, packaging, model, auth).
  - Prefer one primary area; add a secondary area only if strictly necessary.

- status
  - duplicate: Apply when closing as duplicate and reference the canonical issue.
  - has repro: Apply when a clear reproduction has been supplied (steps, environment, and expected vs actual).

- performance
  - memory: Use for general memory concerns and tracking.
  - perf:memory: Use to denote performance-specific memory issues (heap usage spikes, GC pressure, leaks) and optimization work.

- meta
  - external: Use when issues are largely driven by external dependencies, upstream projects, or platform changes beyond our control.

General guidance
- Prefer adding an issue-type label plus area and platform as needed to improve visual organization and triage.
- Keep labels consistent so filtering and dashboards remain useful.
- If in doubt, add a comment explaining label choices; maintainers can refine as needed.
