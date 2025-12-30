# Darfur Testimony Archive

## Purpose

The Darfur Testimony Archive is a public, structured, and verifiable digital repository dedicated to documenting incidents of sexual violence used as a tool of war in the Darfur conflict, Sudan. This archive aims to provide a permanent, citable record that transcends the ephemeral nature of news cycles, serving researchers, policymakers, journalists, and the public.

Our goal is to ensure that each documented incident is recorded with integrity, transparency, and a commitment to ethical reporting, independent of political agendas.

## Methodology & Verification

1. **Source Collection**: Incident reports are gathered from multiple independent sources, including:
   - Eyewitness testimonies
   - Reports from reputable NGOs (e.g., Amnesty International, Human Rights Watch)
   - United Nations documents (e.g., UN Security Council reports, OHCHR statements)
   - Verified journalistic investigations
   - Court records and legal filings where available

2. **Verification Tiers**:
   - **Tier 1**: Multiple independent, corroborating sources (e.g., NGO report + eyewitness + UN mention)
   - **Tier 2**: Two independent sources (e.g., NGO report + eyewitness)
   - **Tier 3**: Single source with high credibility (e.g., detailed UN document)
   - **Unverified**: Initial report awaiting further corroboration

3. **Redaction & Safety**: To protect the identities of survivors and witnesses, all personal identifiers (names, exact addresses, etc.) are redacted or omitted. Geographic details are generalized to the village/area level unless public records already disclose them.

## Repository Structure

```
darfur-testimony-archive/
├── README.md               # This file
├── cases/
│   ├── template.md        # Standard template for all incident reports
│   ├── 2023-10-26-abu-jabal.md  # Example case file (one per incident)
│   └── ...                # Future case files
└── .github/               # (Optional) Workflow automation files
```

### Case File Format

Each case is documented in a separate Markdown file inside the `cases/` directory, following the structure defined in `cases/template.md`. The template includes:

- **Incident ID**: A unique identifier (e.g., DT-2023-001)
- **Date(s) of Incident**: Approximate or exact date(s)
- **Location (Village/Area)**: General location, avoiding precise coordinates
- **Source(s)**: Citations of the sources used, with links where available
- **Verified Status**: Verification tier and brief rationale
- **Redacted Narrative**: A summary of the incident, with all identifying details removed

## Workflow for Adding New Cases

To maintain integrity and transparency, we employ a GitHub-based editorial workflow:

1. **Issue Tracking**: A new GitHub Issue is created for each potential incident, titled “New Case Report: [Village Name] – [Date]”. The issue is populated with the template and labeled with status labels (`source-verification`, `geolocation-needed`, `draft-report`, `ready-for-archival`).

2. **Branch & File Creation**: Once sufficient verification is gathered, a new branch is created (e.g., `case-village-name-2023-10-26`). A case file is added in the `cases/` directory following the template.

3. **Pull Request Review**: A Pull Request is opened to merge the branch into `main`. The PR description links to the original issue, summarizes the incident, and outlines the verification steps. This simulates an editorial review.

4. **Merge & Release**: After review, the PR is merged (preferably with a squash merge). Periodic GitHub Releases (e.g., `v1.0`, `v2.0`) create permanent, citable snapshots of the archive.

## Ethical Commitment

- **Survivor-Centered**: The safety and dignity of survivors is paramount. No identifying information is stored.
- **Impartiality**: Reports are based on verified facts, not political narratives.
- **Transparency**: Every change to the archive is logged via Git commits, and the entire workflow is public.
- **Collaboration**: We welcome contributions from journalists, researchers, and human-rights organizations, provided they adhere to the same verification standards.

## How to Cite This Archive

When referencing a specific case, cite the case file’s permanent URL (e.g., `https://github.com/britdev071809/darfur-testimony-archive/blob/main/cases/2023-10-26-abu-jabal.md`) and mention the archive’s version (e.g., “Darfur Testimony Archive, v1.0”).

For the archive as a whole, cite the GitHub repository URL and the latest release.

## License

The content of this archive is made available under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/), unless otherwise noted in specific case files.

## Contact

For inquiries about the archive, verification procedures, or potential collaborations, please open a GitHub Issue in this repository.

---

*This archive is maintained by independent journalists committed to documenting human-rights violations in Darfur. Last updated: October 2023.*