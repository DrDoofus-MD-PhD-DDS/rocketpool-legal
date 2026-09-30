# Protecting Rocket Pool pDAO Service Contributors
## Legal Structure, Privacy, Compensation, and a Possible Service Layer

**Working Research Paper — Draft 0.1**  
**Date:** September 30, 2026  
**Status:** Internal working draft for discussion and counsel review  
**Audience:** Rocket Pool pDAO participants, GMC and IMC members, RPIP editors, administrators, contributors, core-team liaisons, and prospective legal/tax counsel

> **Working premise:** We are not trying to create leadership. We are trying to create a safer legal way for people to do work that the pDAO has asked them to do.

This paper is not legal or tax advice. It is a research synthesis intended to identify the factual structure, the legal problems worth solving, the realistic structural options, and the questions that should be put to qualified counsel before the pDAO takes action.

---

# 1. Executive Summary

Rocket Pool has spent years becoming more decentralized in governance while remaining largely informal in legal structure. The pDAO now exercises meaningful protocol governance, controls on-chain proposals and treasury spending, elects or recognizes committees and other service roles, and relies on identifiable or pseudonymous people to carry out operational work. Rocket Pool's own governance documents define the pDAO as Node Operators with voting power based on effectively staked RPL and direct the pDAO to actively govern the protocol. On-chain governance has progressively removed earlier dependence on the core team to execute pDAO decisions.

That decentralization has an awkward legal consequence: **not choosing a legal structure does not necessarily mean that courts, regulators, or tax authorities will treat the organization as having no legal character at all.** U.S. DAO litigation has shown that plaintiffs and agencies will use ordinary partnership, association, agency, securities, commodity, and tort doctrines when disputes arise. The outcomes are fact-specific, and the cases do *not* establish that every governance-token holder is automatically liable for every DAO act. They do establish that “we are only a DAO” is not a reliable legal shield.

Rocket Pool's most immediate practical concern is narrower than protecting every pDAO participant. The people most exposed to being characterized as active organizational participants are the people visibly performing organizational functions: GMC and IMC members, administrators, multisig signers, RPIP process workers, treasurers, emergency/security participants, and other contributors who administer funds or interact with third parties. Many receive compensation that is modest relative to the potential burden of defending a lawsuit.

This problem has already influenced behavior. Earlier Rocket Pool legal research considered personal LLCs, indemnification, committee wrappers, Swiss associations, Cayman foundations, BORG-style structures, DAO LLCs, DUNAs, and full-pDAO entity structures. Some current committee participants formed personal LLCs for their Rocket Pool-related activities. Those measures were rational responses to uncertainty, but they are incomplete and burdensome. The pDAO should not have to depend indefinitely on each volunteer building a personal corporate firewall before agreeing to help.

The present project therefore begins with a deliberately limited objective:

> **Can Rocket Pool create a small legal service layer that protects the people carrying out pDAO-authorized work, while leaving the broader pDAO, its membership, and its main treasury outside that entity?**

That is different from incorporating the pDAO. The pDAO would remain sovereign. It would continue to govern protocol parameters, elect or remove service workers, and control its main treasury. A service entity would exist underneath that governance layer to give operational work a legal principal, liability shield, indemnification mechanism, insurance capacity, and potentially contracting capacity.

Four structures currently deserve serious consideration:

1. **Wyoming Unincorporated Nonprofit Association (UNA).** This unexpectedly simple structure requires only two or more members joined for a common nonprofit purpose. Wyoming law treats it as a legal entity separate from its members for contract and tort liability and expressly protects people from liability solely because they are members or authorized management participants. Its advantages are simplicity and compatibility with a small committee-only organization. Its principal uncertainties are pseudonymous membership, federal tax classification, and whether contractual indemnification and advancement can be made as robust as the DUNA's statutory protections.

2. **Wyoming Decentralized Unincorporated Nonprofit Association (DUNA).** Wyoming's DAO-specific association law is extraordinarily well matched to Rocket Pool in several respects: it recognizes smart contracts and enacted governance proposals as governing principles, permits members and nonmembers to act as administrators, does not require the DUNA to maintain members' names and addresses, provides an explicit liability shield for administrators, and expressly authorizes indemnification, advance payment of legal expenses, and insurance. The major new problem is Wyoming's 2026 amendment requiring at least **100 consenting members**. A committee-only DUNA with seven or ten members is no longer available. A separate, voluntary 100+ member service association remains possible, but the 100-member population would exist mainly to support a much smaller administrator layer.

3. **Wyoming DAO LLC.** This is a more conventional entity with clearer federal tax treatment and familiar LLC liability rules. It remains worth comparing, especially now that U.S.-created entities are exempt from federal Corporate Transparency Act beneficial-ownership reporting under FinCEN's August 2026 final rule. However, its conventional member/manager structure and private identification requirements may be a poorer cultural fit for a service group in which some members refuse even private doxxing.

4. **Marshall Islands DAO LLC through MiDAO or a similar RMI structure.** This offshore option deserves renewed attention if U.S. payer-side tax reporting proves culturally unacceptable. RMI DAO LLCs can keep most members pseudonymous while requiring KYC for specified beneficial owners, managers, or another required person. The information is not public. The tradeoff is greater formation and annual cost and continued home-jurisdiction tax obligations for participants. Offshore structure does not make U.S. participants disappear from U.S. law.

The most difficult issue uncovered by the current research is **compensation**. Wyoming entity law is unusually friendly to pseudonymous decentralized participation. Federal tax reporting is less so. Digital assets received for services are ordinary income based on their U.S.-dollar fair market value when received. For 2026, Form 1099-NEC generally applies to at least $2,000 of nonemployee service compensation per payee, and reportable payments without a required TIN can implicate backup withholding. Foreign participants raise a different withholding and documentation regime. A “stipend” calculated from committee participation cannot safely be converted into a “grant” merely by changing its name.

There are nevertheless several plausible design responses. Service workers could choose between full compensation with private tax identification, lower compensation below applicable reporting thresholds where counsel confirms that works, or prospectively waiving compensation. A pDAO-controlled smart contract might pay fixed stipends directly to elected service addresses while the service entity itself does not receive, calculate, or distribute those stipend funds. That separation could strengthen the argument that the legal entity is not the federal payment administrator, but it does not eliminate the possibility that the unwrapped pDAO itself is the payer. This needs tax counsel rather than assumption.

A preliminary anonymous survey of the GMC is more encouraging than expected. There were eight submissions, seven complete. Among the seven complete responses, five said that if forced to choose they would privately identify themselves to a trusted outside professional in exchange for the normal/full stipend; one would remain pseudonymous and take a smaller stipend; one would decline to serve. Five of seven said they were comfortable with a system in which people who privately identify receive more compensation than people who remain completely pseudonymous. This is a small and highly specific sample, and IMC responses remain pending, but it weakens the assumption that private tax identification would necessarily make a U.S. service structure politically impossible.

The current working conclusion is therefore **not** “form a DUNA.” It is:

> A narrow service-layer entity remains worth pursuing. The pDAO itself should not be assumed to need wrapping. The main treasury should presumptively remain outside the service entity. Wyoming UNA and DUNA structures deserve the closest legal review, with an RMI DAO LLC as a serious alternative if U.S. compensation/reporting rules conflict with participant privacy. The decisive questions are now narrow enough to put efficiently to Wyoming and federal tax counsel.

---

# 2. What the Rocket Pool pDAO Actually Is

Legal analysis is only useful if it starts from what Rocket Pool really does rather than from a generic picture of a DAO.

Rocket Pool's pDAO Charter defines the pDAO as Node Operators whose governance power is based on effectively staked RPL. The charter says that the pDAO actively governs the protocol and should prioritize safety, decentralization, and permissionlessness. This is important because pDAO membership is not merely a social label; it is tied to on-chain governance rights and protocol-defined voting power. [RPIP-23]

Rocket Pool has also moved substantially beyond the older model in which community votes were merely signals for a centralized core team. RPIP-33 established on-chain pDAO governance and expressly contemplated the pDAO controlling protocol settings and spending treasury funds. The purpose of that change was to remove dependency on the core team and make governance more decentralized and trustless. [RPIP-33]

Current governance therefore has several layers:

