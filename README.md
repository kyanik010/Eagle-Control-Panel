# Eagle Control Panel

Independent IPTV administration dashboard for managing devices, customers, subscriptions, IPTV sources, external audio M3U catalogs, and synchronization logs.

## Current status

The first commit provides a responsive frontend prototype in `index.html`. Navigation works, and the interface includes sample display data clearly marked as non-production. No real customer data is included.

**Not production-ready yet:** administrator authentication, database access, server-side authorization, audit logs, and IPTV/API integrations have not been connected. Buttons and records that imply backend operations must not be treated as functional until the secure backend is implemented.

## Planned implementation

1. Confirm the interface and dashboard modules.
2. Create a separate Supabase project and database schema.
3. Add secure administrator authentication and role-based authorization.
4. Implement server-side/Edge Function endpoints for device activation, subscriptions, IPTV profiles, and external audio M3U settings.
5. Connect the frontend to those endpoints using only public client configuration; never place service-role keys or IPTV credentials in browser code.
6. Configure GitHub Pages and verify the deployed site.
7. Test each workflow against test data before production use.

## Deploy the static preview

In GitHub, open **Settings → Pages**, select **Deploy from a branch**, choose the default branch and **/(root)**, then save. The repository must be public for standard GitHub Pages on plans that do not support Pages for private repositories.

The static preview can be published before the backend is ready, but it must not contain secrets or real customer data.
