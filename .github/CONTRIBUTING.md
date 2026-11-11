# Contributing to DP-700 Study Notes v2

Thanks for helping keep these notes accurate. They cover **Microsoft DP-700: Implementing Data Engineering Solutions Using Microsoft Fabric**, and Microsoft Fabric ships changes almost weekly, so features get renamed, move from preview to general availability, or change their limits between one revision of the study guide and the next. Reports from people studying with the notes are the best way to catch that.

> [!IMPORTANT]
> **This repo accepts issues, not pull requests.** Pull requests are turned off: I write every change myself and check it against the official documentation, so the notes keep one voice and stay consistent from page to page. If you know exactly how something should read, put your proposed wording in the issue. It's just as useful.

---

## Contents

- [Ways to Help](#-ways-to-help)
- [Before You Open an Issue](#-before-you-open-an-issue)
- [Opening an Issue](#-opening-an-issue)
- [Out of Scope](#-out-of-scope)
- [What Happens Next](#-what-happens-next)
- [Code of Conduct](#-code-of-conduct)
- [Security](#-security)

## 🙌 Ways to Help

Every report fits one of the five types in the issue template:

| Type | What it covers | For example |
| --- | --- | --- |
| **Bug** | A link, the menu, the **On this page** contents, the theme toggle, a diagram or another site feature is broken | A Mermaid diagram doesn't redraw after you switch to dark mode, a contents link doesn't jump to its section, or a Microsoft Learn link returns 404 |
| **Content issue** | Something in the notes is wrong, unclear or missing | A PySpark, T-SQL or KQL sample doesn't run as written, a capacity figure is off, or a decision tree points to the wrong item type |
| **Outdated content** | Microsoft Fabric or the DP-700 exam has changed since the page was written | A preview feature is now generally available, a setting has moved in the admin portal, or the study guide lists a skill the notes don't cover |
| **Device issue** | The site displays or behaves badly on a specific device or browser | A wide comparison table overflows on a phone in portrait, or the menu won't close on a tablet |
| **Other issue** | Anything else, including ideas that would make the notes easier to study | A topic that would read better as a scenario table, or an exam caveat worth adding |

## 🔎 Before You Open an Issue

- **Search the existing issues**, [open and closed](https://github.com/marcogrimaldi29/dp-700-study-notes-v2/issues?q=is%3Aissue). If yours is already there, add a 👍 reaction or a comment with anything new rather than opening a duplicate.
- **Check the date.** The notes are written against the skills measured effective **21 July 2026**. Compare that with the **Skills measured** section of the [DP-700 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/dp-700): if its heading shows a later date, or it lists a skill the notes don't cover, say so in the issue — it tells me which revision to compare against.
- **Check the current docs.** A quick look at the [Microsoft Fabric documentation](https://learn.microsoft.com/en-us/fabric/), and its [What's new](https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new) page in particular, usually confirms whether something has changed, and gives you the link the issue asks for.
- **One problem per issue.** Separate issues are easier to track, fix and close. Several typos on the same page can go in one issue.
- **For a site bug, hard-refresh first** (Ctrl+F5, or Cmd+Shift+R on a Mac) in case your browser is showing an older copy of the page.

## 📝 Opening an Issue

1. Open a new issue with the [Report a problem](https://github.com/marcogrimaldi29/dp-700-study-notes-v2/issues/new?template=ISSUE_TEMPLATE.md) template.
2. Give it a title that names the page and the problem, for example *"Domain 3: Monitor Fabric items uses an old name for Activator"* rather than *"Mistake on page"*.
3. Put an x in the box for the type of problem, fill in the sections that apply, and delete the rest.

> [!TIP]
> To link straight to a section, click its heading in **On this page**, then copy the address from your browser.

### What Makes a Report Easy to Fix

- **A link to the exact section**, not just the page
- **The text as the notes have it**, quoted, so it can be found even if the page has moved on
- **An official source** for any content change — Microsoft Learn is best. A report without one may take longer, because every change has to be checked against the documentation before it goes in
- **Whether the feature is in preview or generally available**, if it matters. The study guide says most questions cover generally available features, so the status changes what the notes should say
- **For bugs and device issues:** the steps to reproduce it, what you expected and what happened instead, the device, operating system, browser and theme, and a screenshot if it shows the problem
- **Your proposed wording**, if you have it. With pull requests turned off, this is the closest thing to suggesting an edit directly

## 🚫 Out of Scope

To keep the notes accurate and the issue tracker useful, please don't open issues for:

- **Live exam content.** Questions, answers or topics remembered from a real exam break [Microsoft's exam security policy](https://learn.microsoft.com/en-us/credentials/support/exam-and-assessment-lab-security-policies) and the exam NDA. Issues or comments that include them will be closed and the content removed.
- **Exam booking, scores or retakes.** [Microsoft Credentials support](https://learn.microsoft.com/en-us/credentials/support/help) can help with those.
- **Help with your own Fabric tenant or project.** For troubleshooting a capacity, a workspace, a pipeline or your own code, ask on the [Microsoft Fabric Community](https://community.fabric.microsoft.com/) or [Microsoft Q&A](https://learn.microsoft.com/en-us/answers/), or open a Microsoft support request.
- **Anything private.** Issues are public, so leave out tenant and workspace IDs, connection strings, keys and tokens, and customer data, including in screenshots.
- **Unofficial sources.** Exam dump sites, third-party practice tests and AI chat answers aren't accepted as the source for a content change.
- **Promotion.** Links to courses, products or services, affiliate links and paid placements won't be added.
- **Security vulnerabilities.** Please [report these privately](https://github.com/marcogrimaldi29/dp-700-study-notes-v2/security/advisories/new), as described in the [security policy](SECURITY.md), not in a public issue.

## 🔄 What Happens Next

- I maintain the notes on my own, in my spare time, so replies are best effort and there's no fixed response time.
- I check each report against the official documentation. If something needs clarifying, I'll ask on the issue, so keep an eye on your GitHub notifications.
- When a fix goes in, the issue is closed with a note on what changed or a link to the change. The live site updates shortly after.
- If nothing changes, the issue is closed with the reason, such as out of scope, can't be verified, or working as intended.
- An issue waiting on a reply may be closed after a while. Comment with the missing details and it can be reopened.

## 🤝 Code of Conduct

By opening, commenting on or reacting to issues here, you agree to follow the [Code of Conduct](CODE_OF_CONDUCT.md). Comments that are abusive, spam or share live exam content may be hidden, edited or locked.

## 🔒 Security

Found a security problem with the site or this repo? Please don't report it in a public issue. Use [Report a vulnerability](https://github.com/marcogrimaldi29/dp-700-study-notes-v2/security/advisories/new) instead, so only you and I can see it. The [security policy](SECURITY.md) has the details.

---

If the notes helped you, the README's [Support](https://github.com/marcogrimaldi29/dp-700-study-notes-v2#support) section has a couple of ways to show it. Thanks for helping make them better for the next DP-700 candidate.
