# LDT4SSC Pilot Project Repository

> ## 🚧 Setup instructions — delete this section once your repository is live
>
> Prefer GitLab (gitlab.com or your own self-managed instance)? Use the
> [GitLab pilot template](https://gitlab.com/ldt4ssc/pilot-template) instead.
>
> 1. Get your own copy of the template:
>    - **On github.com:** click **"Use this template" → "Create a new
>      repository"** on the `pilot-template` GitHub repo, choosing your
>      pilot's org/name, then clone it locally.
>    - **On a GitHub Enterprise Server (GHES) instance:** "Use this
>      template" only works within a single GitHub instance, so you can't
>      use it across github.com → your GHES org. Instead, clone from the
>      public template and push to your own instance:
>      ```bash
>      git clone https://github.com/ldt4ssc/pilot-template.git ldt4ssc-<your-pilot-slug>
>      cd ldt4ssc-<your-pilot-slug>
>      rm -rf .git && git init
>      git remote add origin <your-new-ghes-repo-url>
>      git add -A && git commit -m "Initial commit"
>      git push -u origin main
>      ```
>      Also note: [.github/workflows/validate-updates.yml](.github/workflows/validate-updates.yml)
>      calls a **reusable workflow** hosted at
>      `github.com/ldt4ssc/ldt4ssc.github.io` — GitHub Actions reusable
>      workflows cannot be called across different GitHub instances, so this
>      `uses:` reference will not resolve on GHES as-is. Until a GHES-hosted
>      copy of that reusable workflow exists, replace it with a self-contained
>      job on GHES (checkout, set up Python, `curl` the schema/validator from
>      `raw.githubusercontent.com`, then run it) — check with the LDT4SSC
>      consortium for the current recommended approach, and confirm with your
>      GitHub admin that Actions runners have outbound HTTPS access to
>      `raw.githubusercontent.com` if you go this route.
> 2. Edit [`pilot.yaml`](pilot.yaml) to describe your pilot.
> 3. Read [`updates/README.md`](updates/README.md) to understand the update format.
> 4. Copy one of the examples in `updates/_examples/` and adapt it to write your
>    first update.
> 5. Commit and push. The validation workflow will check that your update
>    conforms to the schema.
> 6. Register your repository URL with the LDT4SSC consortium so that it is
>    picked up by the aggregator. (See the LDT4SSC pilot onboarding package
>    for the current registration mechanism.)

---

` < change as necessary > `

This repository is the home of an **LDT4SSC pilot project**. It contains the
pilot's documentation, shared artefacts, and ongoing updates, and serves as the
canonical public record of the pilot's work within the LDT4SSC initiative.

This repository was created from the [LDT4SSC pilot template](https://github.com/ldt4ssc/pilot-template)
and follows the structure and conventions of the LDT4SSC pilot documentation
framework.

## What this repository is for

This repository is the **project repository** for this pilot within LDT4SSC.
It exists so that:

- The pilot has a **single canonical public location** for its work that is
  visible to the LDT4SSC community and to the wider public.
- The pilot's **updates, milestones, lessons learned, and shared assets** can
  be published in a structured form and aggregated by the Knowledge Hub and
  the LDT4SSC project website.
- The pilot **owns its own record** of its work, independently of any central
  project infrastructure. If LDT4SSC project infrastructure evolves or ends,
  the content in this repository remains intact, open, and accessible.
- Outputs produced by the pilot can be **preserved, cited, and reused** by
  others, now and in the future.

This repository is **the pilot's own**. The consortium maintains the template
and the aggregation infrastructure, but the content is owned, authored, and
controlled by the pilot.

## Repository structure

- [`pilot.yaml`](pilot.yaml) — core metadata describing this pilot (name,
  partners, work strand, focus areas). **Edit this first.**
- [`updates/`](updates/) — structured updates on the pilot's journey:
  milestones, lessons learned, general progress, and references to assets and
  events. See [`updates/README.md`](updates/README.md) for the format.
- [`docs/`](docs/) — general project documentation.
- [`assets/`](assets/) — references to shared artefacts contributed by this
  pilot to the LDT4SSC Assets and Services Repository.
- [`src/`](src/) — source code developed by the pilot, if shared here.
- [`data-models/`](data-models/) — pilot-specific data models or references
  to published data models.

## Licensing

Code in this repository is licensed under the Apache License 2.0. Content
and documentation are licensed under Creative Commons Attribution 4.0
International (CC BY 4.0) unless stated otherwise. See [`LICENSE`](LICENSE) for
details.

## About LDT4SSC

LDT4SSC (Local Digital Twins for Smart and Sustainable Communities) is a
project funded by the Digital Europe Programme under grant agreement number 101226211, developing an interconnected ecosystem of Local Digital Twins across Europe.

Learn more at the [LDT4SSC project website](https://ldt4ssc.eu/) and the
[LDT4SSC Knowledge Hub](https://knowledgehub.ldt4ssc.eu/).