<!-- Google OCR Public README -->
<!-- Formatted following marklovestech GitHub repository layout -->

<div align="center">

# Google OCR

**A lightweight Google Cloud Vision OCR integration for automated document and menu text extraction.**

![platform](https://img.shields.io/badge/platform-Node.js-lightgrey)
![language](https://img.shields.io/badge/JavaScript-ES6%2B-yellow)
![api](https://img.shields.io/badge/API-Google%20Cloud%20Vision-blue)
![status](https://img.shields.io/badge/status-production--ready-brightgreen)

</div>

---

## What it does

Extracting clean, reliable text from physical documents, paper menus, and receipts is a fundamental building block for modern AI agents and document processing pipelines. Raw image uploads often suffer from uneven lighting, multi-column layouts, and unformatted text blocks.

Google OCR is a dedicated Node.js utility designed to interface seamlessly with the Google Cloud Vision API. It ingests image inputs, performs Optical Character Recognition (OCR), cleans up messy text streams, and produces structured text optimized for downstream LLM and NLP agent pipelines.

## Highlights

- **Optical Character Recognition.** Leverages Google Cloud Vision API for high-accuracy text detection across complex visual layouts.
- **Menu & Document Parsing.** Specialized text extraction tailored for multi-column restaurant menus, invoices, and physical documents.
- **Agent Tool Integration.** Native JSON schema integration designed for plug-and-play use in AI agent tool registries.
- **Resilient Preprocessing.** Built-in data formatting and error handling for noisy or rotated image inputs.

## Unique Feature: Agent-Ready Layout Sanitization

Raw OCR output from computer vision endpoints frequently breaks text into disconnected bounding boxes that confuse downstream LLMs. Google OCR incorporates a specialized text sanitizer that:

- Reconstructs spatial text relationships from multi-column restaurant menus and multi-page receipts.
- Normalizes irregular line wraps and whitespace artifacts into clean, semantic Markdown streams.
- Minimizes token overhead for downstream LLM prompts while maintaining 100% data fidelity.

## Tech Stack

| Layer | Technology |
|---|---|
| **Runtime** | Node.js (ES Modules) |
| **API Integration** | Google Cloud Vision API |
| **Parsing** | Custom Text & Layout Sanitizer |

## Why the source is private

This repo is a public-facing description of a working application. The full implementation lives in a private repository. If you are a collaborator, recruiter, or fellow builder who would like a deeper look into the codebase—please reach out below.

## Contact

**Gabriel Shyh** — [@gabrielshyh](https://github.com/gabrielshyh) · [gabrielsshyh2006@gmail.com](mailto:gabrielsshyh2006@gmail.com)