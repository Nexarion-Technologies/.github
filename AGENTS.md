# AGENTS.md

## Cursor Cloud specific instructions

This repository is **documentation and GitHub templates only** — it is the public
GitHub organization profile / community-health repo for Nexarion Technologies
(see `README.md`). There is **no application, dependency manifest, build system,
package manager, or runnable service** here.

- **No dependencies to install.** There is no `package.json`, `requirements.txt`,
  lockfile, `Dockerfile`, `Makefile`, or CI workflow. The startup update script is
  intentionally a no-op; do not add build/test/dependency steps to it.
- **What to "run" / validate** (all with tools already present on the VM):
  - Validate the GitHub issue-form templates parse as valid YAML:
    `python3 -c "import yaml,glob; [yaml.safe_load(open(f)) for f in glob.glob('.github/**/*.yml', recursive=True)]"`
  - The org profile page is `profile/README.md`; it renders on the GitHub org
    Overview page and contains a **Mermaid** flowchart under the "Keystone"
    section. To preview rendering locally, render the Markdown with a
    Markdown+Mermaid renderer (e.g. a small static HTML page using the
    `markdown-it` and `mermaid` CDN builds) and open it in the browser. Node.js
    and Python 3 are available; `cdn.jsdelivr.net` is reachable.
- **The four "products" referenced in `profile/README.md`** (e.g.
  `mcp-operations-context-demo`, `n8n-ai-workflow-demo`, `api-bridge-health-demo`,
  `ai-prompt-eval-harness`) live in **separate external repositories** and are
  **not** part of this workspace. Do not expect their source here.
- **Contribution constraints** in `CONTRIBUTING.md` and `PUBLICATION_POLICY.md`
  apply: use synthetic data only; never add secrets, credentials, private
  endpoints, tenant identifiers, or internal infrastructure details.
