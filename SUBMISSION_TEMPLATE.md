# Partisia Blockchain Build Program - Submission Template

Thank you for your submission! Please fill in the sections below to ensure your project is reviewed accurately.

> **Important:** To submit your project:
>
> 1. Fill out this template
> 2. Submit your project through our [Monday Board](https://forms.monday.com/forms/a23209ca08d9c6b6cb9c08cb0a30466f?r=euc1)
> 3. Create a GitHub Issue in this repository with your progress updates

---

## 0. Legal Requirements

By submitting to this program, I confirm that:

- [x] I am over 18 years old or the age of majority in my jurisdiction of residence, or I am a business entity
- [ ] I am not a resident of, citizen of, or located in:
  - [ ] United States
  - [ ] Any geographic area subject to UN sanctions
  - [ ] Any geographic area subject to US sanctions
  - [ ] Any geographic area subject to EU sanctions
  - [ ] Any geographic area subject to Swiss sanctions
  - [ ] Any geographic area subject to any other sovereign country sanctions or embargoes

---

## 1. Project Information

- **Project Title:**
  _(TriviaParti)_
- **Project Tier:**
  - [ ] Beginner (Easy) – Reward up to $2,000
  - [x] Intermediate (Medium) – Reward $2,000–$4,000
  - [ ] Advanced (Hard) – Reward $4,000+
        _(Select the tier that best fits your project)_
- **Reward:**
  _($3000)_
- **Estimated Timeline:**
  _(2 weeks of active development across 6-week period)_
- **GitHub Repository Link:**
  _(https://github.com/nerds-cooking/partisia-trivia)_
- **Contact Info:**
  _(josh.robson@nerds.cooking)_
- **Team Members:**
  _(Jamie Bell - CTO)_
  _(Simon Gatenby - Tech Architect)_
  _(Josh Robson - Product Owner)_

---

## 2. Project Brief

Objective:
To build a fair, multiplayer trivia game where users submit answers privately. The goal is to prevent cheating and ensure a level playing field by keeping all submissions confidential until scoring.

Key Features:

- Private answer submission via MPC
- Public leaderboard without revealing answers
- Multi-game and multiplayer support
- Custom usernames mapped to wallet addresses
- Admin flow for inputting questions and answers
- All logic handled via a single smart contract

Use of Partisia MPC:

Player answers and the correct answer are secret-shared and evaluated via Partisia’s MPC layer. Scores are computed privately, and only the final result (correct/incorrect) is output on-chain.

Target Users:

DAOs, crypto-native communities, Web3 education platforms, and developers exploring privacy-preserving game mechanics.

Unique Value Proposition:

A true zero-leakage trivia engine powered by Partisia — no answer exposure, fully on-chain, and integrated Parti Wallet. We’ve shipped a full-stack MVP, not just isolated smart contract snippets.

---

## 3. Technical Description

### 3.1 Detailed Overview

_The application consists of a frontend interface (React + Vite) for player interaction, backed by a NestJS server handling API calls and user session logic. Trivia questions and answers are processed via smart contracts written in Rust, deployed on Partisia. All answer submissions are kept private using MPC. The contract commits a hash of the correct answer, and after the round, Partisia MPC nodes securely evaluate responses to calculate scores without revealing individual answers. The results are then aggregated and displayed on a public leaderboard. Role-based permissions are enforced for game organizers, and off-chain signature-based auth is used for secure API access._

### 3.2 Technical Approach

- **MPC Integration:** Secret score aggregation, privacy-enabled submissions
- **Core Functionality:** Private answer submission, MPC-based scoring, public leaderboard, question input, multiplayer support
- **Testing & Verification:** unit tests
- **Security Considerations:** Role based access control, Off-chain signature based authentication layer to dapp API
- **Performance Metrics:** none

### 3.3 Development Stack

- **Frontend:** _(React + Vite)
- **Backend:** _(NestJS)_
- **Smart Contracts:** _(Rust + Partisia)_
- **Other Tools:** _(Coffee)_

---

## 4. Deliverables

List all the deliverables included with your submission:

- Source code [(with clean commit history)](https://github.com/nerds-cooking/partisia-trivia)
- Comprehensive READM: https://github.com/nerds-cooking/partisia-trivia/blob/main/readme.md- 
- Demo: (https://www.loom.com/share/f87f3913fc2e441d84b887efe9a4cd58)
- Website link: (https://trivia.partisia.nerds.cooking/)
- Test: (https://github.com/nerds-cooking/partisia-trivia/blob/main/java-run-tests.sh)

---

## 5. Project Timeline

Start Date:
9 April 2025
Milestone 1:
Description: Smart contract design and implementation using Partisia (MPC integration, question/answer handling)
Target Date: 16 April 2025
Milestone 2:
Description: Frontend (React) and backend (NestJS) integration, leaderboard display, wallet username mapping
Target Date: 19 May 2025
Final Submission Date:
27 May 2025

Buffer Time:
Included ~3–4 weeks of buffer due to delays from unanswered support queries, testnet downtime and parallel work commitments. 

---

## 6. Additional Information
- **(Feedback Deck provided separately) **
---

## 7. Acknowledgment

By submitting this project, I confirm that:

- The work is my own or properly credited.
- I agree to release the project under an approved open-source license.
- I accept the evaluation rubric and community voting process.
- I will provide weekly progress updates through GitHub Issues in this repository.
- I understand that the project must be completed within the estimated timeline.
- I will actively engage with the community and respond to feedback.
- I understand that my project will be subject to community voting on [CrowdSnap](https://www.crowdsnap.ai/), which contributes 10% to the final evaluation score.

---

_Thank you for your submission! We look forward to reviewing your project and will be in touch with feedback._