- **The pDAO itself**, composed of eligible Node Operators with voting power based on effectively staked RPL and delegation.
- **On-chain governance**, through which eligible nodes can propose, vote, and execute certain protocol changes and treasury expenditures.
- **The Grants Management Committee (GMC)**, currently seven voting members, which evaluates and funds grants, bounties, and retrospective awards under a pDAO-created mandate. [RPIP-36; RPIP-76]
- **The Incentives Management Committee (IMC)**, which administers incentives intended to support rETH/RPL usage and liquidity under its governance mandate.
- **RPIP Editors and the pDAO Treasurer**, recognized in the committee/role records and governance process.
- **Administrative roles**, particularly the GMC Administrator, whose responsibilities include meeting coordination, award facilitation, liaison work, treasury functions, and governance drafting under the current GMC framework. [RPIP-76]
- **Security and emergency functions**, including Security Council mechanisms and newer signaling/emergency-ballot governance infrastructure.

Committee service is not purely honorary. RPIP-41 establishes stipend budgets based on target member count, target hours, and a global stipend rate. For the GMC, the current target is seven members, fifteen hours per member, and a $3,150 monthly stipend budget. Committee stipend allocation has historically depended on monthly contribution measures rather than a conventional payroll system. [RPIP-41]

This matters legally because Rocket Pool is no longer well described as a chat room where tokenholders occasionally express opinions. It has governance rules, delegated bodies, recurring funds, defined responsibilities, compensation, operational wallets, and people who make decisions in recognizable organizational roles.

None of that proves that the pDAO, its committees, or its participants are a partnership, corporation, employer, or any other specific legal category. It does mean that a court or agency has real facts to work with if someone asks what the organization is.

---

# 3. Why Legal Structure Matters Even When Nobody “Incorporates”

A recurring intuition in decentralized communities is that legal entity formation creates legal exposure, while remaining informal preserves legal neutrality. That is too simple.

The law already contains default rules for groups that act together without intentionally forming a corporation or LLC. Which rules apply depends on jurisdiction and facts, and Rocket Pool should not assume that any particular default characterization is inevitable. But refusing to choose an entity does not force courts to treat the organization as legally nonexistent.

## 3.1 bZx / Sarcuni: partnership theories are not imaginary

In *Sarcuni v. bZx DAO*, plaintiffs alleged that bZx DAO was a California general partnership and that DAO-related defendants were partners who could be liable for a hack-related loss. At the motion-to-dismiss stage, the federal district court held that the complaint plausibly alleged a general partnership. The court emphasized California's rule that people can form a partnership by carrying on as co-owners of a business for profit whether or not they intended to create a partnership. The decision accepted the allegations for pleading purposes; it was not a final rule that every DAO or tokenholder is always a partner.

The lesson is narrower and more important: **lack of formal incorporation did not prevent the plaintiffs from using ordinary partnership law to construct a liability theory.**

## 3.2 Lido: active participation may matter more than passive tokenholding

The Lido litigation offers an especially useful contrast. In a November 2024 order, the federal court found a pleaded partnership theory plausible as to entities alleged to have the capacity for meaningful participation in Lido DAO management. The court expressly distinguished the theory from one in which every tokenholder automatically becomes a partner. In April 2025, the same court dismissed conditional counterclaims against the plaintiff because the allegations did not show that he jointly carried on the DAO's business or meaningfully participated in management.

Rocket Pool should not assume that those rulings determine how a court would treat Rocket Pool. But they make the practical distinction at the heart of this project easier to see:

> A passive holder or occasional voter may present a different legal profile from an elected committee member, administrator, multisig signer, large delegate, or other person who visibly participates in management-like activity.

That is one reason a committee/service-layer project can be sensible even if the pDAO itself remains unwrapped.

## 3.3 Ooki: an unincorporated DAO is not legally invisible

The CFTC's case against Ooki DAO produced a 2023 default judgment in which the court held Ooki DAO to be a “person” under the Commodity Exchange Act. Earlier in the proceeding the court had treated the DAO as an unincorporated association that could be sued and served. The default posture matters—the court assumed well-pleaded allegations rather than conducting a full adversarial trial—but the case still undercuts the idea that legal accountability can be avoided simply by not filing formation documents.

## 3.4 Being sued is itself a cost

The pDAO does not need to believe that a plaintiff would ultimately win against a committee member to take this seriously. Litigation costs money before the merits are resolved. The burden is particularly hard to justify when people are performing governance work for hundreds of dollars a month.

The practical objective is not to guarantee that nobody can ever sue a participant. No entity can do that. It is to improve the answer when a participant is sued merely because the organization did something:

**Today:** “I am one of the pseudonymous people who helped this unwrapped DAO make and execute decisions.”

**Desired future:** “The relevant operational function was performed through a legally distinct service organization. I acted in an authorized role for that organization, which has its own liability rules, indemnification process, and defense capacity.”

That is a meaningful difference even though it is not absolute immunity.

---

# 4. The Practical Rocket Pool Problem

Rocket Pool's legal-structure problem is unusual because its risk and resources are badly mismatched.

The pDAO does not have a large diversified treasury that can casually spend six figures on offshore structuring. Its main treasury is currently modest, and the committees themselves have been operating in a period of constrained funding. Recent governance changes increased committee funding and rebalanced RPL inflation, but those changes arose in the context of a funding crisis and declining RPL-denominated purchasing power, not abundance.

At the same time, the organization asks real people to perform tasks that look increasingly organizational:

- decide whether grants should receive funds;
- sign multisig transactions;
- administer recurring incentive programs;
- coordinate with external projects or applicants;
- maintain governance processes and voting infrastructure;
- perform treasury and administrative work;
- participate in emergency/security functions;
- communicate publicly in an official capacity.

The solution therefore cannot be a beautiful legal structure that costs more than the problem is worth. It has to be **cheap, boring, maintainable, and culturally tolerable**.

This also explains why the issue cannot be reduced to “there is not much money to sue for.” The principal target of protection is not necessarily the pDAO treasury. It is the personal balance sheet and defense burden of the individual who happened to volunteer for the committee.

A useful way to state the design problem is:

> Rocket Pool needs enough legal structure to protect and support the people doing work, without creating more organizational machinery than the pDAO has money or volunteers to maintain.

---

# 5. How We Got Here

The current project is the result of several earlier approaches, not a sudden decision that Wyoming associations are fashionable.

## 5.1 Personal LLCs

The earliest practical response was individual self-protection. Internal Rocket Pool legal research and several consultation notes encouraged active committee participants to consider conducting Rocket Pool-related activities through personal LLCs. The theory was straightforward: separate personal assets from DAO-related wallets and activities, document the business relationship, keep business funds separate, and create a legal defendant other than the natural person where possible.

Some committee members have done this. It remains useful, particularly where the individual has substantial ongoing work or already operates a personal business entity.

But personal LLCs are an incomplete system-wide solution:

- every new volunteer must separately understand and pay for formation;
- maintaining corporate separateness requires discipline;
- protection can be undermined by poorly documented or pre-formation conduct;
- it does not give the committee itself contractual capacity or insurance;
- it does not give the pDAO a shared mechanism for defending people acting in official roles;
- it raises a fairness problem if serving on a committee effectively requires a person to buy their own legal infrastructure.

The personal-LLC approach may remain complementary to a service entity, but the service entity should ideally reduce the need for it.

## 5.2 Indemnification and legal-defense funding

A second approach was for the pDAO to promise to defend committee members acting in good faith within their authorized roles. This is attractive because it is conceptually simple and can be implemented by governance.

Indemnification is useful, but it is not a substitute for entity formation. If an unwrapped DAO promises indemnification, questions remain about who legally made the promise, who can enforce it, who controls the defense fund, and whether a plaintiff can still characterize the indemnified people as participants in the underlying unincorporated organization.

A service entity can make indemnification much more concrete: the organization can be the indemnifying party, hold a legal-defense reserve, buy insurance, retain counsel, and advance expenses under defined conditions.

## 5.3 One entity per committee and BORG-style models

The research then considered wrapping separate committees or creating related entities. That has the theoretical benefit of isolating risks—GMC liabilities would not necessarily become IMC liabilities, and vice versa.

The practical problem is obvious. Rocket Pool already struggles to fill and sustain service roles. Creating several entities means several sets of governance documents, tax/compliance calendars, legal relationships, possible accounts, insurance arrangements, and transition problems every time committees turn over.

