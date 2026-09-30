# Rocket Pool pDAO DUNA Memo

**Status:** working draft for discussion  
**Audience:** Rocket Pool pDAO participants, committee members, contributors, and possible legal/tax counsel  
**Main idea:** We are not creating leadership. We are trying to create a safe way for people to do work.

## 1. Why this memo exists

Rocket Pool has a lot of real work happening around the protocol, but the pDAO itself is not a legal entity. That is awkward.

The pDAO can vote. It can approve budgets. It can elect or recognize committees. It can decide what it wants. But it cannot easily do ordinary legal things that normal organizations do: sign a contract, hold insurance, accept third-party money cleanly, pay vendors through a recognized structure, or give clear legal protection to the people carrying out approved work.

Historically, our legal discussions jumped between many possible answers: personal LLCs, committee indemnification, Swiss Associations, Cayman foundations, DAO LLCs, DUNAs, MiDAO, BORG-style structures, and doing nothing. A lot of that research was useful, but it also became scattered and hard to act on.

This memo is an attempt to put the current thinking in one place. The goal is not to prove that a DUNA solves everything. The goal is to explain why a narrow DUNA-style service layer still looks like the best low-overhead candidate for Rocket Pool right now, and what questions need to be checked before anyone relies on it.

## 2. Where we came from

The original worry was broad: maybe the pDAO itself could be treated as a general partnership or unincorporated association. If that happened, visible participants might face personal liability for actions that they thought were just DAO governance.

That concern was not imaginary. DAO liability theories have been tested in U.S. litigation, including cases involving Ooki DAO, bZx DAO, Compound DAO, MakerDAO, Lido DAO, and related actors. These cases do not give a simple answer that every DAO voter is liable for everything. But they do show that plaintiffs are willing to argue that DAOs, DAO participants, tokenholders, delegates, founders, investors, or operational contributors can be responsible for DAO-related conduct.

The early reaction was to look at large protective structures. Could the whole pDAO be wrapped in a Cayman foundation? Could a Swiss Association own or represent something? Could every committee have its own entity? Could every individual form a personal LLC? Those ideas all had reasons behind them, but they also had serious practical problems.

A full pDAO wrapper is expensive, politically sensitive, and may create more centralization symbolism than it solves. It can raise hard questions about who the members are, who controls the entity, whether the entity represents all RPL stakers, what tax obligations it creates, and whether it accidentally becomes the legal “manager” of the protocol.

Committee-by-committee entities are cleaner in theory but probably too much bureaucracy. Rocket Pool does not have endless volunteers who want to maintain separate legal entities, bank accounts, filing calendars, insurance policies, and tax processes for each pDAO function.

Personal LLCs may help some individuals, but they do not solve the pDAO’s shared operating problem. They also put the burden on every contributor to form and maintain their own entity, which is unrealistic and unattractive for a pseudonymous volunteer culture.

Doing nothing is simple, but it leaves the same problem we started with: people are doing useful work without a clean legal service layer.

That is how the current preferred framing emerged: do not try to wrap the whole pDAO first. Start with the people and functions actually doing work.

## 3. The current preferred framing

For now, the pDAO probably should not try to wrap itself as a whole.

The better first target is a narrow legal service layer for pDAO-approved committee and administrative work. That service layer should not become the pDAO. It should not claim to represent all RPL holders. It should not control Rocket Pool governance or tokenomics. It should not become a central board.

It should exist to help people do approved work more safely and cleanly.

The simple version is:

- The **pDAO** remains the governance layer.
- The **committees and appointed roles** continue doing their defined work.
- The **legal service layer** provides protection, contracting ability, insurance, payment rails, and administrative support for that work.

This is why a DUNA is interesting. A DUNA is not obviously perfect, but it appears to be designed for exactly the kind of problem we have: a decentralized group that needs some legal existence, limited liability, and operating capacity without creating stockholders, owners, or a conventional company.

## 4. The current pDAO functions that matter

The relevant Rocket Pool pDAO functions include at least the following.

The **GMC**, or Grants Management Committee, receives RPL from the pDAO treasury by onchain vote and makes grants for work that helps the protocol. The pDAO can overturn GMC decisions.

The **IMC**, or Incentives Management Committee, receives RPL from the pDAO treasury and provides incentives to crypto protocols, DeFi protocols, liquidity pools, and exchanges for rETH/RPL usage and liquidity.

