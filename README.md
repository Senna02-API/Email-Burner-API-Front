🚀Email Burner API
**Stop spam signups and protect your database from disposable email addresses.**

👋About me:
I'm a developer with 5 years of experience across Web Dev and Game Dev (C#/Unity). I’ve spent the last 3 years deep-diving into backend architecture and React. I built this API because I wanted to apply enterprise-level logic (like real-time DNS MX-probing) to a simple, affordable tool that actually solves a headache I kept running into in my own projects.

🛡️Privacy:
My API is stateless, I don't store your users emails in databases unlike some big data broker companies.
The service performs a two-step check:
-Blocklist check: Cross reference against known disposable domains (updated daily)
-DNS fallback: Performs a real-time MX-record lookup to catch fresh spam domains that aren't on any lists yet.

⚡ Quick start:
No complex headers or SDKs, just a GET request.

Endpoint:
GET "https://your-railway-url.com/v1/check?email=test@example.com&customer_id=demo"

### Example Response:
{
  "email": "user@temporary-mail.com",
  "is_burner": true,
  "status": "block",
  "reason": "no_mx_record",
  "mode": "demo"
}

💎Pricing:
I don't like credit systems. If your app goes viral, you shouldn't be punished with a massive bill.

€5/month — Unlimited requests.
No Database — Your data is processed in memory and dropped.
Support a Student — Your subscription helps me keep the servers running and keep learning.

💬Feedback?
I'm building this to learn. If you have a suggestion, or found a bug, please reach out!

Email: bravery.cs@gmail.com
Reddit: u/Pale_Arm_7625


