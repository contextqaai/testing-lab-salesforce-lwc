# ContextQA lab — Salesforce · Lightning / LWC

Educational source fork of [trailheadapps/ebikes-lwc](https://github.com/trailheadapps/ebikes-lwc). Original history, notices and license are retained. This is not an endorsed integration or a customer production app.

**Status: source and exercises available. Public deployment, platform import and ContextQA run results are not verified.**

Starting source commit: `57c3b43e443802a0568283f996ad39c12ea74cda`.

## Setup and scope

Deploy only into an authorized scratch org, Developer Edition or suitable sandbox following upstream instructions. Configure permission sets and synthetic data. This app runs on Salesforce Platform and cannot be hosted as a complete Salesforce org on Cloud Run.

Follow the [original setup instructions](../README.md#upstream-project-documentation). See [stack/platform guidance](https://github.com/contextqaai/testing-lab/blob/main/PLATFORMS.md) for deployment boundaries.

## Exercises

| Scenario | Explicit assertion |
|---|---|
| Product search | A seeded product is returned by the intended search. |
| Filtering | The selected product filters produce the expected fixture subset. |
| Product detail | The detail matches the selected catalog product. |
| Reseller journey | The chosen supported reseller workflow produces its specified result. |
| Permission boundary | A separately configured restricted test user cannot perform the protected action chosen for the exercise. |

These are acceptance exercises, not claims that upstream currently satisfies each desired requirement. Inspect the implemented workflow and fixtures before generating executable steps. Missing validation/auth may deliberately demonstrate a failure and must be disclosed.

## End-to-end lesson

Start an owned/authorized copy with synthetic fixtures. State the assertion, create/review a test in your authenticated ContextQA workspace, execute, and inspect the actual verdict. Introduce one disclosed regression in a separate variant, rerun the same assertion, fix the app and rerun. Confirm mutations against disposable data. Keep credentials and private reports out of this repository.

Record app commit/build, fixture/scenario version, browser/runner version, environment and timestamp with every real report. A cached report is recorded evidence, not a new run. No ContextQA report has been generated for this fork yet.

[ContextQA setup](https://contextqa.com/tutorials/getting-started-with-contextqa-test-automation/) · [Central catalog](https://github.com/contextqaai/testing-lab)
