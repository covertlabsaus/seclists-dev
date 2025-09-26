+++
title = "Use SecLists with ffuf for VHost Fuzzing"
description = "Combine SecLists wordlists with ffuf to brute-force virtual hosts."
draft = false
+++

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [{
    "@type": "Question",
    "@id": "https://seclists.dev/faq/seclists-ffuf-vhost",
    "name": "How do I fuzz virtual hosts with ffuf and SecLists?",
    "acceptedAnswer": {
      "@type": "Answer",
      "text": "Use ffuf -w SecLists/Discovery/DNS/namelist.txt -H 'Host: FUZZ.example.com' -u http://example.com to enumerate hidden vhosts."
    }
  }]
}
</script>

SecLists ships curated DNS and vhost lists ideal for `ffuf`.

## Command example

```bash
ffuf -w SecLists/Discovery/DNS/namelist.txt      -H "Host: FUZZ.example.com"      -u http://example.com      -fs 4242
```

- `-fs` filters 404-sized responses.
- `-mc` can match specific status codes.

## Diagram

```mermaid
flowchart LR
    A[SecLists namelist.txt] --> B[ffuf]
    B --> C[Target origin]
    C --> D[VHost responses]
```

Try `Seclists/Discovery/DNS/dns-Jhaddix.txt` for broader coverage, but adjust rate limits to avoid alerts.
