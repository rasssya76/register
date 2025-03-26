<p align="center">
   <img alt="greyrat.dev Banner" src="https://raw.githubusercontent.com/greyrat-dev/register/main/media/banner.png">
</p>

<p align="center">
   <img alt="Domains" src="https://img.shields.io/github/directory-file-count/greyrat-dev/register/domains?color=5c46eb&label=domains&style=for-the-badge">
   <img alt="Open Pull Requests" src="https://img.shields.io/github/issues-raw/greyrat-dev/register?color=5c46eb&label=issues&style=for-the-badge">
   <img alt="Open Issues" src="https://img.shields.io/github/issues-pr-raw/greyrat-dev/register?color=5c46eb&label=pull%20requests&style=for-the-badge">
   <br>
</p>

<h1 align="center">greyrat.dev</h1>

<p align="center"><strong>greyrat.dev</strong> is a service that allows developers to get a sweet-looking <code>.greyrat.dev</code> domain for their personal websites.</p>

# Register
## How to Register

- [Fork](https://github.com/greyrat-dev/register/fork) this repository
- Add a new file called `your-domain-name.json` in the `domains` folder to register `your-domain-name.greyrat.dev`
```json
{
    "description": "Project Description",

    "owner": {
        "repo": "https://github.com/username/repo",
        "email": "hello@example.com"
    },

    "record": {
        "A": ["1.1.1.1", "1.0.0.1"],
        "AAAA": ["::1", "::2"],
        "CNAME": "example.com",
        "MX": ["mx1.example.com", "mx2.example.com"],
        "TXT": ["example_verification=1234567890"],
        "CAA": [
            { "flags": 0, "tag": "issue", "value": "letsencrypt.org" },
            { "flags": 0, "tag": "issuewild", "value": "sectigo.com" }
        ],
        "SRV": [
            { "priority": 10, "weight": 60, "port": 5060, "target": "sipserver.example.com" },
            { "priority": 20, "weight": 10, "port": 5061, "target": "sipbackup.example.com" }
        ]
    },

    "proxied": false
}

```
- Your pull request will be reviewed and merged. *Make sure to keep an eye on it incase we need you to make any changes!*
- After the pull request is merged, please allow up to 24 hours for the changes to propagate
- Enjoy your new `.greyrat.dev` domain! Please consider leaving us a star ⭐️ to help support us!

### NS Records
> **⚠️ Important:**  
> The creation of NS records is temporarily closed. We are currently reviewing our policies and will reopen this feature soon. Thank you for your understanding.

## Report Abuse
If you find any subdomains being used for abusive purposes, please report them by [creating an issue](https://github.com/greyrat-dev/register/issues/new?assignees=&labels=report-abuse&projects=&template=report-abuse.md&title=Report+abuse) with the relevant evidence.

---

<a href="https://www.cloudflare.com">
   <img alt="Cloudflare Logo" src="https://raw.githubusercontent.com/greyrat-dev/register/main/media/cloudflare.png" height="96">
</a>