For a resource-constrained protocol, fragmentation can create more operational risk than it removes.

## 5.4 Cayman foundation structures

Cayman structures were attractive because they are familiar in the crypto industry, can own assets and contract, and can provide an external legal person that absorbs organizational activity. Earlier consultations considered foundation-based “liability sink” concepts.

For Rocket Pool, the persistent problem has been proportionality. Cayman structures are designed for organizations able to support meaningful legal and administrative infrastructure. Rocket Pool's treasury and committee stipends make a high-cost foundation difficult to justify. Foundations can also create a governance council or director layer that feels more permanent and centralized than the pDAO wants.

Cayman remains conceptually useful as an example of what a mature, well-funded DAO might do. It does not currently look like the natural first move for Rocket Pool.

## 5.5 Swiss Association

The Swiss Association was one of the more attractive historical options. Earlier counsel discussions emphasized Switzerland's established, technology-neutral association law, flexible member governance, and long history relative to newer DAO-specific statutes. It was particularly attractive when the United States was perceived as hostile or unpredictable for crypto projects.

That relative advantage has changed. The United States has adopted more DAO-specific law, Wyoming has refined its DUNA framework, and federal securities policy toward protocol staking became materially clearer in 2026. A Swiss Association remains a possible alternative, but the reason to accept foreign jurisdictional cost and complexity is weaker than it was in the earlier paper.

## 5.6 Wrapping the whole pDAO

The broadest solution would be to make the pDAO itself a legal organization. That would address the legal identity problem most directly, but it creates political and structural questions that are unusually difficult for Rocket Pool:

- pDAO membership is dictated by protocol governance rights, not a conventional membership application;
- some members will not consent to joining a legal entity;
- many members are pseudonymous;
- participation is international;
- tax consequences may differ by jurisdiction;
- the pDAO community is strongly privacy- and permissionlessness-oriented;
- the main treasury is controlled by pDAO governance and should not casually be placed under a separate board or manager;
- forcing legal membership through a successful pDAO vote raises consent questions rather than solving them.

It may eventually be appropriate to formalize the pDAO itself. This paper does not conclude that it never should. The point is that **full-pDAO wrapping is not necessary to pursue the narrower problem of protecting service contributors.**

## 5.7 The service-layer idea

The current framing emerged from those failures and tradeoffs:

> Leave the pDAO as the sovereign governance layer. Create a narrow legal organization underneath it for the people and functions that actually perform operational work.

The service entity should not own the protocol, manage tokenomics, or become the pDAO's board of directors. It should exist to make delegated work legally boring.

---

# 6. Design Requirements

Before selecting an entity, Rocket Pool should define the requirements. Otherwise entity selection becomes a list of abstract legal advantages that do not fit the community.

## 6.1 Preserve pDAO sovereignty

The pDAO must remain the ultimate governance authority for protocol matters. The service entity should receive delegated authority, not sovereign authority.

## 6.2 Do not automatically wrap the pDAO

Service-layer formation should not require every RPL-staking pDAO participant to become a legal member of the service entity.

## 6.3 Leave the main treasury outside by default

The pDAO's main treasury is small enough that moving it into a legal entity provides limited economic benefit and creates tax, control, and political complexity. The working presumption should be that it remains governed and held as it is today.

## 6.4 Protect active workers

The structure should cover committee members, administrators, editors, treasurers, and other pDAO-authorized service roles where appropriate. Protection should attach because of the person's role and authorized conduct, not because the person is publicly doxxed.

## 6.5 Preserve public pseudonymity

A viable structure must allow most service workers to remain publicly pseudonymous. The project should distinguish public identity disclosure from limited private tax/compliance disclosure.

## 6.6 Minimize private identification

Some current and prospective workers may refuse even private doxxing. A structure should therefore support uncompensated or low-compensation pseudonymous participants where legally possible and should avoid collecting identity data that is not actually required.

## 6.7 Keep overhead proportional

Rocket Pool should not spend Cayman-foundation money to solve a committee-stipend problem. Formation, tax preparation, registered-agent services, insurance, and ongoing administration must be affordable relative to the treasury and the actual risk.

## 6.8 Make turnover easy

Committee and service roles change. A structure that requires expensive legal amendments every time an elected member rotates is a poor fit.

## 6.9 Work internationally

Rocket Pool service contributors are not all U.S. persons. The structure must anticipate foreign participants rather than treating them as exceptions.

## 6.10 Do not make legal restructuring depend on governance redesign

A future unified service-worker election may make operational sense, but legal protection should be implementable under today's committee structure. Otherwise objections to governance reform could sink the legal project and vice versa.

---

# 7. Candidate Structure One: Wyoming UNA

The ordinary Wyoming Unincorporated Nonprofit Association has become the unexpected contender in this research.

## 7.1 What it is

Wyoming defines a nonprofit association as an unincorporated organization of **two or more members joined by mutual consent for a common nonprofit purpose**. A member is someone who may participate in selecting management or developing association policy. The statute allows the association to hold real and personal property and to be a beneficiary of a trust or contract. [Wyo. Stat. §§ 17-22-102 to -104]

That fits a seven- or ten-person service organization far more naturally than a 100-member DUNA.

## 7.2 The liability shield is substantive

The important provision is § 17-22-106. Wyoming says the UNA is a legal entity separate from its members for determining contract and tort rights and liabilities. A person is not liable for the association's contract **solely because** the person is a member or authorized to participate in management. Likewise, a person is not liable for a tort for which the association is liable solely because the person is a member or authorized management participant. A judgment against the association is not, by itself, a judgment against a member.

That statutory language is unusually relevant to Rocket Pool. The people we are trying to protect are not passive members; they are precisely the people authorized to participate in management-like functions.

The word “solely” matters. The UNA does not immunize a person from their own fraud, intentional misconduct, personal tort, or independent statutory violation. It helps prevent liability from being imputed merely because of organizational status or management participation.

## 7.3 State-law formalities appear light

Unlike an LLC, Chapter 22 does not appear to require conventional articles of organization as the condition of existence. The association arises from the statutory facts of mutual consent and common nonprofit purpose. Wyoming says a UNA **may** file a statement appointing an agent for service of process. This needs practical counsel review, because an entity that wants an EIN, insurance, or contracts may still need documentary proof of existence and authority even if the statute itself is light.

## 7.4 The two major unknowns

### Pseudonymous membership

The ordinary UNA statute does not expressly require a member-name registry, but it also lacks the DUNA's explicit statement that the association need not collect or maintain names and addresses. We need Wyoming counsel to confirm whether a UNA can be validly composed and managed by blockchain identities whose underlying natural-person names are not known to the association.

### Indemnification and advancement

Chapter 22 contains the liability shield but does not contain the DUNA's detailed statutory indemnification, advancement-of-attorney-fees, and insurance section. The association can contract and hold property, so contractual indemnification may be available, but this should not be assumed to be equivalent to the DUNA's explicit statutory framework.

This is probably the decisive UNA question:

> Can a Wyoming UNA agreement provide robust indemnification, mandatory advancement of reasonable defense expenses, and insurance coverage to pseudonymous authorized managers on terms comparable to a DUNA?

If the answer is yes, the UNA may be the cleanest structure for Rocket Pool's actual size.

---

# 8. Candidate Structure Two: Wyoming DUNA

The Wyoming DUNA remains the structure most obviously drafted with blockchain organizations in mind.

## 8.1 Why it fits conceptually

The DUNA statute expressly recognizes:

- smart contracts;
- distributed-ledger voting;
- enacted governance proposals as governing principles;
- membership voting rights established through distributed-ledger technology;
- administrators who may be members or nonmembers and who perform operational tasks at the direction of the membership.

Those concepts map unusually well onto a pDAO-delegated service organization.

## 8.2 The 2026 100-member change

Effective July 1, 2026, Wyoming requires a DUNA to consist of **at least 100 members joined by mutual consent** under an agreement, which may be written or inferred from conduct, for a common nonprofit purpose. If membership later falls below 100 and the entity otherwise satisfies Wyoming UNA requirements, the statute automatically converts it to an ordinary UNA unless its governing principles say otherwise. [2026 Wyo. Sess. Laws ch. 25; Wyo. Stat. §§ 17-32-102, -114]

