# code-sample

Sample e-commerce codebase used as the audit target for [Auditix](https://github.com/rtk5/Auditix) — a hybrid AI system that scans Python codebases for business policy violations.

## Structure

```
code-sample/
├── payment/
│   ├── abstract_models.py
│   └── utils.py
├── customer/
│   ├── abstract_models.py
│   └── utils.py
├── offer/
│   ├── abstract_models.py
│   └── utils.py
└── checkout/
    ├── session.py
    └── utils.py
```

## About

This repo contains Python modules simulating a real e-commerce backend — payment processing, customer data handling, discount logic, and checkout flows. Some functions intentionally violate business policies to serve as ground-truth test cases for the auditor.

When scanned by Auditix, this codebase produced **24 violations across 337 chunks** (93% compliance rate).

## Usage

Clone this repo and point Auditix at it to run a full compliance audit. See the [main repo](https://github.com/rtk5/Auditix) for setup instructions.
