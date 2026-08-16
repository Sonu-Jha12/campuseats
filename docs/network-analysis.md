# Network Analysis

## Page Load Summary

- Total requests: 30
- Total data transferred: 1.6 MB
- Total resources/page size: 1.9 MB
- Finish time: 12.13 seconds
- DOMContentLoaded: 3.46 seconds
- Load event: 7.44 seconds

## Slowest Resource

The slowest resource was:

`553780578-52b3039d-1e4c-4684-951c-93f0f1e73611.png`

- Type: PNG
- Status: 200 OK
- Size: 341 kB
- Time: 4.03 seconds

This was the slowest resource visible in the Network waterfall.

## 3xx and 4xx Responses

### 302 — Found / Redirect

A request returned status code 302. This means the requested resource was temporarily redirected to another location.

### 404 — Not Found

The `rum` XHR request returned status code 404. This means the requested resource could not be found on the server.

### 204 — No Content

Some requests returned 204. This means the request was successfully processed, but the server returned no response body.

## Observation

The page made 30 network requests. The total resource size was about 1.9 MB. The slowest individual resource was a 341 kB PNG that took 4.03 seconds. The page reached DOMContentLoaded in 3.46 seconds and the Load event occurred at 7.44 seconds.