This fundamentally changes the old Rocket Pool proposal. A DUNA consisting only of GMC/IMC/service workers no longer works.

But it does **not** necessarily mean that the entire pDAO must become the DUNA.

A separate Rocket Pool Service DUNA could have:

- 100+ voluntary, consenting community members;
- a much smaller elected or appointed administrator group;
- no control over the main pDAO treasury;
- a purpose limited to supporting pDAO-authorized service work.

The 100 members would constitute the association. The administrators would do the operational work.

## 8.3 Privacy is the DUNA's strongest advantage

Wyoming expressly says that a DUNA **is not obligated to collect and maintain a list of members or individual member information, including names or addresses**. [Wyo. Stat. § 17-32-124(e)]

This is a major distinction from conventional entities. A voluntary 100-member association could potentially be defined by wallet-based consent and governance identity rather than a spreadsheet of legal names.

The statute does not, however, eliminate federal EIN, tax, banking, insurance, or counterparty KYC obligations. State-law anonymity and federal tax privacy are separate questions.

## 8.4 Administrators map well to committee workers

An administrator can be a member or nonmember authorized by the membership to fulfill administrative or operational tasks. That provides a natural statutory category for GMC/IMC/admin/editor/treasury roles without requiring those people to constitute the 100-member base.

Wyoming also permits the DUNA to pay reasonable compensation and reimburse reasonable expenses for services, including administration, operation, voting, and participation. [Wyo. Stat. § 17-32-104]

## 8.5 Liability and indemnification are unusually explicit

The DUNA is a separate legal entity for contract and tort liability. A person is not liable merely because they are a member, administrator, or authorized management participant. A judgment against the DUNA is not, by itself, a judgment against a member or administrator. [Wyo. Stat. §§ 17-32-107 to -109]

More importantly for this project, § 17-32-125 expressly permits the DUNA to:

- reimburse authorized expenses;
- indemnify members and administrators for liabilities incurred in activities on behalf of the DUNA;
- advance reasonable litigation expenses and attorneys' fees, subject to statutory conditions and member approval;
- purchase insurance on behalf of members and administrators.

This is almost a statutory description of the problem Rocket Pool wants to solve.

## 8.6 The price of those advantages

The 100-member requirement is not trivial. Rocket Pool would need to maintain real consensual membership rather than merely declare random pDAO addresses to be DUNA members. Recruitment, resignation, and governance need to be handled intentionally.

The DUNA also remains novel in federal tax law. Real DUNAs such as Towns Lodge have obtained EINs, filed Form 8832, and operated as corporations filing Form 1120, but tax practitioners previously asked Treasury and the IRS for precedential guidance specifically because DUNA classification was not entirely clear under the existing entity-classification regulations. A real-world implementation is encouraging; it is not the same as binding IRS guidance.

The Rocket Pool DUNA should therefore not be formed until tax counsel confirms how to avoid partnership/K-1 treatment for a pseudonymous 100-member association.

---

# 9. Candidate Structure Three: Wyoming DAO LLC

A Wyoming DAO LLC remains the conventional U.S. comparison.

Its advantages are important:

- well-understood LLC limited liability;
- conventional operating-agreement machinery;
- clear state filing and continuity;
- explicit smart-contract governance under Wyoming's DAO LLC statute;
- far clearer federal tax classification than a DUNA or UNA.

A multi-member domestic LLC is generally a partnership for federal tax purposes unless it files Form 8832 and elects corporate treatment. If it elects C-corporation treatment, the corporation files Form 1120 and does not issue partnership K-1s merely because people are members. That path is familiar to accountants and the IRS.

The DAO LLC also became less unattractive in 2026 because FinCEN's final BOI rule now exempts U.S.-created entities from Corporate Transparency Act beneficial-ownership reporting. That removes a major objection found in earlier Rocket Pool drafts.

The problem is Rocket Pool culture. Conventional LLC administration often expects identifiable managers or other responsible parties. Even if that identity information is not public, some service workers have indicated that they may refuse private doxxing as well. It may be possible to use one identified manager and treat pseudonymous workers as agents or contractors, but if substantial structuring is required to make an LLC behave like a DUNA, the DAO-specific association may be the more natural tool.

The DAO LLC should stay on the comparison table, but it is no longer the obvious baseline.

---

# 10. Candidate Structure Four: Marshall Islands DAO LLC / MiDAO

The Marshall Islands DAO LLC deserves renewed attention because the most difficult part of the Wyoming project is becoming federal payer-side identity reporting rather than state entity law.

## 10.1 Privacy model

Current MiDAO documentation says most DAO LLC members can remain pseudonymous while specified persons complete KYC/KYB. Under its current process, KYC generally applies first to anyone with 25% or more governance rights; if nobody meets that category, to all managers if there are managers; if neither category applies, to a member. The beneficial-owner/KYC information is not public, although it can be disclosed when legally required.

This is culturally closer to Rocket Pool's likely tolerance: **a small number of people privately identify while the broader group remains wallet-based.**

## 10.2 Cost

The RMI option is more expensive than Wyoming. MiDAO currently advertises standard formation at $9,500, with discounts as low as $3,000 for projects under $250,000 in treasury and funding. Annual fees currently range from $2,000 to $5,000 depending on treasury/funding size. Those are provider prices and can change; separate legal/tax advice may add cost.

For Rocket Pool, that is not trivial. A structure that costs several thousand dollars every year consumes money that could otherwise fund protocol work.

## 10.3 Compliance remains real

RMI DAO LLCs have annual filings, beneficial-owner information reporting, representative-agent requirements, and periodic KYC refreshes. The Marshall Islands registry also requires annual economic-substance reporting for non-resident domestic entities.

The RMI is therefore not an “anonymous offshore escape.” It is a different allocation of compliance.

## 10.4 Tax caution

The official RMI corporate registry says non-resident domestic entities are statutorily exempt from RMI taxes. MiDAO additionally describes nonprofit DAO LLCs as tax-free in the RMI and without economic owners. Those claims address RMI law, not the U.S. tax obligations of a U.S. administrator, grantee, or service provider. MiDAO itself advises members to obtain home-jurisdiction tax advice.

The key question for Rocket Pool is therefore not whether the RMI entity itself pays RMI tax. It is:

> Does a foreign nonprofit DAO LLC allow meaningful compensation and grants to pseudonymous participants without imposing U.S. payer-side identification requirements that are materially similar to the Wyoming problem?

That question has not yet been researched enough to treat RMI as a solution. It is the correct fallback branch if Wyoming tax reporting proves culturally unacceptable.

---

# 11. Comparison of the Leading Structures

| Issue | Wyoming UNA | Wyoming DUNA | Wyoming DAO LLC | RMI DAO LLC / MiDAO |
|---|---|---|---|---|
| Minimum member population | 2 | 100 | LLC structure | Flexible under RMI rules |
| Need to wrap pDAO | No | No | No | No |
| Separate legal person / liability shield | Yes | Yes | Yes | Yes |
| Explicit DAO/smart-contract governance | No specific DAO provisions | Strong | Strong | Strong |
| Explicit administrator role | No DUNA-style definition | Strong | Manager/member model | Flexible manager/algorithmic model |
| Explicit member-name privacy | Not explicit | Strong statutory language | More conventional records | Most members can remain pseudonymous under provider model |
| Explicit indemnification/advance/insurance | Needs counsel | Strong | Conventional LLC | Operating-agreement / RMI counsel review |
| Federal tax clarity | Uncertain | Novel but corporate elections used in practice | Strongest | Cross-border complexity |
| 100-member maintenance problem | No | Yes | No | No comparable Wyoming threshold |
| Cultural privacy fit | Potentially good | Very good at state-law level | Mixed | Potentially good |
| Cost | Potentially lowest | Potentially low state-law overhead | Low/moderate | Material provider fees |
| Principal concern | Indemnity + tax + pseudonymous validity | 100 members + federal tax/payment rules | Private identity/manager fit | Cost + cross-border tax/compliance |

No structure is currently ready for selection without counsel.

---

# 12. Privacy: “Doxxing” Is Not One Thing

The project has repeatedly become confused because “doxxing” is used to mean several very different disclosures.

For design purposes, at least five privacy levels should be distinguished:

