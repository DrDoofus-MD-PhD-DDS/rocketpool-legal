# Internal Memo: A Committee-First Legal Service Layer for Rocket Pool pDAO Work

**Status:** Canonical integrated memo derived from the structured docs  
**Audience:** pDAO committee members, contributors, delegates, core team liaisons, and legal/tax counsel  
**Purpose:** Explain why the pDAO may want a narrow legal service layer for committee and administrative work, without creating a central board, management company, or legal wrapper for the entire pDAO.

## 1. Summary

Rocket Pool's pDAO currently has people doing real work on behalf of the protocol, but it does not have a clean legal service layer for that work.

The pDAO can approve budgets, elect committees, and make governance decisions. But the pDAO itself is not a legal entity. That means it cannot easily sign contracts, hold insurance, open ordinary accounts, accept third-party funds, hire vendors, or provide clear liability protection to the people carrying out pDAO-approved tasks.

This memo explores a narrow solution: a committee-first legal structure, possibly a DUNA or another low-overhead U.S. entity, that exists only to support pDAO-approved committee and administrative work.

The goal is not to create DAO leadership. The goal is to create a safe way for people to do work.

## 2. What We Are Not Trying to Do

This project should not be framed as “wrapping the pDAO” or “creating management for the DAO.”

For now, the preferred approach is not to create a legal entity that claims to represent all RPL stakers, control Rocket Pool governance, manage the protocol, own the treasury, or direct tokenomics.

The pDAO should remain the governance layer. The legal structure, if created, should be a service and execution layer. It should help committees and contributors carry out approved functions, but it should not become the pDAO's board, officer group, management company, or central decision-maker.

## 3. The Practical Problem

Several pDAO-related bodies and roles already perform useful work.

The GMC receives RPL from the pDAO treasury and funds grants that help the protocol. The IMC funds incentives for rETH and RPL liquidity and integrations. RPIP Editors help administer the RPIP process. The pDAO Treasurer executes approved transfers and related treasury tasks. The GMC Admin provides administrative support. The Security Council can act in emergencies. Future administrative or coordination roles may need to work with vendors, marketing teams, service providers, or third-party protocols.

These roles are useful, but they sit in an awkward legal position. People may be asked to approve spending, negotiate with vendors, interact with third parties, manage incentives, or handle funds without the basic legal tools that normal organizations use.

The current setup makes simple things harder than they need to be. For example, it is difficult to sign a vendor contract, hold an insurance policy, accept third-party incentive funding, pay a service provider cleanly, or indemnify a committee member for work done in good faith.

A legal service layer could solve some of these operational problems without changing who governs Rocket Pool.

## 4. The Risk We Are Trying to Reduce

One concern is that plaintiffs or regulators may argue that an unwrapped DAO, committee, or group of governance participants is an unincorporated association or general partnership. If that theory succeeds, individual participants could face personal exposure for actions they understood as DAO or committee work.

This does not mean every pDAO voter is automatically liable for everything. The law is unsettled, fact-specific, and jurisdiction-dependent. But DAO liability theories have been tested in U.S. courts, and they should be taken seriously.

The highest practical risk is probably not ordinary passive pDAO voting. The higher-risk category is visible, repeated, operational work: approving grants, negotiating with third parties, administering funds, executing transactions, managing incentives, and making emergency decisions.

That is why a committee-first structure makes sense. It focuses protection where people are actually doing work.

## 5. Preferred Direction: One Shared Service Layer

Earlier discussions considered separate legal entities for each committee. That may be clean on paper, but it is probably too much overhead for Rocket Pool.

A single shared service layer is likely more practical. It could support the GMC, IMC, RPIP Editors, Treasurer, administrative support roles, Security Council, and future pDAO-approved administrative functions. The structure would need clear internal separation between roles, but it would avoid the cost and volunteer burden of maintaining separate entities for each committee.

The service layer should be boring, narrow, and practical.

It should be able to do things like:

- hold an insurance policy;
- sign vendor contracts;
- pay contributors, vendors, and administrators;
- administer committee budgets;
- receive pDAO-approved funding;
- receive restricted or pass-through third-party incentive funding when appropriate;
- convert volatile assets to stable assets for budgeting;
- indemnify covered participants for good-faith work within scope;
- document role separation and conflicts policies.

It should not control the protocol, direct the pDAO, or become the place where tokenomics policy is made.

## 6. Why a DUNA May Be a Good Fit

A DUNA, or Decentralized Unincorporated Nonprofit Association, may fit this problem because it is designed for decentralized groups that need legal existence without equity ownership or profit distribution.

A DUNA is nonprofit, but that does not necessarily mean it is a charity. The important point is that the entity should not exist to distribute profits to members. Reasonable compensation for actual work can be different from a profit distribution.

For Rocket Pool, the DUNA model may be attractive if it can provide:

- limited liability protection for covered participants;
- role-based coverage for elected or appointed committee members;
- support for pseudonymous participation;
- low setup and maintenance cost;
- no equity or ownership interests;
- the ability to contract, hold insurance, and pay vendors;
- a clear separation between pDAO governance and committee execution.

The key question for counsel is whether a DUNA can protect people based on their pDAO-recognized committee role without forcing every covered person to sign legal membership paperwork or publicly disclose their identity.

