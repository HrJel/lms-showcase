# Implementation notes — LMS

## Evidence ledger

- Bolek-OnlineCourses README explicitly calls this a runnable Django assignment scaffold.
- Source contains manage.py, course app, templates, requirements.txt, and optional Worker proxy.
- Source specifies Django 4.2 through below 5.2 in requirements.txt.

## Functional narrative

An online course and quiz/assessment demonstration, built around learners, instructors, lessons, questions and assessment results.

### Functional areas

- Course, lesson, learner and enrollment models
- Administrative management of learning records
- Question/choice submission and result feedback
- Local Django development workflow

## Implementation constraints

- Do not claim enterprise LMS maturity, payment support, mobile-native apps, or a production cloud deployment.
- Demo user details and grading content must be synthetic.

## What this repository implements

- Markdown documentation, project-level metadata, safe viewer mode classification and release checklists.
- **No actual application runtime**, private source tree, database schema, email transport, credentials or deployment wiring.
- **No real live preview** is wired without an approved separate demo endpoint.

## Mapping from source to public presentation

The source references have been read for high-level technical accuracy, but private repositories and URLs are intentionally **not** disclosed in this publication. Documentation is paraphrased and stripped of confidential configuration. Technical assumptions requiring full source review remain marked as unverified.

## Upgrade path

1. Verify exact product and canonical source/version with the rights holder.
2. Inventory features that may safely be demonstrated.
3. Capture anonymized screenshots and create fake-data demo fixtures.
4. Independently test each indicated platform.
5. Update `portfolio.json` only after a reviewer approves the published claim.
