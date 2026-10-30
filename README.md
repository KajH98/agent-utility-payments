# Agent Utility Hub — Paid Website Status API

A machine-readable website availability and response-time
checking API for AI agents, automation tools, and developers.

## API Endpoint

GET https://agent-utility-x402.irishkaj.workers.dev/check?url=https://example.org

## Pricing

$0.01 USDC per request.

Payments use the x402 protocol on Base mainnet.

No subscription or API key required.

## What It Does

- Checks whether a public website responds
- Reports HTTP status
- Measures response time in milliseconds
- Follows up to 3 redirects
- Returns machine-readable JSON

## Example Response

{
  "website": "example.org",
  "reachable": true,
  "http_status": 200,
  "http_success": true,
  "response_time_ms": 37,
  "redirects_followed": 0,
  "checked_at": "2026-10-30T18:00:00.000Z"
}

The response above is illustrative. Actual results vary.

## Payment

Unpaid requests receive HTTP 402 Payment Required.

Compatible x402 clients can use the payment requirements
returned by the gateway to authorize payment and retry.

Network: Base mainnet
Asset: USDC
Price: $0.01 per request

## Limitations

- Public HTTP/HTTPS websites only
- Homepage checks only
- No custom ports
- HEAD requests
- 8-second overall timeout

## Status

The API is deployed. Unpaid access protection has been
verified. Successful payment and settlement have not yet
been independently tested.
