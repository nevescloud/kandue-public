# kandue

Source for **kandue.app** — the site, feedback form and issue tracker for the Kandue Chrome extensions, Kandue for Students and Kandue for Graders on Canvas LMS. GitHub Pages from `main:/docs`, CNAME `kandue.app`. No build step: `docs/` is served verbatim. The extensions' source is not in this repository.

- **Installed extensions request these paths directly**, so each must keep answering at the same URL: `/` (homepage), `/feedback.html` (panel link), `/uninstall.html` (opened on uninstall; the graders extension adds `#product=graders`). An installed copy only picks up a new URL when it updates, so moving or renaming one of these paths breaks every older install.
- **One privacy policy per store item**: `privacy.html` for Students, `privacy-graders.html` for Graders. They disclose different hosts; do not merge them.
- **Feedback is a prefilled GitHub issue.** `feedback.html` and `uninstall.html` open `issues/new` in this repository with a `template=` from `.github/ISSUE_TEMPLATE/`; the user submits under their own account. Labels come from the template files, so a new form needs its own template.
- Issues and this repository are public: nothing written here should assume a private reader.

The other two public domains live in other repositories:

- **jonasneves.com** — `jonasneves/jonasneves.github.io`, the author's site; it links here, and the privacy policies' contact address is on that domain.
- **neves.cloud** — `nevescloud/nevescloud.github.io`.
