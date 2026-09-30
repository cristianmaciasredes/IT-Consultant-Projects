# Case Study: AI-Driven Knowledge Base Optimization for ServiceNow.

**Domain:** IT Service Management (ITSM), Knowledge Management, GenAI Integration. 

## Overview
As organizations migrate toward AI-driven ITSM platforms like ServiceNow's Now Assist, legacy knowledge bases often become a bottleneck. Traditional articles are frequently dense, poorly structured, and contain embedded media that Generative AI cannot process natively.

This repository demonstrates a prompt architecture methodology (GEM) designed to automate the transformation of legacy IT documentation into strict, KCS-compliant HTML modules. 

## The Challenge
*   **Unstructured Data:** Legacy articles lacking a standardized format cause poor AI summarization and hallucination.
*   **Media Blindness:** GenAI tools cannot "read" screenshots or videos, losing critical step-by-step context.
*   **HTML Ingestion Constraints:** ServiceNow requires specific HTML structures to ingest and map fields correctly (Case Description, Cause, Environment, Resolution, MetaData).

## The Solution: GEM Prompt Methodology
A specialized prompt architecture is utilized to act as a technical writing assistant. It processes chaotic source text and outputs clean, actionable data. 
*   **View the Prompt Architecture:** [gem_instructions.md](./gem_instructions.md)

**Key Capabilities:**
1.  **KCS Enforcement:** Forces the output into strict Knowledge-Centered Service methodology.
2.  **Media Translation:** Automatically generates contextual text descriptions for `<image>` and `<video>` tags without breaking the native ServiceNow attachment URLs (`/sys_attachment.do`).
3.  **Clean HTML Segmentation:** Outputs distinct code blocks ready for direct database ingestion.

## Impact Demonstration (Before & After)

To illustrate the effectiveness of this methodology, below is a comparison of a standard legacy article versus its AI-optimized counterpart.

*   **[Before Optimization (Legacy Article):](./articulo_original.md)** Dense, unstructured text, heavy reliance on inline images without alt-text, poor readability.
*   **[After Optimization (Now Assist-Ready):](./articulo_optimizado.md)** Structured HTML modules, actionable steps `<ol>`, synthesized media descriptions, and clean metadata.

---
*Disclaimer: All data in these examples has been fully anonymized and generalized to protect confidentiality. The methodology reflects industry best practices.*
