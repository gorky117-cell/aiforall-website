# AI for ALL Website

Website and demo-request backend for AI for ALL.

## Railway

Deploy this repository on Railway with the Node start command:

```powershell
npm start
```

Set these Railway variables for the contact / request-demo form:

| Variable | Purpose | Recommended value |
| --- | --- | --- |
| `RESEND_API_KEY` | Resend API key used to send emails | From Resend dashboard |
| `REQUEST_DEMO_TO` | Your inbox for new demo requests | `gaurav@aiforall.ltd` |
| `REQUEST_DEMO_FROM` | Verified sender identity for emails to you | `AI for ALL <gaurav@aiforall.ltd>` |
| `REQUEST_DEMO_CONFIRMATION_FROM` | Verified sender identity for confirmation emails to visitors | `AI for ALL <gaurav@aiforall.ltd>` |
| `REQUEST_DEMO_REPLY_TO` | Where visitor replies should go | `gaurav@aiforall.ltd` |
| `REQUEST_DEMO_REDIRECT` | Success page after form submit | `/request-demo-thanks.html` |

The form sends:

- A new request email to `REQUEST_DEMO_TO`.
- A confirmation email to the visitor who submitted the form.

## Domains

The server routes domains as follows:

- `www.aiforall.ltd` and `aiforall.ltd` serve `aiforall-final.html`.
- `gaurav.aiforall.ltd` serves `index.html`.
