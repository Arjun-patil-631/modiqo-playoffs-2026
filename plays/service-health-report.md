# service-health-report

## Purpose
Reusable public-service health/status workflow.

## Input
`service` — public service name.

## Workflow
1. Resolve the service to a known public status source.
2. Fetch current status.
3. Check active incidents.
4. Identify affected components.
5. Produce an overall verdict.

## Public Play
https://play.modiqo.ai/arjun/service-health-report@0.1.0

## Verification
Created and verified with GitHub, Supabase, and Cloudflare.
The published public version was successfully executed with `github`.
