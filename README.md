# TORAM Provenance

**Intelligent Financial Market Provenance Infrastructure**

TORAM is building the infrastructure that makes a financial decision traceable from market reality to financial action.

> Markets are democratized. Trustworthy financial intelligence infrastructure is not.

## Category thesis

TORAM defines **Intelligent Financial Market Provenance Infrastructure** as the verifiable chain:

`Market → State → Intelligence → Decision → Authority → Execution → Outcome`

The public site explains the problem, category, reference architecture and company vision without exposing proprietary quantitative implementation.

## Technology

The site is deliberately static and lightweight:

- semantic HTML;
- Tailwind CSS v4, compiled at deploy time;
- GitHub Pages;
- GitHub Actions deployment;
- no client-side framework or analytics dependency.

The workflow builds a minimal `_site` artifact containing only the public HTML pages and minified Tailwind CSS.

## Public disclosure boundary

Safe to discuss publicly:

- the structural market-access problem;
- the provenance category and company vision;
- high-level Data Authority / Decision Authority / Execution Authority separation;
- the existence of the NIFTY 50 reference implementation;
- founder background;
- sourced public-market statistics.

Do not publish here:

- Chapter 21 formulas, weights, thresholds or calibration;
- proprietary feature definitions that reveal implementation;
- raw decision-audit datasets;
- credentials, infrastructure addresses or secrets;
- internal repositories or source code;
- unsupported or extrapolated performance claims.

## Deployment

Deployment is handled by `.github/workflows/deploy-pages.yml`.

For first-time GitHub Pages activation, set:

**Settings → Pages → Build and deployment → Source → GitHub Actions**

Then run or re-run the **Deploy TORAM Provenance** workflow.

## Public purpose

This repository is informational. It is not investment advice, a brokerage service, an offer of securities, or a claim of future performance.