## 7. DUNA Scope

The DUNA, if used, should have a narrow purpose.

A possible purpose statement:

> The organization exists to provide administrative, contractual, insurance, indemnification, treasury-support, and execution services for pDAO-approved Rocket Pool committee and contributor functions. It does not govern the Rocket Pool protocol, represent RPL holders as a class, control protocol tokenomics, or act as the management body of the pDAO.

This distinction is important. The DUNA should not be the pDAO. It should not claim to speak for all RPL stakers. It should not be described as a board, management committee, or leadership council.

It is a service layer.

## 8. Role-Based Coverage and Pseudonymity

One design goal is for protection to follow the pDAO-recognized role rather than the individual's public identity.

Possible rule:

> A covered participant is any person or wallet/handle holder who is duly elected, appointed, or authorized to perform a covered pDAO committee or administrative role under approved pDAO governance processes, while acting within the scope of that role.

This does not mean nobody is ever identified. A realistic structure may still require an identified organizer, registered agent, tax responsible person, bank signer, or counsel-facing representative. The goal is more modest: ordinary committee members should not have to publicly dox themselves merely to receive basic protection for approved work, if counsel confirms that a role-based structure is workable.

## 9. Tokenomics Firewall

Many committee members may also be Rocket Pool node operators, RPL stakers, or pDAO voters. That overlap should not automatically disqualify them from protection. People can wear different hats.

However, the DUNA itself should not act for the purpose of increasing RPL value or increasing RPL staking rewards.

The DUNA should not officially initiate, sponsor, recommend, or advocate tokenomics changes whose primary purpose is to increase economic returns to RPL holders or RPL stakers. Examples include increasing voter_share, creating or increasing RPL burns, or reframing protocol decisions around holder value.

That does not mean DUNA-covered people lose their personal governance rights. A committee member should still be able to vote in the pDAO, write an RPIP in a personal capacity, or speak as an individual community member. The key is that the person must not present that tokenomics advocacy as an official DUNA action or official committee-service-layer position.

RPIP Editors are a special case. They may process, format, review, and move RPIPs neutrally, including RPIPs that involve tokenomics. That procedural work should not be treated as official advocacy if the editors do not endorse the substance in their editor role.

## 10. Third-Party Funds and Incentives

Third-party funds may be useful for IMC incentives or future ecosystem programs, but they are a special risk category.

The service layer should avoid looking like a revenue-generating business-development company, broker, promoter, or seller of governance influence.

A lower-risk model would treat third-party funds as restricted or pass-through program funding for pDAO-approved incentive work. Funds should be documented, separately accounted for, not distributed as profits, and not conditioned on a promised governance outcome.

Higher-risk arrangements include commissions, success fees, undisclosed side payments, recurring business-development revenue, or payments conditioned on advocacy for a vote or integration.

This area needs legal and tax review before any final design.

## 11. Tax Questions

The tax issues are important and should be treated as open questions for tax counsel, not settled conclusions.

Questions include:

- How is pDAO treasury RPL inflation treated before it is allocated?
- Is a transfer from the pDAO treasury to a committee Safe income to anyone?
- Does the answer change if the Safe is controlled by an unincorporated committee, a DUNA, an LLC, or another entity?
- What is the tax treatment when a DUNA receives RPL?
- What happens when a DUNA sells or swaps RPL for USDC?
- Are committee stipends paid in RPL compensation income at fair market value when received?
- What reporting is required for payments to U.S. and non-U.S. contributors?
- How should third-party protocol incentives paid to the IMC or DUNA be characterized?
- Could recurring third-party incentive activity create unrelated business income, trade or business income, sales tax, information reporting, or other obligations?

A conservative working assumption is that payments to individuals for services are taxable to those individuals, whether paid in fiat, USDC, ETH, or RPL. Asset conversions by an entity may also create accounting and tax consequences. The exact treatment depends on the entity, facts, accounting method, jurisdiction, and role of the recipient.

## 12. Language Guide

The words used to describe this structure matter.

Prefer:

- service layer;
- execution layer;
- administrative support;
- committee support entity;
- pDAO-approved work;
- covered role;
- neutral process support;
- indemnification for good-faith work within scope.

Avoid:

- board of the DAO;
- DAO management;
- directors of the pDAO;
- officers of the pDAO;
- controlling members;
- representatives of all RPL holders;
- managing token holder value;
- maximizing RPL value;
- protocol leadership.

The core message should be simple:

> We are not creating leadership. We are creating a safe way for people to do work.

## 13. Practical Recommendation

The next step should not be a final governance vote. The next step should be a scoped legal review.

The pDAO should ask counsel to evaluate a narrow service-layer structure for committee and administrative work. The review should assume that the pDAO itself remains unwrapped for now, and that the service entity does not govern Rocket Pool or represent token holders.

If counsel confirms that a DUNA or similar U.S. structure can provide meaningful protection with low overhead, the pDAO can then consider a narrowly drafted proposal authorizing setup, budget, scope, and operating constraints.

The intended outcome is modest: give people doing approved work a safer and cleaner way to do that work.

---

This memo is part of the canonical `docs/` set, but it is still a working research document. It does not constitute legal or tax advice.