The **RPIP Editors** oversee the RPIP process. They generally do not create RPIPs themselves. Their role is closer to process administration than policy leadership.

The **pDAO Treasurer** executes approved transfers and related treasury tasks.

The **GMC Admin** provides administrative support and is paid in RPL.

The **Security Council** is a trusted group, including core team members, that can make emergency parameter changes if something dangerous or buggy happens.

There may also be a future administrative or coordination function. That role could coordinate vendor work, marketing teams, roadmap preparation, contracts, third-party incentives, and other business-like work, while still requiring pDAO approval for major decisions.

These are the places where the practical legal problem shows up. The risk is not just theoretical “DAO law.” It is that real people are approving grants, handling funds, interacting with third parties, coordinating work, or responding to emergencies without a clean legal wrapper for those actions.

## 5. What problem the service layer should solve

The pDAO currently lacks a legal service layer that can:

- sign contracts;
- hold insurance;
- accept or administer certain third-party funds or incentives;
- pay vendors cleanly;
- pay committee stipends or administrative compensation through a recognized structure;
- document conflicts and role boundaries;
- indemnify committee members for good-faith work within scope;
- act as a liability sink if a dispute arises from committee work.

The phrase “liability sink” is not magic. It does not mean nobody can ever sue individuals. It means that if a dispute arises from an approved committee function, there is at least an entity that was designed to be the responsible legal counterparty. That is better than forcing every question back onto an unwrapped DAO, a multisig, or random visible contributors.

This is especially important if the pDAO wants committees to do more than passively hold funds. The moment committees start signing vendor agreements, receiving third-party funds, coordinating external campaigns, or giving commitments to third parties, the lack of a legal service layer becomes a real limitation.

## 6. Why DUNA still looks like the best hope

A DUNA, or Decentralized Unincorporated Nonprofit Association, is currently the most interesting candidate because it seems to match several Rocket Pool constraints at once.

It is nonprofit, but not necessarily a charity. That matters. We are not talking about creating a public charity or a foundation with a charitable mission. We are talking about a nonprofit association that does not have equity owners and does not distribute profits to members.

That should still allow reasonable compensation for actual work. Committee stipends, admin pay, vendor payments, and contributor compensation should not be treated as profit distributions merely because they are paid by a nonprofit association. The key is that payments should be reasonable compensation for services or reimbursement/payment for actual work, not a way to distribute economic upside to members.

A DUNA may also support a role-based and pseudonymous structure better than a normal LLC. That is very important for Rocket Pool. The ideal is not to require every committee member to form a personal LLC, sign a legal membership agreement, or dox themselves just to receive some protection for a pDAO role.

The working hope is:

> Protection should follow the pDAO-recognized role, not the public identity of the person.

For example, if the pDAO elects someone to the GMC, or appoints someone as Treasurer, or recognizes someone as an RPIP Editor, the DUNA structure might define that role as a covered role. The person might be known by a handle, wallet address, or governance identity rather than a public legal name. There may still need to be one or more legally identified organizers, agents, or service providers behind the scenes, but the ordinary committee participant should not necessarily have to publicly dox to be covered.

That exact design needs legal review. But it is the right design target.

Compared with the alternatives, a DUNA-style structure appears to offer the best combination of:

- low overhead;
- no equity ownership;
- no profit distributions;
- compatibility with decentralized governance;
- possible protection for pseudonymous participants;
- ability to contract and hold insurance;
- ability to support multiple committees through one shared structure.

That is why DUNA still feels like the best hope.

## 7. Why not wrap the whole pDAO?

Wrapping the entire pDAO sounds clean until you start asking what it means.

Who are the members? Every RPL staker? Every voter? Every node operator? Every person who ever votes? Only active delegates? Only people who opt in? What about people who are pseudonymous? What about people in jurisdictions where participation in a legal entity creates tax or reporting consequences?

Who controls the wrapper? If the entity has directors, managers, officers, members, or a board, does that imply that those people control the protocol? If the wrapper signs something, is it signing for every RPL holder? If the wrapper owns something, is it holding it for the pDAO, the protocol, tokenholders, or itself?

Those questions are solvable in some contexts, but they are not cheap or simple. For Rocket Pool, they also risk sending the wrong cultural message. The pDAO is not trying to create a central company to manage the protocol.

