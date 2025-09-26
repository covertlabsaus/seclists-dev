+++
title = "Contribute New Wordlists to SecLists Properly"
description = "Follow the SecLists guidelines when submitting new wordlists."
draft = false
+++

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [{
    "@type": "Question",
    "@id": "https://seclists.dev/faq/seclists-contribute-wordlist",
    "name": "How do I contribute a new wordlist to SecLists correctly?",
    "acceptedAnswer": {
      "@type": "Answer",
      "text": "Follow the CONTRIBUTING.md rules: add the file under the correct train-case directory, update the folder README, credit the source, and submit a pull request with context."
    }
  }]
}
</script>

Maintainers expect consistent structure and attribution.

## Checklist
1. Choose the right folder (e.g., `Discovery/Web-Content`).
2. Name the file descriptively: `api-endpoints-2024.txt`.
3. Update the folder `README.md` with title, use case, source.
4. Run `git lfs track` if the file exceeds 100 MB (avoid when possible).
5. Open a PR summarising how the list was built and licensing confirmation.

## Diagram

```mermaid
flowchart LR
    A[New wordlist] --> B[Place in correct folder]
    B --> C[Document in README]
    C --> D[Pull request]
```

Respect privacy: scrub any PII before sharing wordlists publicly.