1. **Public disclosure** — legal identity appears in public filings, public governance documents, or searchable registries.
2. **Community disclosure** — other committee members or pDAO participants learn the person's identity.
3. **Internal compliance disclosure** — one designated pDAO/service-entity compliance person knows the identity.
4. **Professional disclosure** — only an outside lawyer, accountant, or specialized payment provider knows the identity.
5. **Government disclosure** — tax or regulatory authorities receive identity information through legally required filings.

A service member may reject level 2 while tolerating levels 4 and 5. Treating both situations as “doxxing” obscures a potentially workable compromise.

## 12.1 Preliminary GMC survey

An anonymous GMC survey conducted in September 2026 produced eight submissions, seven complete. This is not a representative pDAO poll; it is valuable because the respondents are the people whose willingness to serve is directly relevant.

Among the seven complete responses:

- six would privately identify to one designated pDAO legal/compliance person;
- five would identify to an outside lawyer/accountant;
- five would identify to a third-party payment/compliance provider;
- two selected the option saying they would not provide their legal identity to anyone, although one of those also selected conditional disclosure options and explained that trust and the legal consequences of identity disclosure would determine the answer;
- when forced to choose the most likely real-world option, five selected private identification to a trusted outside professional in exchange for the normal/full stipend, one selected pseudonymity plus a smaller stipend, and one selected declining to serve;
- five were comfortable with differential compensation where private-identification participants receive a normal stipend and fully pseudonymous participants receive less or nothing; one would accept the arrangement but reduce effort; one opposed it.

The survey also suggests that “everyone will happily work for free” is a poor assumption. Two of the seven complete respondents said they probably would not serve unpaid, three were uncertain depending on workload, and only two expected to contribute similarly without compensation.

IMC responses are pending and may produce a different privacy profile. The appropriate conclusion at this stage is modest:

> Private identity disclosure to a trusted professional appears more acceptable to current GMC participants than earlier discussion assumed, but a viable structure still needs a pseudonymous path for people who refuse it.

---

# 13. Compensation: The Hardest Federal Issue

The biggest obstacle to a U.S. service entity may not be Wyoming law. It may be federal information reporting.

## 13.1 Crypto compensation is still compensation

The IRS states directly that digital assets received in exchange for services are ordinary income. The amount is the fair market value in U.S. dollars when received. Digital assets received by an independent contractor for services are generally self-employment income. Paying in RPL rather than dollars therefore does not remove the tax issue.

## 13.2 2026 reporting threshold

For payments made in 2026, Form 1099-NEC generally applies when a trade or business pays a nonemployee at least **$2,000** for services during the calendar year. The threshold increased from $600 for pre-2026 payments and is scheduled for inflation adjustment after 2026.

That threshold affects information reporting; it does **not** create a tax-free allowance. A participant paid $1,800 still has taxable income.

## 13.3 W-9 and backup withholding

When a U.S. person receives reportable 1099 payments, the payer normally needs a taxpayer identification number, typically obtained on Form W-9. Missing or incorrect TIN information can trigger 24% backup withholding for reportable payments.

That is why meaningful recurring compensation is difficult to combine with complete private anonymity from the payer.

## 13.4 Foreign participants are different, not automatically easier

Foreign participants implicate source-of-income, withholding, Form 1042-S, W-8, treaty, and physical-location rules. A foreign person performing services entirely outside the United States may have a substantially different result from a U.S. person, but the payer may need documentation to know that the person is foreign and that the services are foreign-source.

The project should not promise a universal $2,000 anonymity rule for international workers.

## 13.5 “Call it a grant” is not a solution

Current committee stipends are earned through service: meeting attendance, transaction signing, and contribution formulas. Calling those payments “grants” would not change their substance.

Genuine grants are different and can fall under other information-reporting rules, including Form 1099-MISC for certain non-government grants. But a payment for ongoing committee service should be structured honestly as compensation.

---

# 14. Possible Compensation/Privacy Paths

The emerging design does not require one compensation rule for everyone.

## 14.1 Full stipend + private identification

A participant who wants normal compensation could provide required tax information privately to a trusted accountant, lawyer, compliance administrator, or payment provider. Public identity need not follow from private tax compliance.

This is the most conventional path and, based on the preliminary GMC survey, may be acceptable to many existing service workers.

## 14.2 Smaller stipend below the applicable reporting threshold

A U.S. nonemployee who remains below the applicable annual 1099-NEC threshold may avoid a 1099 filing triggered solely by that compensation amount. This could permit a modest pseudonymous stipend while the participant remains responsible for reporting the income.

This needs counsel confirmation, particularly for backup-withholding edge cases, aggregated payments, foreign participants, and worker classification. The stipend should not be engineered at $1 below the threshold; a meaningful buffer would be prudent if the concept is used.

## 14.3 Prospectively waive compensation

An administrator can potentially remain unpaid without losing the state-law liability protections associated with their organizational role. If a person chooses this path, the waiver should occur prospectively, before compensation becomes earned or unconditionally available, to avoid constructive-receipt questions.

The survey suggests this is useful as an option but should not be the primary staffing model.

## 14.4 Payment through a personal business entity

Some participants already use personal LLCs. Depending on how a personal entity is taxed and documented, it may affect payer-side reporting and privacy. A disregarded single-member LLC does not necessarily hide the owner's federal taxpayer identity from the payer, while corporate tax treatment can change information-reporting mechanics.

This is too participant-specific to make the default rule, but it can remain an optional path.

## 14.5 Third-party confidential payment provider

A specialized provider might collect tax identities and handle reporting while Rocket Pool service peers know only wallet identities. This does not create absolute anonymity—the provider knows the person—but it can preserve community pseudonymity.

Cost and crypto compatibility need investigation.

---

# 15. Separating the Service Entity From the Stipend Payer

One of the strongest current design ideas is to separate legal role from payment execution.

Conceptually:

```text
                       Rocket Pool pDAO
                              |
              +---------------+----------------+
              |                                |
      elects service workers          delegates service functions
              |                                |
      fixes stipend by RPIP                    v
              |                       Service UNA / DUNA
              v                                |
      stipend smart contract                    |
              |                           administrators
              v                                |
      elected wallet addresses          perform service work
```

The pDAO, not the service entity, would:

- set the stipend amount;
- define objective eligibility;
- fund a smart contract;
- cause the smart contract to pay elected addresses automatically.

The service entity would not receive those stipend funds, calculate relative contribution, or decide monthly pay.

This could be strengthened by replacing the current contribution-weighted stipend with a fixed amount for each seated service worker, subject only to objective status such as election, resignation, removal, or prospective opt-out. The service entity would therefore have less “management or oversight” over compensation.

The tax benefit is **not established**. Federal rules can sometimes treat a person as a reporting payer even when another party supplies the funds if that person exercises management or oversight over the payment. Conversely, purely ministerial payment functions can be treated differently. The smart-contract design is promising precisely because it creates a clearer factual separation, but counsel needs to determine whether the reporting payer is the pDAO, the service entity, another person, or nobody who can practically perform conventional reporting.

There is also a liability-architecture question. The documents must make clear that a person is paid by the pDAO because they hold an elected service role, while the actual operational work is undertaken in their capacity as an administrator or agent of the legal service entity. Otherwise direct pDAO compensation could be used to argue that the worker was really acting as an unwrapped pDAO manager rather than through the service entity.

This is one of the most important questions for counsel.

---

# 16. Grants to Anonymous Recipients

Formation of a UNA or DUNA does **not**, by itself, prohibit grants to pseudonymous recipients.

The problem is federal payer/grantor status. If the service entity itself becomes an identifiable U.S. grantor, certain sufficiently large grants can trigger information-reporting or foreign withholding/documentation obligations. Current IRS instructions place certain non-government grants and other income payments in Form 1099-MISC reporting at the applicable threshold.

This creates a strong reason not to assume that the GMC grant reserve should automatically be moved into the service entity.

A better working design may be:

```text
pDAO / existing grant treasury
        |
        | approves and pays grants
        v
 pseudonymous recipients

Service entity
        |
        | protects / organizes GMC administrators
        v
 committee service workers
```

The hard question is whether the service entity becomes the tax “payor” anyway if its administrators substantively select recipients or control awards. A stronger separation would have the pDAO approve award slates and the service entity perform only recommendation or ministerial execution, but that would add governance friction and may be unnecessary if counsel reaches a more favorable tax conclusion.

