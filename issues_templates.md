# p2pHub — Complete Issue Set

This document contains all planned issues for building the peer-to-peer learning platform, p2pHub.  
Grouped by development phases.

---

## Phase 1 — MVP: Core Functionality

### [MVP] Create basic user authentication system

**Description:**  
Implement registration and login logic with default role `peer`. Use JWT or session-based login. No email confirmation required for now.

**Acceptance Criteria:**
- [ ] Registration form
- [ ] Secure login
- [ ] Password hashing (bcrypt)
- [ ] JWT/session setup

**Tags:** `auth` `backend` `security` `phase-1`

---

### [MVP] Implement user roles logic

**Description:**  
Add support for 4 roles: peer, curator, project creator, admin.

**Acceptance Criteria:**
- [ ] Role field in DB
- [ ] Permissions for different actions
- [ ] UI adapts to role

**Tags:** `roles` `backend` `auth` `phase-1`

---

### [MVP] Build project catalog UI

**Description:**  
Frontend interface for listing available projects.

**Acceptance Criteria:**
- [ ] Project card: title, XP, short desc, tag
- [ ] Grid/list toggle
- [ ] Search/filter stub

**Tags:** `frontend` `ui` `projects` `phase-1`

---

### [MVP] Create 3-review submission logic

**Description:**  
Each project requires 3 peer reviews before it’s accepted.

**Acceptance Criteria:**
- [ ] Track submitted reviews per project
- [ ] Block completion until 3 done
- [ ] XP = function of 3 reviews + test

**Tags:** `review` `backend` `logic` `phase-1`

---

### [MVP] Implement P2P Points system

**Description:**  
Each peer has P2P Points: 1 point = 1 review slot.

**Acceptance Criteria:**
- [ ] Initial balance = 5
- [ ] Spend 1 to submit project
- [ ] Earn 1 for reviewing

**Tags:** `gamification` `backend` `xp` `phase-1`

---

### [MVP] Review scheduling calendar

**Description:**  
Peers book review sessions via calendar. Reviewers offer time slots.

**Acceptance Criteria:**
- [ ] Reviewer sets availability
- [ ] Peer books slot
- [ ] Penalty for cancel <1h

**Tags:** `calendar` `scheduling` `frontend` `phase-1`

---

### [MVP] Minimal admin dashboard

**Description:**  
Admins can review new users, handle flags, and see submissions.

**Acceptance Criteria:**
- [ ] User approval flow
- [ ] Project moderation
- [ ] Flagged review list

**Tags:** `admin` `moderation` `dashboard` `phase-1`

---

### [MVP] Upload and link MVP PDF in /docs

**Description:**  
Upload official MVP document and link it in the README.

**Tags:** `documentation` `meta` `phase-1`

---

## Phase 2 — Expansion, Feedback, UX

### [Phase 2] Add review flag system

**Description:**  
Let reviewers tag peer submissions with quality flags.

**Acceptance Criteria:**
- [ ] Flags: `cheating`, `good code`, `bear service`
- [ ] Display in user history
- [ ] Affect XP

**Tags:** `review` `flags` `moderation` `phase-2`

---

### [Phase 2] Add one-time appeal system

**Description:**  
Allow peers to appeal a project once. Resolved by curator/admin.

**Acceptance Criteria:**
- [ ] Appeal request form
- [ ] Review by elevated role
- [ ] Final XP update

**Tags:** `appeals` `review` `logic` `phase-2`

---

### [Phase 2] Add multilingual UI and auto-translation

**Description:**  
UI should support switching languages and live translation in reviews.

**Tags:** `i18n` `frontend` `UX` `phase-2`

---

### [Phase 2] Add terminal time tracking

**Description:**  
Track time peer spends actively on project through embedded timer.

**Tags:** `tracking` `UX` `terminal` `phase-2`

---

### [Phase 2] Build skill radar + progress dashboard

**Description:**  
Graph showing % growth in categories based on projects completed.

**Tags:** `analytics` `dashboard` `frontend` `phase-2`

---

### [Phase 2] In-app chat system for peers/reviewers

**Description:**  
Messaging system between participants.

**Tags:** `chat` `messaging` `community` `phase-2`

---

## Phase 3 — Monetization, AI, Mobile

### [Phase 3] Project monetization system

**Description:**  
Enable creators to publish and sell access to their own projects.

**Tags:** `marketplace` `monetization` `phase-3`

---

### [Phase 3] AI-based review assistant

**Description:**  
Use GPT API to suggest feedback, detect review quality, or verify originality.

**Tags:** `AI` `review` `GPT` `phase-3`

---

### [Phase 3] Public learning marketplace

**Description:**  
Project explorer with public/private toggle and optional paid access.

**Tags:** `explorer` `marketplace` `frontend` `phase-3`

---

### [Phase 3] Discord integration bot

**Description:**  
Bot for notifications, review alerts, XP logs.

**Tags:** `integrations` `discord` `community` `phase-3`

---

### [Phase 3] Mobile app (React Native)

**Description:**  
Basic version of the platform for mobile usage.

**Tags:** `mobile` `frontend` `ux` `phase-3`

---
