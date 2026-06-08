

### Goals
- **One consistent folder template** across all Sections and Section Working Groups (WGs) with two levels.
- **No loss of access rights** during/after restructuring.
- **Clear governance** (who creates folders, who grants access, how changes are requested)
- **Clear communication**
- **Solid timeline**

---

## Action Plan

## 1) Standard folder structure (template + naming rules)

### A. Design principles
- **Same top-level layout** for every working group. - Erste zwei Ebenen auf Sektionsebene gleich! Section ELSA /
- **Few top folders** (avoid deep nesting).
- **Separate “work in progress” vs “published/final.”**
- **Standard metadata in names** so files can be searched without opening.

### B. Proposed working group template
Example (adapt names to your org language):

- `01_Admin` (membership, onboarding, contacts, policies)
- `02_Planning` (roadmaps, calendars, meeting agendas)
- `03_Projects` (active work; project subfolders)
- `04_Meetings` (minutes, decision log)
- `05_Deliverables` (final outputs, publications)
- `06_Resources` (templates, reference, assets)
- `99_Archive` (read-only; by year)

Inside `03_Projects`, enforce a mini-template per project:
- `01_Brief`
- `02_Working_Docs`
- `03_Data`
- `04_Outputs`
- `99_Archive`

### C. Naming conventions (minimum viable standard)
- Folder names: `NN_Topic` (two-digit order keeps consistent sorting).
- Documents: `YYYY-MM-DD Topic – WG – vX` (or “FINAL”).
- Decisions: `DEC-### ShortTitle` with a decision log in `04_Meetings`.

Deliverables: publish-only folder + strict “final” naming.

**Deliverable of this step:** a 1–2 page “Drive Information Architecture Standard” + example tree.

---

## 2) Access rights management (audit + “future-proof” model)

### A. Target permission model (recommended)
- Use **Google Groups** (mailing lists) for Drive permissions, not individuals:
  - `wg-<name>-owners` (can manage, structure, permissions)
  - `wg-<name>-editors` (edit working docs)
  - `wg-<name>-viewers` (read-only)
  - Optional: `wg-<name>-external` (if external partners exist)
- Apply permissions **at the working group root**, keep exceptions rare and documented.

### B. Audit approach (before moving anything)
For each working group:
- Identify **root folder(s)** used today.
- Export/record:
  - direct shares (users)
  - group shares
  - link-sharing settings
  - external domains/users
- Flag “high risk” items:
  - sensitive data
  - externally shared files
  - shared drives vs “My Drive” ownership issues

### C. Restructuring strategy that preserves rights
- Prefer **move within the same Drive container** (e.g., within a Shared Drive) to preserve permissions.
- If moving across boundaries (My Drive → Shared Drive), permissions/ownership can change: plan controlled migration steps.
- Freeze changes during cutover window (short, scheduled).

**Deliverable of this step:** an “Access Rights Blueprint” + per-WG permission map.

---

## 3) Communication plan (stakeholder + cadence)

### Stakeholders
- Working group leads (decision + escalation)
- Members (end users)
- Admins (Drive / Google Workspace)
- Security / compliance (if applicable)

### Channels + rhythm
- Announcement email (why, what, timeline, what changes for them)
- Biweekly status update (mailing list)
- Dedicated Q&A doc (Google Doc) + office hours
- One meeting with leads:
  - confirm template
  - confirm access groups
  - identify special cases

### Key messages to include
- What will remain the same (Docs/Sheets/Slides, links where possible).
- What will change (folder locations, naming, where to store new content).
- How access is handled (group-based permissions, request process).
- How to report issues (single intake channel).

---

## 4) Implementation timeline (practical milestones)

### Recommended structure (example: 6–10 weeks)
1. **Week 1–2: Discovery**
   - Inventory all working group roots and structures
   - Access audit + special cases
2. **Week 2–3: Design**
   - Finalize template + naming + permission groups
   - Pilot plan
3. **Week 3–5: Pilot (2–3 working groups)**
   - Restructure + validate permissions + collect feedback
4. **Week 5–8: Rollout**
   - Batch by batch (e.g., 5–10 groups/week)
5. **Week 8–10: Stabilization**
   - Fix broken shortcuts/links (where applicable)
   - Clean up duplicates, finalize archive rules

### Task allocation (RACI-style)
- **Project Owner:** scope/decisions
- **Drive Admin:** group permissions, shared drives, policies
- **WG Lead:** validates structure + special cases
- **Migration/Restructure Operator:** executes moves, cleanups
- **Comms Lead:** emails, meetings, training
- **Security/Compliance:** approves retention/external sharing rules

**Deliverable of this step:** a tracking sheet per WG: status, owner, risks, completion checklist.

---

# Phase 2 — Evaluate and (Optionally) Migrate to NextCloud

## 1) Evaluate NextCloud (requirements-driven)
Define requirements first (not tool-first), e.g.:
- Data location/sovereignty, encryption, audit logs
- Collaboration needs: real-time co-editing, comments, versioning
- Identity management: SSO, group sync, MFA
- External sharing controls (expiring links, passwords)
- Search, retention, legal hold, backups
- Mobile usability and offline access
- Admin effort (patching, monitoring, storage scaling)