The grant issue should therefore remain separate from the stipend issue. The pDAO should not sacrifice a functioning pseudonymous grant program merely because it wants liability protection for committee workers.

---

# 17. The Main Treasury Should Presumptively Remain Outside

The main pDAO treasury is not the reason this project exists.

Moving it into the service entity would create several unnecessary questions:

- Is the legal entity now the owner of pDAO assets?
- Does an administrator have legal control that the pDAO did not intend to delegate?
- Does receipt of treasury assets create entity-level income or tax accounting?
- Does moving funds imply that the entity represents all pDAO participants?
- Would the community accept an off-chain legal principal standing between on-chain governance and treasury assets?

For a roughly $200,000 treasury, the benefit is not obviously worth the complication.

The working assumption should be:

> **The pDAO treasury remains under pDAO smart-contract control. The service entity holds only assets needed for its own legal existence, insurance, defense, administration, or specifically delegated operations.**

Even committee grant/incentive reserves should stay outside until tax counsel confirms there is a reason to move them inside.

---

# 18. Does Formalizing Now Make the Past Worse?

This concern deserves direct treatment because it will arise whenever a U.S. entity, EIN, tax return, or accountant is discussed.

The concern is understandable: if historical stipends and grants were paid on-chain without conventional W-9s or information returns, will forming an entity now “shine a flashlight” on earlier practices?

The correct answer is neither “yes, therefore never formalize” nor “no, the new entity erases the past.”

## 18.1 Formation is prospective risk management

A service entity can create a clear legal framework for future conduct. It can define roles, liability allocation, tax processes, indemnification, insurance, and recordkeeping from an effective date forward.

## 18.2 Formation does not retroactively erase liability

A new entity is not a time machine. Wyoming's own 2026 DUNA amendments make the principle explicit in the merger context: a merger does not affect personal liability, if any, of a member, administrator, or manager for an obligation incurred before the merger became effective. [2026 Wyo. Sess. Laws ch. 25, § 17-32-127(d)(viii)]

A newly created service entity should therefore never be marketed as a firewall that retroactively makes historical conduct safe.

## 18.3 Formation is not an admission that the past was unlawful

Organizations routinely formalize as they mature. Incorporating today does not concede that yesterday's informal activity was illegal. It means the organization now wants clearer prospective rules.

## 18.4 Historical tax conclusions should not be invented

It is too categorical to say that the IRS automatically treated the historical pDAO as a general partnership or that every past stipend necessarily required a 1099 from a clearly identifiable payer. Civil partnership law and federal tax entity classification are separate analyses. The central historical question is **who, if anyone, was the legally obligated payer or tax entity under the facts then in existence**.

Likewise, the fact that individual recipients reported and paid tax on their stipends is favorable, but it does not automatically cure any payer-side information-reporting, backup-withholding, or entity-return obligation that may have existed.

## 18.5 Do not speculate about audit probability

There is no reliable basis for claiming that entity formation will trigger an audit or that it will not. The appropriate response is to ask counsel whether prospective formation creates any affirmative duty to remediate, disclose, or amend historical activity.

A key counsel question should be:

> If a Rocket Pool service entity begins on a stated effective date, can it expressly assume only prospective service obligations, and does formation, EIN acquisition, or a tax-classification election create any duty to address historical pDAO/GMC stipend or grant practices?

This is the right way to confront the past: understand it, do not misrepresent it, and do not let uncertainty make future structuring impossible.

---

# 19. What Changed Since the Original Legal Research

The earlier Rocket Pool legal paper was rational to be cautious about U.S. structuring. The U.S. regulatory environment was materially more hostile and ambiguous.

That premise has changed enough that domestic options deserve a fresh review.

## 19.1 SEC crypto interpretation in 2026

On March 17, 2026, the SEC issued a Commission-level interpretive release on crypto assets and transactions, effective March 23. The release provides a token taxonomy and addresses protocol staking, among other activities. It is substantially stronger authority than the earlier 2025 staff statements because it is an interpretation of the Commission itself rather than only Division staff guidance.

The Commission's current materials describe specified protocol-staking activities as outside securities transactions and treat specified staking receipt tokens tied to non-security digital commodities as digital tools or, in some circumstances, digital commodities. Ether is expressly treated as a digital commodity in the Commission's framework.

That is highly relevant to Rocket Pool and liquid staking. It does **not** mean “the SEC has ruled that rETH and RPL are securities-law safe in every circumstance.” The interpretation is fact-specific, does not replace Howey, and is not a statute or final judicial decision. RPL presents separate facts from ETH or a pure staking receipt.

The proper conclusion is narrower:

> One of the major reasons earlier Rocket Pool research treated a U.S. entity as unusually dangerous has materially weakened. U.S. entity options should now be evaluated on their actual liability, tax, and privacy merits rather than rejected at the threshold because of the 2022–2024 enforcement environment.

## 19.2 CTA / BOI changed

Earlier drafts worried that forming a U.S. entity would trigger federal Corporate Transparency Act beneficial-ownership reporting. FinCEN's August 11, 2026 final rule now exempts U.S.-created entities from BOI reporting and says U.S. persons do not need to provide BOI under that regime. The rule became effective August 14, 2026.

This does not eliminate IRS responsible-party identification, W-9/W-8 requirements, registered-agent records, banking KYC, or litigation discovery. It does remove a major old objection to domestic formation.

## 19.3 Wyoming DUNA law changed in the opposite direction

At the same time, Wyoming made a change that hurts Rocket Pool's original committee-only DUNA idea: as of July 1, 2026, a DUNA needs 100 consenting members. That means the old idea of simply making seven GMC members and seven IMC members into a DUNA cannot be carried forward unchanged.

The result is a much more interesting current comparison:

- **ordinary UNA** for the small worker group;
- **100+ member DUNA** supporting a small administrator group;
- **DAO LLC** as conventional domestic entity;
- **RMI DAO LLC** as offshore fallback.

---

# 20. Optional Future Governance Reform: A Unified Service Layer

Legal entity formation should not depend on governance reform, but the two issues intersect.

Rocket Pool's committee structure was designed during a higher-energy period with a larger volunteer pool. Recent elections and committee participation suggest that maintaining numerous formally separate roles may become harder over time. A small number of people increasingly perform much of the operational work while elections sometimes struggle to attract more candidates than available seats.

One possible future model is a single annual election for approximately ten **service contributors**. Candidates would run on the explicit premise that they want to perform pDAO service work for modest compensation. Once elected, the group would allocate operational responsibilities internally based on skill and workload:

- some would perform GMC award review;
- some would handle IMC work;
- one might act as treasurer;
- one or more might edit RPIPs;
- one could maintain governance infrastructure or bots;
- one could serve as legal/compliance administrator;
- roles could overlap and change during the term.

The pDAO would remain sovereign. It could remove service workers, change the mandate, override decisions where governance permits, or abolish the structure.

This model could reduce election fatigue and match the reality that a small group of contributors already performs multiple kinds of work. It also maps naturally to a DUNA “administrator” concept.

But it creates legitimate concerns about concentration of operational authority, conflicts, workload, appointment of security roles, compensation, and continuity. It would require significant RPIP changes.

Therefore:

> **The service-layer governance redesign should be evaluated as a separate governance project. A UNA/DUNA should be capable of protecting today's committees first.**

This separation prevents people who dislike one reform from being forced to oppose the other.

---

# 21. Preliminary Findings

The current research supports the following *working findings*, not final recommendations.

### 21.1 The problem is real enough to justify further work

DAO cases do not prove that Rocket Pool committee members are liable, but they make it unreasonable to treat the legal risk as imaginary. Active service participants have more reason to care than passive governance participants.

### 21.2 Whole-pDAO wrapping should not be the default solution

Rocket Pool's pDAO membership, privacy culture, international population, and treasury-control model make whole-pDAO entity formation politically and legally difficult. It should remain a later option rather than a prerequisite for service-worker protection.

### 21.3 The main treasury should remain outside for now

The legal project should solve service-worker risk, not reorganize a small on-chain treasury unnecessarily.

### 21.4 The Wyoming UNA is now a serious candidate

Its two-member threshold and explicit separate-entity/management-participant liability rules make it far more substantial than a casual “club.” Its unanswered indemnification, pseudonymous-validity, and tax-classification questions are narrow enough for counsel.