The committee-first approach is more modest. It does not answer every possible DAO liability question. It does not make the pDAO a legal entity. It simply gives the people doing approved work a safer and cleaner way to do that work.

If the pDAO later becomes richer, more operationally complex, or more legally exposed, a broader wrapper can be reconsidered. But full pDAO wrapping should not be the first move.

## 8. One shared structure, not separate entities for every committee

Another question is whether each committee should have its own entity. The cleaner legal answer might be yes. The practical Rocket Pool answer is probably no.

Separate entities would mean separate paperwork, separate ownership or membership questions, separate filing calendars, possibly separate tax returns, separate insurance decisions, separate bank or exchange accounts, and separate leadership burdens.

Rocket Pool has limited money and limited volunteer energy. A structure that requires each committee to find its own legal maintainers will probably fail in practice.

The better target is one shared service layer with internal role separation. The DUNA or similar entity could support GMC, IMC, RPIP Editors, Treasurer, GMC Admin, Security Council, and future administrative functions under one umbrella. Each function can have its own scope and rules, but the entity overhead is shared.

That is not perfectly clean. But it is realistic.

## 9. What the DUNA should be allowed to do

The DUNA should be boring and practical. It should not be a think tank for tokenomics or a central planning office for Rocket Pool. It should help approved work happen.

Appropriate functions may include:

- administering pDAO-approved committee budgets;
- paying stipends, admins, contributors, and vendors;
- signing vendor or service contracts for approved work;
- holding insurance for covered roles and functions;
- indemnifying covered participants for good-faith work within scope;
- converting RPL to USDC or another stable asset for budgeting and volatility management;
- coordinating grants and incentive programs that have already been authorized by the pDAO or a covered committee process;
- supporting emergency/security functions where the pDAO has already approved the role;
- maintaining records, policies, and conflict disclosures.

The DUNA should be able to execute. It should not be able to govern the protocol on its own.

## 10. What the DUNA should avoid

The DUNA should avoid anything that makes it look like the manager of the DAO, the representative of all RPL holders, or a vehicle for increasing RPL holder value.

It should not:

- claim to be the pDAO;
- claim to represent all RPL holders or all node operators;
- take custody or ownership of the whole pDAO treasury;
- originate or officially recommend tokenomics changes designed to increase RPL value;
- advocate increasing voter_share or similar RPL staking rewards in its official capacity;
- promote RPL burns or other value-accrual mechanisms in its official capacity;
- receive ongoing protocol fees for the benefit of members;
- operate as a profit-seeking business development company;
- become the place where protocol strategy is centrally decided.

The short version: the DUNA can help people carry out work. It should not try to make number go up.

This is not because tokenomics discussion is bad. Tokenomics is a legitimate pDAO topic. But tokenomics advocacy should happen through ordinary pDAO governance, by individuals acting in their personal capacity, not through the official service-layer role of the DUNA.

## 11. The “different hats” problem

Committee members may also be node operators, RPL stakers, voters, delegates, grant recipients, contributors, or community advocates. That overlap is normal in a DAO.

The important distinction is role.

A person serving in a DUNA-covered committee role should not use that official role to advocate for tokenomics changes that increase their own RPL returns. But that same person should not lose their ordinary pDAO rights. They can still vote. They can still speak as individual community members. They can still write or support RPIPs in a personal capacity.

The clean rule is:

> DUNA-covered work should stay inside the service/execution role. Personal governance activity should be clearly personal.

RPIP Editors are a good example. An RPIP Editor may process an RPIP about voter_share, RPL burns, inflation, or other tokenomics questions. That is procedural work. It should not be treated as official advocacy if the editor is neutral in the editor role. But if that same person wants to argue for the proposal, they should do that as an individual pDAO participant, not as “the DUNA” or “the RPIP Editor function.”

This is basically a conflict and role-separation policy. It does not require people to stop being community members. It requires them to be clear about which hat they are wearing.

## 12. RPL, rETH, and securities uncertainty

The securities backdrop is better than it was during earlier discussions, but it is not risk-free.

Recent U.S. regulatory direction has become more favorable to crypto than the 2022-2024 enforcement-heavy period. Reporting in 2025 described SEC staff guidance taking the view that protocol staking and liquid staking arrangements are not necessarily securities transactions, and liquid staking tokens such as rETH were discussed in that context. That is helpful for Rocket Pool. It suggests that the old assumption “anything involving rETH/RPL in the U.S. is probably too toxic to touch” is too pessimistic.