**Critical point:** NextCloud alone does not equal Google Docs collaboration. Real-time editing typically requires integration (e.g., **Collabora Online** or **OnlyOffice**) and must be tested with your user base.

**Deliverable:** a scored comparison matrix + go/no-go criteria.

---

## 2) Migration strategy (if go decision)
- Build NextCloud target structure first (same template as Drive).
- Decide migration unit: per working group vs per shared drive.
- Plan “content types” handling:
  - Google Docs/Sheets/Slides need conversion (to Office formats) or alternative editing approach.
  - Keep originals? Export both PDF (for archival) + editable format (DOCX/XLSX/PPTX) if needed.
- Pilot with one working group end-to-end before scaling.

**Deliverable:** migration runbook + pilot report.

---

## 3) Access rights transfer
- Map Google Groups → NextCloud groups/roles.
- Define role model in NextCloud:
  - owners/admins
  - editors
  - viewers
  - external collaborators
- Validate permissions with a sample set:
  - internal member can edit correct folders
  - viewer cannot edit
  - external links behave as intended
  - audit trail works

**Deliverable:** access mapping table + test protocol + sign-off.

---

## 4) Communication and training
- Decision announcement: why NextCloud, what changes, timeline
- Role-based training:
  - end users (upload, share, edit, versioning)
  - WG owners (permissions, folder creation)
  - admins (support, recovery, retention)
- Create “how-to” quick guides + FAQ + migration support channel

---

## 5) Migration timeline (example: 3–6 months depending on volume)
1. Requirements + vendor/hosting decision
2. Technical setup (SSO, storage, backups, monitoring)
3. Pilot migration + training
4. Wave migrations + support
5. Cutover + freeze window + validation
6. Decommission or archive Google Drive (policy decision)

---

# Pros/Cons + Chances/Dangers (Risk Evaluation)

## Option A — Restructure and stay on Google Drive

### Pros
- Minimal disruption; users already know the tools.
- Best-in-class real-time collaboration for Docs/Sheets/Slides.
- Lower operational overhead (Google manages infrastructure).
- Existing sharing workflows and external collaboration are mature.

### Cons
- Data sovereignty may be limited (depends on contract/region and org requirements).
- Vendor lock-in (Docs formats, ecosystem dependency).
- Permission sprawl risk if not governed (link sharing, ad-hoc shares).

### Chances (Upside)
- Fast standardization across 300+ users.
- Immediate security improvements via group-based permissions.
- Better findability, onboarding, and reduced duplication.

### Dangers/Risks (and mitigations)
- **Broken links / confusion:** mitigate with redirects via shortcuts, comms, cutover windows.
- **Permission leakage:** mitigate with audit, group-based model, restrict “anyone with link”.
- **Shadow drives / parallel structures:** mitigate with governance + periodic audits + clear “where to store what”.

---

## Option B — Migrate to NextCloud

### Pros
- Stronger path to **data sovereignty** (self-host/sovereign hoster, clearer data residency).
- High configurability (retention, encryption options, integration flexibility).
- Potentially better alignment with internal compliance policies.

### Cons
- Collaboration experience may be weaker unless Collabora/OnlyOffice matches your needs.
- Higher admin/ops effort (updates, scaling, performance, backups, incident handling).
- Conversion away from Google-native docs can cause fidelity loss and workflow changes.

### Chances (Upside)
- Reduced dependency on a single hyperscaler.
- Better control over sharing, retention, and auditing (depending on setup).
- Potential long-term cost/control benefits (case-dependent).

### Dangers/Risks (and mitigations)
- **User adoption risk:** mitigate with pilots, champions, training, phased rollout.
- **Loss of Google Docs features:** mitigate by validating Collabora/OnlyOffice workflows early; define “must-have” features.
- **Migration complexity & data loss:** mitigate with pilot migrations, checksums/export logs, dual-run period.
- **Performance/support burden:** mitigate with professional hosting/managed NextCloud + SLAs + monitoring.

---

# Final Deliverables (What “Done” Looks Like)

## If you stay on Google Drive
- Signed-off folder template + naming standard
- Google Groups-based permission model deployed for every WG
- All working groups migrated to the standard structure
- Governance: onboarding/offboarding process + quarterly permission audit
- Documentation: “How we use Drive” guide + escalation/support route

## If you migrate to NextCloud
- Completed requirements & scoring matrix + decision record
- NextCloud configured (SSO, groups, backups, monitoring, editing suite)
- Pilot validated (docs conversion, collaboration, permissions)
- Wave migration completed + training delivered
- Google Drive decommission/archival policy executed

---

## To tailor this into a ready-to-run plan, I need 6 inputs
1. Are you using **Shared Drives** or mostly **My Drive** folders today?
2. Do working groups include **external collaborators** (outside your domain)?
3. Any compliance constraints (data residency, retention periods, ISO/GDPR specifics)?
4. Approx. total data volume + number of top-level working groups?
5. Is real-time co-authoring **non-negotiable** for most teams?
6. Do you have (or want) **SSO/IdP** (e.g., Azure AD/Entra, Keycloak) for NextCloud?

If you answer these, I can produce a concrete timeline (with durations), a folder template adapted to your org, and a permissions/governance blueprint that’s implementable with minimal disruption.