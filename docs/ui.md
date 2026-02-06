# Dashboard UI Design (Competitor-Inspired, Modern)

## Design Principles
- **Information density with clarity**: compact cards, consistent spacing, progressive disclosure.
- **Action-oriented**: primary CTAs anchored in top-right for quick workflows.
- **Predictable navigation**: left sidebar with sections and nested items.
- **Real-time context**: status indicators, timestamp labels, and live updates.

## Layout Overview
```
┌─────────────────────────────────────────────────────────────────────────┐
│ Top Bar: Logo | Workspace switcher | Search | Notifications | User menu │
├───────────────┬─────────────────────────────────────────────────────────┤
│ Sidebar       │ Main Content                                             │
│ - Overview    │ - KPI summary cards (4-6)                                │
│ - Analytics   │ - Trend chart (line/area)                                │
│ - Users       │ - Funnel/Retention chart                                │
│ - Billing     │ - Table: latest events                                  │
│ - Settings    │ - Right rail: alerts + tasks (optional)                  │
└───────────────┴─────────────────────────────────────────────────────────┘
```

## Key Screens
### 1) Overview Dashboard
- **KPI cards**: ARR, MRR, Active Users, Conversion Rate, Churn.
- **Primary chart**: multi-series line/area (last 30/90 days).
- **Secondary chart**: cohort retention or funnel breakdown.
- **Table**: recent activity (user signups, payments, alerts).

### 2) Analytics
- **Segmented filters**: product, region, plan, channel.
- **Chart types**: line, bar, stacked area.
- **Drill-down drawer**: click data points to open detail panel.

### 3) Users
- **User list** with inline status (Active/Paused).
- **Details drawer** for profile, usage, billing.
- **Bulk actions**: export, suspend, tag.

### 4) Billing
- **Revenue breakdown** by plan.
- **Invoices** and **payouts** table.
- **Alerts** for failed payments.

## Components & Interactions
- **Global search** with typeahead and keyboard shortcuts.
- **Notifications** panel for incidents and system events.
- **Contextual filters** pinned to top of content area.
- **Empty states** with action prompts.
- **Skeleton loaders** for async data.

## Visual Design (Competitor Dashboard Style)
- **Color palette**: Neutral base with single accent (e.g., Indigo/Teal).
- **Typography**: Inter or Manrope.
- **Cards**: soft shadows, 12px radius, subtle borders.
- **Charts**: minimal gridlines, bold tooltips.
- **Dark mode**: optional, with elevated surfaces.

## Example Component Spec
### KPI Card
- Title, value, delta (+/-), sparkline.
- Support for time range selection.

### Sidebar
- Collapsible groups
- Sticky bottom with workspace settings and help.

## UI Tech Stack (Latest)
- **Next.js 14** + React Server Components.
- **Tailwind CSS** + **shadcn/ui** components.
- **Recharts** or **Visx** for charts.
- **Radix UI** primitives for accessibility.
- **TanStack Table** for data grids.
