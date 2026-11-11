# ResellingKori Postman Collection

Test the [ResellingKori Partner API](https://github.com/Resellingkori/partner-docs) directly from Postman — no code needed.

## Setup (2 minutes)

1. Download `ResellingKori-Partner-API.postman_collection.json`
2. Open **Postman** → **Import** → select the file
3. Click the collection → **Variables** tab
4. Set these three variables:

| Variable | Value |
|---|---|
| `base_url` | `https://resellingkori.com/wp-json/rk/v1` |
| `key_id` | Your Key ID (`rkk_...`) |
| `secret` | Your Secret (`rks_...`) |

5. Click **Save**

## Test your connection

Open the **Ping** request → click **Send**  
Expected: `200 OK` ✅

The collection signs every request automatically (HMAC-SHA256 / RK2).

## Requests

| # | Request | Method | What it does |
|---|---|---|---|
| 1 | Ping | GET | Check connection |
| 2 | Get products | GET | Browse catalogue |
| 3 | Search products | GET | Search by keyword |
| 4 | Get product | GET | Single product details |
| 5 | Validate order | POST | Check order without creating it |
| 6 | Create order | POST | Place a real order |
| 7 | Get order | GET | Look up an order |
| 8 | List orders | GET | List your orders |
| 9 | Cancel order | POST | Cancel an order |
| 10 | Get stores | GET | List your stores |
| 11 | Rotate key | POST | Generate a new secret |
| 12 | List webhooks | GET | Show registered webhooks |
| 13 | Register webhook | POST | Add a webhook URL |
| 14 | Verify webhook | POST | Test webhook delivery |
| 15 | Update webhook | PATCH | Change webhook settings |
| 16 | Delete webhook | DELETE | Remove a webhook |

## Sandbox

Change `base_url` to `https://sandbox.resellingkori.com/wp-json/rk/v1` for testing.

## Documentation

- [Getting Started](https://github.com/Resellingkori/partner-docs/blob/main/GETTING_STARTED.md)
- [Full API Guide](https://github.com/Resellingkori/partner-docs/blob/main/PARTNER_API_GUIDE.md)
