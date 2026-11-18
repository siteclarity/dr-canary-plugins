# Dr. Canary Customer Journey QA

Find UX bugs and verify fixes

![Dr. Canary Customer Journey QA](assets/icon.png)

Give your AI agent a QA wingman. Bring Dr. Canary customer journey evidence into Claude to find what blocks customers on connected websites, web applications and mobile web.

## What you can do

### Find bugs and improve the user experience

- Review signup, onboarding through a first completed task, forms, booking and checkout.
- Inspect the observed action, result and available browser evidence rather than guessing from a page's appearance.
- Guide: [User experience testing](https://www.drcanary.com/capabilities/user-experience-testing/)

### Prepare a fix brief for your developer or coding agent

- The brief covers what the customer tried, the expected and observed result, the page and recorded browser view, with screenshots when available.
- Your team or coding agent makes the change.
- After a supported recheck, compare later evidence before calling the original problem fixed.
- Guide: [Reports and evidence](https://www.drcanary.com/capabilities/reports/)

### Compare desktop and mobile

- Compare the same step across recorded desktop and mobile views.
- Supported browser profiles are desktop Chrome and emulated mobile WebKit; a particular journey's coverage comes from its records.
- A missing view stays unverified.

### Plan what to try next

- On Monitoring, save a customer task and visible success condition as a shopper's area of focus.
- Saving a focus does not start a check.
- Manage saved shoppers and schedules, review authorized Groups, and request supported rechecks using their actual saved scope.
- Guide: [Secret shoppers](https://www.drcanary.com/capabilities/secret-shoppers/)

### Review lead follow-up

- Read an identified test inquiry alongside the email or text replies that were captured.
- Check whether the response addressed the customer's question.
- A shopper configured to submit can send test inquiries on Monitoring.
- Guide: [Lead engagement testing](https://www.drcanary.com/capabilities/lead-engagement-testing/)

### Inspect cookie consent evidence

- Inspect cookie consent evidence across arrival, rejection, acceptance, withdrawal and return visits.
- Findings describe observed browser requests and storage; they are not a legal compliance certification.
- Guide: [Consent testing](https://www.drcanary.com/capabilities/consent-testing/)

## Requirements

- Requires a Dr. Canary account with connected sites.
- Reads use the evidence available to that account.
- Saved changes and rechecks require the application's role and Monitoring permissions and follow your assistant's approval controls.
- Rechecks can use allowance or send enabled test inquiries; queue acceptance is not report publication.
- Connect and learn the supported workflows: https://www.drcanary.com/mcp/

## Install in Claude Code

```
/plugin install dr-canary --marketplace siteclarity/dr-canary-plugins
```

## Connect your account

1. Open this plugin's Connectors tab in Claude and connect Dr. Canary.
2. Sign in through Dr. Canary's normal OAuth flow and review the account permissions.
3. On Team or Enterprise, your organization owner first adds the connector. Each member then connects their own Dr. Canary account.

### What your account allows

- Reads use the sites and reports available to that account.
- Changing saved shoppers or requesting checks requires the application's existing owner or admin role and active Monitoring.
- A one-time Checkup supplies its report and evidence.
- The shopper's settings determine inquiry effects, and checks can use the site's allowance.

## Skills

- **`report-review`**
  - Helps explain published findings, screenshots, browser coverage, inquiry replies and report comparisons.
  - Preserves unavailable evidence and the scope of the recorded check.
- **`site-test`**
  - Helps manage saved shoppers, calendars and areas of focus, request supported checks, and follow the exact returned run to its report.
  - Follows Claude's approval controls and the account's application permissions.

## Try these requests

Try these requests after connecting your account.

- Find the customer blockers in my latest report and prepare a fix brief for my coding agent.
- Save a signup-to-first-task focus on my app's shopper, without running a check.
- I deployed a fix. Help me recheck my connected site, then compare the new evidence with the original finding.

## Data

- The plugin sends tool requests to your Dr. Canary account through `https://www.drcanary.com/api/mcp/`. These carry the site, report, check or shopper you ask about and any shopper settings you save.
- The plugin stores nothing itself.
- It contains skills, a connector reference and an icon. It has no scripts, hooks or local servers.
- [Privacy policy](https://www.drcanary.com/legal/privacy/)

## Documentation and support

- [Capabilities and examples](https://www.drcanary.com/capabilities/)
- [Connection guide](https://www.drcanary.com/mcp/)
- [Supported tools](https://www.drcanary.com/mcp/tools/)
- [Account permissions](https://www.drcanary.com/mcp/permissions/)
- [Connection troubleshooting](https://www.drcanary.com/mcp/troubleshooting/)
- [Privacy policy](https://www.drcanary.com/legal/privacy/)
- [Terms of service](https://www.drcanary.com/legal/terms/)

## License

- Published by SCAI LLC under the [Apache License 2.0](LICENSE).
- The license covers the files in this plugin. It does not grant permission to use the Dr. Canary name or logo.
- Use of the Dr. Canary service is governed by its [Terms of service](https://www.drcanary.com/legal/terms/).
- [Contact support](https://www.drcanary.com/mcp/troubleshooting/)