### 21.5 The DUNA remains the best statutory match, but 100 members are a real cost

If Rocket Pool can assemble and maintain 100 voluntary members, the DUNA offers exceptionally relevant protections: pseudonymous member records, smart-contract governance, administrators, indemnification, advancement, and insurance.

### 21.6 The DAO LLC has become more viable but may still be culturally inferior

Federal BOI reporting is no longer the major obstacle it once was, and federal tax treatment is clear. The challenge is whether conventional LLC management can protect mostly pseudonymous workers without forcing private identity disclosure that those workers refuse.

### 21.7 RMI is a real fallback, not a magic escape

RMI/MiDAO may allocate identity compliance more compatibly with Rocket Pool, but it costs more and does not erase home-jurisdiction tax obligations. It should be researched specifically on U.S. compensation/grant reporting before being treated as a solution.

### 21.8 Compensation/privacy is the pivotal implementation issue

State entity law may permit anonymity more readily than federal payment law. The project succeeds only if it can offer a privacy/compensation menu acceptable to actual service contributors.

### 21.9 The preliminary GMC survey makes a U.S. solution more plausible

Most complete GMC respondents chose private professional disclosure plus full compensation when forced to select a real-world option. That does not settle IMC or future candidate attitudes, but it means the project should not assume universal resistance.

### 21.10 Historical uncertainty should be reviewed, not used as a reason to remain informal forever

Prospective formation does not erase the past and does not admit wrongdoing. Counsel should tell the pDAO whether any historical remediation is required and where the line can be drawn for future operations.

---

# 22. Questions for Wyoming / Entity Counsel

1. **UNA pseudonymity.** Can a Wyoming UNA validly consist of members identified only by blockchain addresses or pseudonyms where mutual consent and governance participation are provable, even if the association itself does not collect their underlying legal names?

2. **UNA management coverage.** Does § 17-22-106 protect GMC/IMC/service workers who act as authorized management participants when the relevant liability is organizational rather than based on their own independent wrongful conduct?

3. **UNA indemnification.** Can a UNA agreement create enforceable indemnification and mandatory advancement of reasonable legal-defense expenses for pseudonymous authorized managers, comparable in practical effect to DUNA § 17-32-125?

4. **UNA insurance.** Can the UNA purchase D&O/E&O or comparable insurance for pseudonymous authorized managers, and what identity information would insurers require?

5. **DUNA membership.** Can the 100-member “mutual consent” requirement be satisfied through wallet-based opt-in or on-chain governance action without collecting members' legal names?

6. **DUNA administrators.** Can DUNA administrators remain pseudonymous to the association and other administrators while one separate responsible person handles tax/compliance identity requirements?

7. **DUNA proof of existence.** Which Wyoming filings, if any, are legally required or practically necessary for a DUNA/UNA that will obtain an EIN, contract with counsel, and buy insurance but will not own real estate?

8. **Public records.** Exactly which names, signatures, or addresses would become publicly searchable under the recommended UNA/DUNA setup?

9. **pDAO separation.** Can the governing principles clearly state that the service entity is not the pDAO, does not represent all pDAO participants, has no control over protocol governance, and owns no main pDAO treasury assets?

10. **Delegated work.** Can the pDAO delegate committee functions to the legal service entity while retaining ultimate governance and removal/override power without making the pDAO itself a member/owner of the entity?

11. **Direct pDAO compensation.** Can service administrators be legally acting for the UNA/DUNA while receiving their stipend directly from a pDAO-controlled smart contract, or would that relationship undermine the entity liability theory?

12. **Past activity.** Can formation documents expressly make the service entity responsible only for obligations arising on or after its effective date, without assuming historical pDAO/committee liabilities?

---

# 23. Questions for Federal Tax Counsel

1. **UNA classification.** What is the default federal tax classification of a Wyoming UNA structured as a nonprofit service association with no economic ownership rights?

2. **UNA corporate election.** Is that UNA an “eligible entity” that can reliably elect association/C-corporation treatment on Form 8832 and thereby avoid member K-1s?

3. **DUNA classification.** What is the current best-supported federal tax classification of a Wyoming DUNA, and can Rocket Pool safely follow the corporate-election model used by existing DUNAs such as Towns Lodge?

4. **Member identity.** If the entity is taxed as a corporation, what member or administrator identity information must the entity, return preparer, or IRS actually receive beyond the SS-4 responsible party?

5. **Responsible party.** Can one genuine legal/compliance administrator serve as the SS-4 responsible party without requiring other pseudonymous administrators to provide legal names merely because of their role?

6. **Worker classification.** Are elected or appointed Rocket Pool service administrators properly treated as independent/nonemployee service providers rather than employees under the contemplated decentralized governance structure?

7. **Sub-$2,000 compensation.** For a U.S. nonemployee paid below the applicable annual 1099-NEC threshold, is there any independent federal reason the service entity must collect a W-9/TIN if no backup withholding or other reportable-payment rule applies?

8. **Flat stipend smart contract.** If the pDAO itself sets a fixed stipend and an autonomous contract pays elected wallet addresses without service-entity discretion, does the service entity become a §6041/§6041A reporting payer merely because the recipients perform services through it?

9. **Unwrapped pDAO payer.** If the service entity is not the payer, is the unwrapped pDAO itself treated as the reporting payer, and if so what practical federal filing obligations follow?

10. **Foreign administrators.** What W-8, source-of-services, 1042-S, and withholding requirements apply to non-U.S. administrators, particularly those performing all services outside the United States?

11. **Genuine grants.** If GMC grant decisions remain outside the entity and grants are paid directly from a pDAO-controlled wallet, under what circumstances could the service entity still be treated as the federal payer/grantor because its administrators selected recipients?

12. **Historical payments.** Who, if anyone, had historical information-reporting or backup-withholding obligations for pre-formation GMC/IMC stipends and grants, given the absence of a formal legal payer?

13. **Prospective formation.** Does obtaining an EIN or making a Form 8832 election create any affirmative duty to disclose, amend, or remediate historical pDAO/committee payment practices?

14. **RMI comparison.** If a Marshall Islands nonprofit DAO LLC pays U.S. persons or pseudonymous foreign persons for services, how do U.S. information-reporting and withholding rules differ from a Wyoming entity?

---

# 24. Practical Next Steps

The next steps should be deliberately incremental.

## Step 1 — Finish committee preference data

Complete the IMC version of the privacy/compensation survey. Keep GMC and IMC cohorts distinguishable rather than pooling them immediately. If possible, later survey RPIP editors, delegates, and people plausibly willing to serve in future service roles.

## Step 2 — Prepare a short counsel packet

Do not send a lawyer the entire historical legal archive first. Send:

- a two-page factual description of pDAO/committee structure;
- the proposed narrow service-layer architecture;
- the UNA/DUNA comparison;
- the compensation/payment diagram;
- the focused questions in Sections 22 and 23.

That should make paid counsel time answer the questions Rocket Pool actually needs.

## Step 3 — Get targeted Wyoming and tax answers before selecting an entity

The project should not vote on “form a DUNA” before resolving:

- UNA pseudonymous validity;
- UNA indemnification/advancement;
- UNA/DUNA federal classification;
- payment reporting;
- foreign administrator treatment;
- historical transition risk.

## Step 4 — Research RMI only if necessary

If tax counsel concludes that meaningful U.S.-entity compensation requires identity disclosure that committees will not tolerate, perform a targeted RMI/MiDAO analysis focused on **compensated pseudonymous workers and grants**, not another generic offshore-jurisdiction survey.

## Step 5 — Separate legal formation from governance reform

If a service entity is viable under current committee rules, form it that way first. A later RPIP can consolidate elections and service roles if the community wants it.

---

# 25. Closing Perspective

Rocket Pool's legal problem is not that it failed to become a conventional company. The protocol was deliberately built around permissionless software, independent Node Operators, and decentralized governance. Turning that into a conventional management corporation would solve the wrong problem.

The problem is more specific. A decentralized protocol still depends on human beings willing to perform mundane, visible, and sometimes legally consequential work. Those people should not have to pretend that the work has no legal character simply because the protocol is decentralized. Nor should the solution require the whole pDAO to surrender privacy or on-chain sovereignty.

The design target is therefore modest:

> **A legal shell around service, not a legal owner above governance.**

