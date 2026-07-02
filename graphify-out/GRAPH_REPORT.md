# Graph Report - findfee  (2026-07-02)

## Corpus Check
- 33 files · ~6,991 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 78 nodes · 49 edges · 2 communities detected
- Extraction: 96% EXTRACTED · 4% INFERRED · 0% AMBIGUOUS · INFERRED: 2 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Community 0|Community 0]]
- [[_COMMUNITY_Community 3|Community 3]]

## God Nodes (most connected - your core abstractions)
1. `useSidebar()` - 3 edges
2. `NavProjects()` - 2 edges
3. `NavUser()` - 2 edges
4. `cn()` - 2 edges
5. `BreadcrumbLink()` - 2 edges
6. `cn()` - 2 edges
7. `SidebarMenuSubButton()` - 2 edges

## Surprising Connections (you probably didn't know these)
- `NavProjects()` --calls--> `useSidebar()`  [INFERRED]
  src\components\nav-projects.tsx → src\components\ui\sidebar.tsx
- `NavUser()` --calls--> `useSidebar()`  [INFERRED]
  src\components\nav-user.tsx → src\components\ui\sidebar.tsx

## Communities

### Community 0 - "Community 0"
Cohesion: 0.25
Nodes (5): NavProjects(), NavUser(), cn(), SidebarMenuSubButton(), useSidebar()

### Community 3 - "Community 3"
Cohesion: 0.5
Nodes (2): BreadcrumbLink(), cn()

## Knowledge Gaps
- **Thin community `Community 3`** (5 nodes): `breadcrumb.tsx`, `Breadcrumb()`, `BreadcrumbLink()`, `BreadcrumbPage()`, `cn()`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Are the 2 inferred relationships involving `useSidebar()` (e.g. with `NavProjects()` and `NavUser()`) actually correct?**
  _`useSidebar()` has 2 INFERRED edges - model-reasoned connections that need verification._