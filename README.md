# 🚀 Email Burner API
**Stop spam signups and protect your database from disposable email addresses.**

A high-performance, flat-rate API that detects 100k+ temporary and burner email domains in real-time.

---

## ⚡ Quick Start
Get an answer in milliseconds. 

**Endpoint:**
`GET https://email-burner-api-production.up.railway.app/v1/check?email=target@example.com&customer_id=YOUR_ID`

### Example Response:
```json
{
  "email": "test@mailinator.com",
  "disposable": true,
  "status": "block",
  "message": "Request processed under your monthly subscription."
}