But this is not the same thing as permanent statutory certainty. SEC staff views can change. Courts can disagree. Specific facts matter. A token can be non-security property in one context but part of an investment contract in another context depending on how it is sold, promoted, packaged, or managed.

For this memo, the practical conclusion is:

> Current conditions make a U.S. DUNA-style structure worth exploring. They do not eliminate the need for careful scope limits.

That is another reason the DUNA should stay away from official tokenomics advocacy and RPL value-accrual work.

## 13. Tax and accounting issues

The tax issues are real, but they should not make the project feel impossible.

A simple working assumption is that crypto is generally treated as property for U.S. tax purposes. Payments to people for services are generally income to those people, whether paid in dollars, USDC, ETH, or RPL. Converting RPL to USDC may create gain or loss for the entity that does the conversion. Stipends paid in RPL likely need to be valued at the time of payment. Vendors and contributors may need ordinary tax reporting depending on who they are, where they are, how much they are paid, and what entity is paying them.

The harder questions are upstream:

- What is the tax treatment of RPL inflation received by the pDAO treasury?
- What is the tax treatment when the pDAO sends RPL to a committee Safe?
- Does the answer change if the Safe is controlled by a DUNA?
- Is the transfer income, a contribution, a grant, agency funding, or something else?
- What happens if the DUNA receives RPL and later sells it for USDC?
- What filings does the DUNA need if it pays U.S. or non-U.S. contributors?
- How should third-party protocol incentives be treated?

Those questions need tax review before anyone relies on a final answer. But they do not necessarily defeat the idea. They mostly mean the DUNA should keep clean records and avoid unnecessary complexity.

A sensible policy would be:

- hold only what is needed for approved work;
- convert volatile assets for budgeting, not speculation;
- document payment purpose;
- pay reasonable compensation only for actual work;
- avoid profit distributions;
- avoid active trading or yield strategies;
- keep third-party funds restricted to approved programs where possible.

## 14. BOI / CTA reporting

The Corporate Transparency Act and beneficial ownership reporting rules have changed over time. As of the 2025 FinCEN interim rule reported publicly, domestic U.S. companies were exempted from beneficial ownership reporting, while certain foreign reporting companies still had obligations.

That is useful for a U.S. structure, but it should not be treated as permanent. BOI/CTA rules have been politically contested and legally unstable. If the pDAO actually forms a DUNA or other entity, someone should confirm the then-current reporting requirements.

The practical takeaway is not “there is definitely no reporting forever.” It is:

> Current BOI/CTA posture appears less burdensome for domestic U.S. entities than it was in early 2024, but this should be checked at formation.

## 15. Third-party funds and incentives

This is one of the trickiest areas.

One reason to have a legal service layer is so the pDAO, IMC, or related functions can accept or administer incentives from third-party protocols more cleanly. That might be useful. For example, another protocol might want to contribute funds toward a liquidity campaign, integration, co-incentive program, or ecosystem effort.

But this should be handled carefully. The DUNA should not become a revenue-generating business development company. It should not take recurring protocol fees for the benefit of members. It should not accept payments that create hidden conflicts or make it look like the DUNA is selling governance influence.

A safer model is restricted program funding:

- the third party contributes funds for a specific, disclosed purpose;
- the purpose is consistent with a pDAO-approved or committee-approved program;
- the DUNA documents that it is administering funds, not selling influence;
- conflicts are disclosed;
- funds are not distributed as profits to members;
- any compensation is reasonable payment for actual work.

This may still require legal and tax review. But it is a more defensible direction than “the DUNA can collect revenue from protocols.”

## 16. Anonymity and pseudonymity

Rocket Pool has pseudonymous contributors. Any workable structure has to respect that.

The ideal is that ordinary covered participants do not need to publicly disclose their legal identities merely because they serve on a pDAO committee. The DUNA might define covered roles by pDAO election, appointment, RPIP process, Snapshot/onchain vote, multisig role, or other governance record.

Coverage could be based on things like:

- wallet address;
- forum handle;
- Discord handle;
- committee election record;
- pDAO vote outcome;
- multisig membership;
- written appointment by an already-approved committee.

There may still need to be one legally identified organizer, registered agent, tax contact, banking contact, or attorney/accountant. That is different from forcing every committee member to dox publicly.

