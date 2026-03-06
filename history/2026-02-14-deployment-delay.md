# Incident Report: CDN Asset Delay

**Date:** 2026-02-14  
**Duration:** 45 minutes  
**Impact:** Intermittent 404 errors when accessing the 2026 Press Kit PDF.  

**Root Cause:** A misconfiguration in the CDN cache invalidation script caused the `eggtrail-spring-campaign-kit-2026.pdf` to be served as an empty object for approximately 15 minutes.

**Resolution:** Sara (Ops) manually purged the edge cache and re-verified the file hash. All systems are now nominal.
