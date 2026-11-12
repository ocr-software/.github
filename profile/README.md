# ocr-software.com: OCR API with word boxes, layout, tables and confidence

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ocr-software/.github/main/assets/banner-dark.svg">
  <img alt="OCR API returning each word with its box and confidence" src="https://raw.githubusercontent.com/ocr-software/.github/main/assets/banner-light.svg" width="100%">
</picture>

[ocr-software.com](https://ocr-software.com/) is an OCR API for PDFs and scans. You send a document and get back, for every page, the text, a box for every word, the layout, the tables and a confidence, so you see which words to check.

ocr-software.com is operated by Helm & Nagel GmbH, a company in Germany. The company is ISO/IEC 27001 certified; [proof and scope of the certificate](https://trust.helm-nagel.com/).

## What you get

- For each page the text, a box and a confidence for each word, the layout and table cells, depending on the pipeline you pick.
- Three pipelines, each pinned by `name@version`. `scan-ctc@2` returns the same bytes however a page is batched (300 of 300 test pages identical at batch size 1, 8 and 16, on the reference engine).
- `scan-ctc@2`: clean and scanned pages, a box and a confidence for every word.
- `scan-ctc-tables@2`: pages with tables, every cell with its row and column.
- `scan-vlm-ctc@2`: hard pages such as poor scans and fax, with the origin of every word.
- Output as JSON, plain text, Markdown, hOCR or a searchable PDF.
- The hosted API runs on a Hetzner server in Helsinki, Finland, EU. The uploaded document is deleted when the job ends, and the result stays retrievable for 24 hours.
- Run it on your own server: the [package](https://ocr-software.com/docs/install/) takes the same calls as the hosted API.

## Start here

- [OCR API with word bounding boxes: home page](https://ocr-software.com/)
- [Try OCR free on one of your pages](https://ocr-software.com/try/)
- [OCR API documentation](https://ocr-software.com/docs/) and the [curl guide for your first call](https://ocr-software.com/docs/api-guide/)
- [OCR pipelines: what each one returns](https://ocr-software.com/docs/pipelines/)
- [Output formats: JSON, Markdown, hOCR, searchable PDF](https://ocr-software.com/docs/formats/)
- [Gallery: watch test pages being read word by word](https://ocr-software.com/gallery/)
- [OCR API comparison: six things to check](https://ocr-software.com/blog/own-ocr-case-study/)
- [Pricing and offer](https://ocr-software.com/offer/pricing/)
- [History of OCR since 1913](https://ocr-software.com/about/)
- [Contact](https://ocr-software.com/contact/)
- [Guide for AI agents](https://ocr-software.com/docs/agents.md)

## Integrations

- [ocr-software-mcp](https://github.com/ocr-software/ocr-software-mcp): MCP server that lets Claude, Cursor and other agents read PDFs and scans through the API. A person picks the pipeline and confirms the quote before anything runs. Background: [OCR for AI agents (MCP)](https://ocr-software.com/integrations/mcp/).
- [nextcloud-ocr-software](https://github.com/ocr-software/nextcloud-ocr-software): OCR app for the Nextcloud Assistant and Flow (Nextcloud 33 to 35). Background: [OCR for Nextcloud](https://ocr-software.com/integrations/nextcloud/).

Both are MIT licensed.

## Provider and legal

The service is operated by Helm & Nagel GmbH. [Terms](https://ocr-software.com/legal/saas-terms/) · [Privacy](https://ocr-software.com/legal/privacy/) · [Imprint](https://ocr-software.com/legal/imprint/) · [Security](https://ocr-software.com/legal/security/)
