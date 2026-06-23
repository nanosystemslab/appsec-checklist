# API Endpoint Inventory

| Method | Path/topic | Purpose | Auth required? | Required role/scope | Input validation | Rate limit | Logs? |
|---|---|---|---|---|---|---|---|
| GET | /api/devices/{id}/status | | Yes | viewer | device ID authorization | | Yes |
| POST | /api/devices/{id}/command | | Yes | operator/admin | schema + range checks | | Yes |
