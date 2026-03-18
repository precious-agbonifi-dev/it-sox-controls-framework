# IT SOX Controls Framework

A practical, ready-to-use IT SOX (Sarbanes-Oxley) controls library built from real-world public sector and enterprise experience. Includes control narratives, evidence templates, testing procedures, and audit-readiness checklists.

> Built by Precious Agbonifi — drawing on experience at MOPAC, GLA, Virgin Media O2, The British Library, and Queen Mary University of London.

---

## 📐 What's Included

```
it-sox-controls-framework/
├── controls/
│   ├── access-management/
│   │   ├── AC-01-user-provisioning.md
│   │   ├── AC-02-privileged-access.md
│   │   └── AC-03-access-reviews.md
│   ├── change-management/
│   │   ├── CM-01-change-control-process.md
│   │   └── CM-02-emergency-changes.md
│   ├── incident-management/
│   │   └── IM-01-incident-response.md
│   └── data-backup/
│       └── DB-01-backup-and-recovery.md
├── templates/
│   ├── evidence-request-list.xlsx
│   ├── control-testing-workpaper.xlsx
│   └── risk-control-matrix.xlsx
├── checklists/
│   ├── audit-readiness-checklist.md
│   └── quarterly-review-checklist.md
└── README.md
```

---

## 🔑 Key Control Domains

### 1. Access Management (AC)

The highest-risk area in most SOX audits. Controls cover:

- **User provisioning & de-provisioning** — joiners, movers, leavers process
- **Privileged access management** — who has admin rights and why
- **Periodic access reviews** — quarterly certification of user access
- **Segregation of duties** — no single user can initiate AND approve transactions

**Sample Control Narrative — AC-01: User Provisioning**

```
Control Objective:
Ensure that access to financial systems is granted only to authorised
individuals, based on approved business need, and removed promptly upon
role change or termination.

Control Description:
HR triggers a provisioning workflow upon new hire or role change.
The line manager approves access via the ITSM portal. IT operations
provisions access within 2 business days. Access is logged and
reviewed quarterly by the system owner.

Frequency: Per event (onboarding/offboarding)
Control Type: Preventive
Evidence Required:
  - Approved access request tickets
  - HR notification emails
  - System access logs
  - Quarterly review sign-off
```

---

### 2. Change Management (CM)

**Sample Control Narrative — CM-01: Change Control**

```
Control Objective:
Ensure all changes to IT systems supporting financial reporting are
authorised, tested, and approved before deployment to production.

Control Description:
All changes are submitted via the Change Advisory Board (CAB) process.
Changes are classified (Standard, Normal, Emergency), tested in a
non-production environment, and approved by the CAB before deployment.
Post-implementation reviews are conducted for significant changes.

Frequency: Per change event
Control Type: Preventive & Detective
Evidence Required:
  - Change request tickets with approval chain
  - Test results / UAT sign-off
  - CAB meeting minutes
  - Deployment logs
```

---

## 📋 Audit Readiness Checklist

Use this 90 days before an audit:

- [ ] User access reviews completed and signed off for all in-scope systems
- [ ] Privileged access list reviewed and certified
- [ ] Terminated users removed from all systems within SLA
- [ ] Change tickets include approvals, test evidence, and rollback plans
- [ ] Backup logs reviewed and restoration tests documented
- [ ] Incident log reviewed — no unresolved critical incidents
- [ ] System owner attestations collected
- [ ] IT risk register updated and reviewed by management
- [ ] Vendor access reviewed and documented
- [ ] Data retention policy compliance verified

---

## 🗂️ Risk Control Matrix (Sample)

| Control ID | Domain | Risk | Control | Type | Frequency | Owner |
|---|---|---|---|---|---|---|
| AC-01 | Access Mgmt | Unauthorised access to financial systems | User provisioning process with manager approval | Preventive | Per event | IT Ops |
| AC-02 | Access Mgmt | Excessive privileges | Quarterly privileged access review | Detective | Quarterly | CISO |
| CM-01 | Change Mgmt | Unauthorised changes to prod | CAB approval required for all changes | Preventive | Per event | Change Mgr |
| DB-01 | Backup | Data loss / inability to recover | Daily backups with monthly restoration tests | Preventive | Daily | Infrastructure |

---

## 🤝 Contributing

This framework is open source. If you've worked through a SOX audit and have improvements, templates, or additional control narratives to add, PRs are welcome.

## 📄 License

MIT — free to use, adapt, and share with attribution.