If Wyoming's UNA is strong enough, Rocket Pool may be able to accomplish that with a very small association. If the DUNA's explicit administrator and indemnification protections are worth the 100-member burden, a voluntary service DUNA may be better. If U.S. tax identity requirements remain incompatible with contributor culture, RMI or another non-U.S. model may deserve the cost. If none of those are worth the tradeoffs, the pDAO can knowingly choose to remain informal while strengthening personal LLC, indemnification, insurance, and legal-defense measures.

What the pDAO should avoid is confusing “we chose not to form an entity after understanding the tradeoffs” with “there is no legal problem because we never formed one.”

The project has now narrowed enough that the remaining uncertainty is not an excuse for another year of abstract entity shopping. The next useful information should come from two places: **the people who actually serve, and qualified counsel answering a short list of concrete questions.**

---

# Appendix A — Historical Consultation Record

The legacy Rocket Pool legal-research paper contains internal summaries of consultations and discussions with several lawyers or legal-structure specialists. These notes are useful as history but should **not** be cited publicly as current legal opinions without verifying the original communications and obtaining permission where appropriate.

The internal notes record, in substance:

- **Croke Fairchild / Michael Frisch (November 2024):** discussion of pDAO and committee liability, general-partnership exposure, personal LLCs, indemnification, compliance procedures, committee entity options, and broader structures such as Cayman. The notes emphasized that active committee/delegate participants may have more exposure than conventional shareholders and that future risk can be reduced even if past conduct cannot be retroactively cured.
- **MetaLeX:** a layered framework separating pDAO, committees, and individuals; committee formalization; Cayman/BORG concepts; and limits of individual wrappers where documentation or timing is poor.
- **MME:** Swiss Association and foundation models, including flexible association governance and models that distinguish tokenholder signaling from legal-entity execution.
- **William Brown / ENSPunks:** personal LLCs for active individuals, DUNA possibilities for committees or a DAO, and concern that an entity formed later does not automatically absorb liabilities incurred before formation.

These consultations are one reason the project should not be presented as AI inventing a theoretical legal problem. The exact current conclusions, however, should come from fresh counsel review under 2026 law.

---

# Appendix B — Preliminary GMC Privacy/Compensation Survey

**Status:** GMC-only first round; IMC pending.  
**Submissions:** 8 total, 7 complete.

### Private identity disclosure (select all that apply, 7 complete responses)

- One designated pDAO legal/compliance person: **6/7**
- Small pDAO compliance group: **4/7**
- Outside lawyer/accountant: **5/7**
- Third-party payment/compliance provider: **5/7**
- “Would not provide my legal identity to anyone”: **2/7**, with one of those respondents also selecting conditional disclosure options

### Small stipend while fully pseudonymous (< approximately $2,000/year)

- Yes, same expected contribution: **1/7**
- Yes, but likely closer to minimum expected work: **2/7**
- Maybe, depending on role/workload: **4/7**
- No: **0/7**

### Completely unpaid while pseudonymous

- Yes, same expected contribution: **2/7**
- Yes, but likely closer to minimum expected work: **0/7**
- Maybe, depending on role/workload: **3/7**
- No: **2/7**

### Differential compensation based on privacy choice

- Comfortable: **5/7**
- Accept, but likely reduce work: **1/7**
- Unsure: **0/7**
- Would not serve because unfair: **0/7**
- Oppose system even if personally taking full stipend: **1/7**

### Most likely actual choice

- Private identification to trusted outside professional + full stipend: **5/7**
- Remain pseudonymous + smaller stipend: **1/7**
- Remain pseudonymous + no stipend: **0/7**
- Only serve if another privacy-preserving method exists: **0/7**
- Decline to serve: **1/7**

These results should not be generalized beyond the current GMC cohort. They are useful because they directly measure the behavior of existing service participants rather than abstract community opinion.

---

# Appendix C — Key Authorities and Current Sources

This is a working source list, not a formal Bluebook bibliography.

### Rocket Pool governance
- RPIP-23, **pDAO Charter**.
- RPIP-33, **Implementation of an On-Chain pDAO**.
- RPIP-36, **Committee Membership Record**.
- RPIP-41, **Committee Stipends**.
- RPIP-76, **Updating of Grants Management Committee 3 – Membership Reduction**.
- RPIP-81, **Rebalance RPL Inflation for Protocol Funding**.
- RPIP-84, **pDAO Signaling Governance**.
- RPIP-86, **Saturn 2 Upgrade**.

### DAO cases
- *Sarcuni v. bZx DAO*, S.D. Cal., order on motions to dismiss, Mar. 27, 2023.
- *Samuels v. Lido DAO*, N.D. Cal., order on motions to dismiss, Nov. 18, 2024.
- *Samuels v. Lido DAO*, N.D. Cal., order dismissing conditional counterclaims, Apr. 9, 2025.
- *CFTC v. Ooki DAO*, N.D. Cal., default judgment, June 8, 2023.

### Wyoming
- Wyoming Unincorporated Nonprofit Association Act, Wyo. Stat. §§ 17-22-101 through -115.
- Wyoming Decentralized Unincorporated Nonprofit Association Act, Wyo. Stat. §§ 17-32-101 through -129.
- 2026 Wyoming Senate File 22 / Session Laws ch. 25, effective July 1, 2026.
- Wyoming Decentralized Autonomous Organization Supplement, Wyo. Stat. ch. 31.

### Federal tax / reporting
- IRS, 2026 Instructions for Forms 1099-MISC and 1099-NEC.
- IRS, Publication 1099 (2026), General Instructions for Certain Information Returns.
- IRS, Digital Asset Transaction FAQs, including services paid in digital assets.
- IRS, Instructions for Form SS-4.
- IRS, Form 8832 / Entity Classification guidance.
- IRS, Publication 515 (2026), withholding for nonresident aliens and foreign entities.

### Federal regulatory environment
- SEC Release 33-11412 / 34-105020, **Application of the Federal Securities Laws to Certain Types of Crypto Assets and Certain Transactions Involving Crypto Assets**, issued Mar. 17, 2026, effective Mar. 23, 2026.
- FinCEN, final 2026 BOI reporting rule, effective Aug. 14, 2026.

### DUNA implementation examples
- Towns Lodge public formation, financial, and tax materials, including its disclosed Form 8832 corporate election and Form 1120 filing approach. This is an implementation example, not binding tax authority.

### Marshall Islands / MiDAO
- Republic of the Marshall Islands corporate registry materials on LLCs, non-resident entity tax treatment, and economic-substance reporting.
- MiDAO 2026 documentation on DAO LLC registration, KYC/KYB, beneficial-owner reporting, annual filings, and pricing. MiDAO is a service provider and expressly states that it is not a law firm; its tax/legal claims should be independently verified before reliance.

---

# Appendix D — Claims That Should Not Appear in Future Summaries Without Qualification

To prevent old drafts from reintroducing overstatements, the following shorthand claims should be avoided:

- **“Rocket Pool is a general partnership.”**  
  Better: Rocket Pool faces factual and jurisdiction-dependent risk of partnership or association characterization under default law.

- **“Every pDAO member could be jointly and severally liable.”**  
  Better: some DAO cases have allowed partnership theories at the pleading stage; other cases distinguish meaningful management participation from passive tokenholding.

- **“RPL and rETH are not securities.”**  
  Better: the 2026 SEC interpretation materially improves the federal securities-law environment for specified crypto assets, protocol staking, and staking receipt tokens; RPL and every rETH arrangement still require fact-specific analysis.

- **“A DUNA requires no doxxing.”**  
  Better: Wyoming expressly permits a DUNA not to maintain members' names/addresses, but federal tax, EIN, insurance, banking, payment, and legal-process requirements can identify particular people privately.

- **“A DUNA fixes historical liability.”**  
  Better: formation improves prospective structure but does not retroactively erase obligations or personal liability already incurred.

- **“Committee stipends can just be called grants.”**  
  Better: tax treatment follows substance; payments earned for committee services are compensation regardless of label.

- **“Below $2,000 means tax-free.”**  
  Better: the 2026 $2,000 threshold generally concerns information reporting; the recipient still has taxable income.

- **“Offshore means outside U.S. law.”**  
  Better: an offshore entity may change entity-level jurisdiction and compliance, but U.S. participants remain subject to applicable U.S. tax and other law.

---

**End of Draft 0.1**