This is a key question for counsel:

> Can the DUNA provide meaningful role-based protection to pseudonymous committee members without requiring each person to sign public legal membership documents?

If the answer is yes, the DUNA becomes much more attractive. If the answer is no, the value of the structure drops, but it may still help with contracts, insurance, and vendor payments.

## 17. Language matters

The structure should be described carefully. Not because we are trying to hide anything, but because sloppy words can create the wrong legal and cultural impression.

Good words:

- service layer;
- execution layer;
- administrative support;
- committee support structure;
- pDAO-approved work;
- covered role;
- neutral process support;
- good-faith work within scope;
- role-based protection.

Words to avoid:

- board of the DAO;
- DAO management;
- directors of the pDAO;
- officers of the pDAO;
- controlling members;
- representatives of all RPL holders;
- maximizing RPL value;
- managing the protocol;
- leadership council.

The message should stay simple:

> The pDAO still governs. The DUNA helps people safely execute approved work.

## 18. What a minimal structure might look like

A very simple version could look like this:

1. The pDAO approves creation or use of a DUNA-style service entity.
2. The entity charter says it exists only to support pDAO-approved committee and administrative functions.
3. Covered roles are defined by pDAO governance records, committee appointments, or recognized process documents.
4. The entity can sign contracts, hold insurance, pay contributors/vendors, administer approved funds, and indemnify covered participants.
5. The entity cannot represent all RPL holders, control the protocol, own the full pDAO treasury, or advocate tokenomics changes in its official capacity.
6. The entity keeps simple records: funds received, payments made, contracts signed, conflicts disclosed, and role coverage decisions.
7. The pDAO can amend, limit, defund, or terminate the arrangement by governance.

This is meant to be incremental and reversible. It should not lock Rocket Pool into a large legal structure forever.

## 19. What still needs to be checked

The DUNA idea is promising, but a few questions need to be checked before formation:

- Is a Wyoming DUNA, or another U.S. nonprofit association form, actually the best fit?
- Can covered roles be defined by pDAO governance status rather than signed membership agreements?
- Can pseudonymous participants receive useful protection?
- Who, if anyone, must be legally identified?
- What filings, EIN, registered agent, tax returns, or state requirements apply?
- What BOI/CTA rules apply at the time of formation?
- Can the entity hold RPL and convert RPL to USDC for budgeting?
- How should pDAO transfers to the entity be characterized for tax purposes?
- How should committee stipends and vendor payments be reported?
- Can third-party incentive funds be accepted as restricted program funding?
- What insurance is available and worth buying?
- What indemnification language should be adopted?

This does not mean “nothing works without massive legal spend.” It means we have a short list of questions for a limited review.

The legal review should be scoped. It should not ask counsel to redesign all of Rocket Pool governance. It should ask whether this narrow service-layer concept works, what the main traps are, and what minimal documents are needed.

## 20. Practical recommendation

The current recommendation is:

> Keep the pDAO unwrapped for now. Explore one shared DUNA-style service layer for pDAO-approved committee and administrative work. Use it to protect people doing work, not to create DAO leadership.

This approach is not perfect. It does not solve every DAO liability problem. It does not make all tax questions disappear. It does not eliminate the need for careful behavior.

But compared with the realistic alternatives, it still seems like the best hope:

- cheaper and lighter than Cayman or Swiss foundation-style structures;
- less fragmented than separate entities for every committee;
- more useful than telling every contributor to form a personal LLC;
- less centralizing than wrapping the entire pDAO;
- more protective than doing nothing.

The DUNA should be treated as a tool, not a power center.

The best final framing is still:

> We are not creating leadership. We are creating a safe way for people to do work.

## 21. Source notes and uncertainty

This memo is a working document, not legal or tax advice.

Important current anchors include:

- DAO liability theories remain active and unsettled in U.S. litigation.
- U.S. securities treatment of staking and liquid staking appears more favorable than during the earlier enforcement-heavy period, but staff guidance and regulatory posture can change.
- U.S. tax treatment of crypto generally starts from the idea that digital assets are property, but entity-level and payment-specific questions require actual tax review.
- BOI/CTA reporting has changed since 2024, with domestic-company reporting apparently narrowed under 2025 FinCEN changes, but this should be checked at formation.

The memo should be updated as law, regulation, and Rocket Pool facts change.
