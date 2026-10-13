# SOC Investigations

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026 (Asia/Calcutta)  
**Documentation status:** Completed

This workspace contains 19 case narratives and 50 screenshots, organized by platforms, analysis categories, case reports, and evidence. Jayanth K completed the documentation organization, navigation, captions, indexes, and file/link checks. Personal live-lab execution has not been independently verified in this workspace.

## Platforms

| Platform | Case documents | Index |
|---|---|---|
| LetsDefend | 14 | [Complete case index](LetsDefend/README.md) |
| TryHackMe | 5 | [Complete case index](TryHackMe/README.md) |

## How to review a case

1. Open its README for the case overview and navigation.
2. Read `analyst-note.md` for the existing case note.
3. Open `reports/investigation.md` for the narrative and captioned images.
4. Review `evidence-index.md` for image hashes and missing proof-of-work fields.

## Evidence status

Personal execution logs, screenshot capture provenance, and actual execution dates are **Not recorded** in the case evidence indexes. Documentation checks confirm organization and file/link integrity, not independent verification of the investigation findings. The documentation update date is separate from retained event timestamps. See [the evidence requirements](EVIDENCE-STATUS.md).

## Repository overview

```text
SOC-Investigations/
├── README.md
├── ACTION-REQUIRED.md
├── EVIDENCE-STATUS.md
├── LetsDefend/              # 14 case document sets
│   ├── README.md
│   ├── malicious-file-analysis/
│   ├── malware-analysis/
│   ├── phishing-email-analysis/
│   └── web-attack-analysis/
├── TryHackMe/               # 5 case document sets
│   ├── README.md
│   └── phishing-email-analysis/
└── docs/
    ├── documentation-history.md
    ├── previous-index.md
    └── REPOSITORY-STRUCTURE.md
```

Each case contains `README.md`, `analyst-note.md`, `evidence-index.md`, `reports/investigation.md`, and `screenshots/`. See the [complete current file tree](docs/REPOSITORY-STRUCTURE.md).

## Reading screenshots

Every case README has an alert preview and a link directly to its report's screenshot section. Every report has quick navigation and full-resolution links beside its images. If technical text looks small, open the full-resolution image and click it to enlarge.

## Documentation conventions

[Documentation history](docs/documentation-history.md) · [Previous repository index](docs/previous-index.md)

- Platform names retain their official casing; category folders use lowercase kebab-case.
- Case folder names preserve unique case IDs, including both SOC104 event IDs.
- All detailed reports use `reports/investigation.md`.
- Screenshot filenames are lowercase and keep their actual PNG or JPEG format.
- All indexes and images use relative links.
- Unsupported fields are marked Not recorded.
