# Review Regression Lab

A small, interactive concept demo for comparing two versions of an AI-assisted marketing review against the same set of examples.

**This is an independent concept prototype. It is not affiliated with Luthor and does not connect to or evaluate Luthor's product. All cases, labels, and review outputs are fictional and illustrative. This is not compliance or legal advice.**

## Why we built it

Luthor's product reviews marketing assets for issues such as unsupported claims, missing disclosures, brand-policy conflicts, and sensitive information. When a review model, prompt, or policy changes, teams need to understand how its decisions changed before relying on the update.

Luthor has written publicly about testing known examples, measuring what an AI reviewer catches or misses, and repeating those checks after changes. This demo makes that workflow tangible: it runs a fixed, human-labeled sample set through two simulated review versions and makes the differences easy to inspect.

The point is to show a possible evaluation workflow and invite feedback. It does not claim that Luthor lacks this capability or that these sample results reflect its systems.

## What the demo does

- Shows 12 fictional marketing-review examples with expected human-labeled outcomes.
- Compares simulated baseline and candidate decisions against those expected outcomes.
- Summarizes risk detection, false alarms, and overall agreement.
- Filters the examples to show disagreements, candidate misses, and candidate false alarms.
- Shows the content, expected result, and both review outputs when an example is selected.
- Exports the fictional test cases as JSON.

The examples include a projection missing context, a disclosure lost in a crop, an unsupported testimonial, a sensitive-looking number, and benign content that should pass. The scores are static, authored demonstration values; no model is run when you click **Run comparison**.

## Open it

No install or build step is needed. Open `index.html` in a browser.

The demo is a single self-contained HTML file. It makes no network requests and uses no external services.

## Sources and context

- [Luthor: Human-in-the-Loop Is Not Enough for AI Marketing Review](https://www.luthor.ai/blog/human-in-the-loop-ai-marketing-review-controls) discusses testing known compliant and non-compliant examples, monitoring misses, and rerunning tests after model, prompt, or policy changes.
- [Luthor](https://www.luthor.ai/) describes its marketing compliance review platform and audit trail.

These links explain the public context for the concept. They do not imply Luthor reviewed or endorsed this prototype.

## Limitations

- The test cases and expected outcomes are fictional and have not been validated by compliance professionals.
- Baseline and candidate results are simulated fixtures, not outputs from Luthor or another model.
- The displayed metrics illustrate comparison mechanics only; they are not evidence of model quality, safety, or regulatory compliance.
- A production evaluation would need an authorized dataset, qualified human labels, and actual model or policy versions.
