# Working Research Memo

## Committee/Service Entity Options for the Rocket Pool pDAO

**September 17, 2026 — research draft**

### Purpose and assumptions

This memo considers a deliberately narrow objective: **protect the people performing operational work for Rocket Pool's pDAO without placing the entire pDAO into a legal entity.**

For this analysis, the desired architecture is:

* the broader pDAO remains outside the service entity;
* the main pDAO treasury remains controlled directly by on-chain pDAO governance;
* existing or future GMC/IMC operating reserves could potentially belong to the service entity;
* the entity performs delegated administrative functions for the pDAO;
* most service workers must be able to remain pseudonymous **even to lawyers, accountants and service providers**;
* one identifiable person might privately identify to the IRS, counsel, accountants, etc., if unavoidable, preferably without public disclosure;
* costs must be modest; and
* legal structuring should not require the proposed consolidation of GMC/IMC/editors/etc. into a new service group, although it should accommodate that later.

The three structures considered are an ordinary Wyoming UNA, an opt-in Wyoming DUNA with 100+ members, and a Wyoming DAO LLC.

This is research to frame counsel questions, not a substitute for Wyoming and federal tax counsel.

---

## 1. Preliminary finding: the pDAO does not have to be the entity

Nothing I've found makes “wrap the entire pDAO” the necessary consequence of protecting its committees.

In fact, Wyoming's DUNA statute expressly separates **members** from **administrators**. An administrator can be a member or nonmember authorized to perform administrative or operational tasks at the direction of the membership. Its governing principles can include smart contracts and enacted governance proposals. ([Wyoming Legislature][4])

That gives us a legally coherent conceptual model:

**pDAO → delegates defined functions → service entity → authorized people perform those functions**

The main treasury need not necessarily become property of the service entity merely because the pDAO delegates work to it. Both Wyoming UNAs and DUNAs are legally capable of owning their own personal property and entering contracts, so a service entity could potentially own only the funds actually allocated to GMC/IMC operations. ([Wyoming Legislature][4])

This is one of the important distinctions from the original big legal paper: we don't have to choose between *no entity* and *entity owning all Rocket Pool governance and assets*.

---

# 2. Ordinary Wyoming UNA

A Wyoming Unincorporated Nonprofit Association is strikingly simple. It consists of **two or more members joined by mutual consent for a common nonprofit purpose**. A member is someone who can participate in selecting management or developing association policy. ([Wyoming Legislature][4])

So a ten-person Rocket Pool service group fits the basic statutory concept naturally. There is no artificial 100-person membership population to manufacture.

### Liability protection

This is the most important discovery.

Wyoming doesn't merely recognize a UNA as an informal club. It expressly makes the UNA **a legal entity separate from its members for contract and tort liability**. It further says a person isn't liable for an association contract or tort merely because the person is a member or is authorized to participate in management. A judgment against the UNA is not by itself a judgment against a member. ([Justia Law][5])

For our use case, that language is surprisingly good. It isn't just shielding passive members; it specifically mentions people **authorized to participate in management**.

That gets much closer to the GMC problem than I expected.

### Formation and bureaucracy

The statute does not use the normal LLC incorporation model. The association arises from the members' mutual consent and common nonprofit purpose. It **may** file a statement appointing an agent for service of process, but that filing is not phrased as a prerequisite to legal existence. The filing fee is only $5. ([Wyoming Legislature][4])

I do not see an LLC-style annual report requirement in Chapter 22.

This potentially makes the UNA extraordinarily inexpensive from a state-law standpoint. The real expense would be having counsel draft the association agreement properly, obtaining tax advice, accounting, perhaps an agent, and insurance—not Wyoming franchise fees.

### Privacy

Here's where the UNA is simultaneously promising and less certain than the DUNA.

Nothing in Chapter 22 that I found requires the association to submit a member list to Wyoming. The optional service-agent filing names the agent and is signed by someone authorized to manage the association. ([Wyoming Legislature][4])

But the UNA statute also **doesn't expressly say** that the association need not collect members' legal identities.

The DUNA statute does.

So I am comfortable saying a UNA does not appear to have a statutory member-registry filing requirement. I am **not yet comfortable saying that ten completely pseudonymous Discord identities can unquestionably constitute the UNA and its management without anybody knowing who they are**.

That is a very good question for Wyoming counsel.

### Indemnification

The UNA statute lacks the DUNA's unusually explicit indemnification, advancement-of-defense-costs and insurance provisions.

The UNA is capable of contracting and holding property, so it may well be possible to put contractual indemnification into the association agreement and buy insurance. But I haven't found a Chapter 22 equivalent to DUNA §17-32-125, and I don't want to infer that its scope is identical.

This is probably the biggest substantive disadvantage of UNA relative to DUNA for *our* purpose. The entire reason we're doing this is to protect people if litigation occurs, so explicit statutory legal-defense machinery has real value.

### Tax problem

The federal classification is not obvious.

“Nonprofit” is a Wyoming state-law classification; it **does not automatically make the organization federally tax exempt**. ([IRS][6])

Federal classification rules normally make many domestic multi-member business entities partnerships unless they qualify or elect to be associations taxed as corporations. But the members of a nonprofit UNA aren't conventional equity owners sharing profits. The IRS recognizes unincorporated associations as legal forms that can, for example, seek nonprofit tax exemption. ([IRS][7])

I would not assume that a Rocket Pool UNA defaults to partnership treatment, nor that Form 8832 unquestionably solves it, without tax counsel.

**This is a major unresolved item.**

---

# 3. Opt-in Wyoming DUNA

The DUNA is now a strange fit for Rocket Pool because the 2026 legislature changed the threshold to **at least 100 members joined by mutual consent**. The agreement can be written or inferred from conduct. ([Wyoming Legislature][3])

If membership later falls below 100, a qualifying DUNA automatically becomes an ordinary Wyoming UNA unless its governing principles specify otherwise. ([Wyoming Legislature][3])

That latter provision matters: Wyoming itself sees the UNA and DUNA as points on the same organizational continuum rather than completely unrelated structures.

### We do not need 100 committee members

The more sensible Rocket Pool DUNA design would be:

**100+ voluntarily opted-in community members**
↓ elect/authorize
**roughly 10 administrators**
↓ perform
**GMC / IMC / editing / administrative functions**

Those 100 members need not be the entire pDAO.

Most importantly, the statutory definition requires **mutual consent**, which reinforces my view that we should not simply declare all RPL stakers DUNA members against their wishes. ([Wyoming Legislature][4])

A voluntary opt-in could perhaps be as simple as an on-chain acknowledgement or defined governance action. The exact mechanism should be blessed by Wyoming counsel.

### Privacy is where DUNA really distinguishes itself

The DUNA statute now says explicitly:

> a DUNA is not obligated to collect and maintain a list of members or individual member information, including their names or addresses.

That is unusually well aligned with Rocket Pool. ([Wyoming Legislature][4])

It also allows blockchain governance and smart contracts directly in the governing principles. ([Wyoming Legislature][4])

That means the 100-member requirement sounds more alarming from a privacy perspective than it actually is. We don't necessarily need:

> “100 people, please email Jason your driver's license.”

We may instead need:

> “100 governance identities affirmatively consent to membership according to the governing principles.”

The latter sounds feasible.

### Liability protection is extremely well tailored

The DUNA is a separate legal entity. Wyoming specifically says that liability does not attach merely because someone is:

* a member,
* an administrator,
* authorized to participate in management, or
* treated as a member.

A judgment against the DUNA isn't automatically a judgment against its member or administrator. ([Wyoming Legislature][4])

This is remarkably close to exactly what we're trying to accomplish.

### Indemnification and defense expenses

This is probably the DUNA's strongest advantage over an ordinary UNA.

The statute expressly permits indemnifying members and administrators for liabilities incurred through activities on behalf of the DUNA. It also permits **advancing attorneys' fees before the litigation is resolved**, subject to statutory conditions, and buying insurance for members and administrators. ([Wyoming Legislature][4])

For a project whose central objective is basically:

> “Don't make volunteer GMC members fund their own defense when somebody sues Rocket Pool,”

that is very compelling statutory machinery.

### The service workers do not necessarily need to be DUNA members

The definition of administrator expressly allows an administrator to be a **nonmember**. ([Wyoming Legislature][4])

That is useful.

The 100-person population could exist principally to constitute the decentralized association and exercise its membership governance. The ten people actually doing operations can have the separate status of administrators.

And those administrators are expressly included in the liability and indemnification provisions.

### One private identity may still be necessary

State law does not create a federal tax identity.

To obtain an EIN, the IRS generally requires a **natural-person “responsible party”** who ultimately controls or exercises effective control over the entity and its assets. The IRS requires that person's name and SSN/ITIN; a mere nominee cannot serve. ([IRS][8])

So the model you suggested remains plausible:

**100+ pseudonymous members**
**~10 pseudonymous administrators**
**1 actual responsible person privately known to IRS/counsel/accountant**

But that responsible person has to have a genuine role. We can't hire a random person solely to lend us a Social Security number.

This is exactly where a “Legal/Compliance Administrator” role could make sense—and why compensation for assuming that administrative burden isn't unreasonable.

### Public versus private doxxing

The DUNA statute says it **may** file an agent-for-service statement. That filing names an agent and requires signature by someone authorized to administer the DUNA. ([Wyoming Legislature][4])

It therefore looks possible at the statutory level to create a DUNA without a conventional public articles-of-organization filing.

But I want counsel to answer whether foregoing that filing creates practical problems obtaining an EIN, insurance, banking, contracts or proof of legal existence.

The goal would be:

**one person privately identified → acceptable**

rather than:

**one person publicly identified in searchable Wyoming records → avoid if possible**

### Federal tax is the major unresolved DUNA problem

This is more unsettled than some DUNA marketing materials imply.

In 2024, tax lawyers from Gibson Dunn formally asked Treasury and the IRS to issue guidance specifically answering whether Wyoming DUNAs are automatically corporations, partnerships, or eligible entities capable of making a Form 8832 election. Their submission says existing federal tax classification of DUNAs is unclear. ([Regulations.gov][9])

I have not found subsequent precedential IRS guidance resolving that issue.

On the other hand, actual DUNAs are now proceeding with corporate taxation. Towns Lodge, for example, says its administrator obtained an EIN and filed Form 8832 electing **C-corporation taxation**, explicitly avoiding tax-exempt treatment. It originally existed as a three-member Wyoming UNA and then became a DUNA after reaching 100 members. ([Towns Lodge][10])

That's quite relevant to us because it is almost a live demonstration of:

**small UNA → 100 members → DUNA → Form 8832 → taxable corporation**

But this is a practitioner's implementation, not an IRS revenue ruling. We should treat it as evidence that sophisticated people are doing this, not as proof that the IRS has definitively approved every step.

If corporate treatment works, it solves one enormous Rocket Pool concern:

**no K-1s to 100 pseudonymous members.**

That's probably essential.

---

# 4. Wyoming DAO LLC

The DAO LLC is substantially more familiar from a tax perspective.

Wyoming expressly allows one or more people to form a DAO LLC by filing articles with the Secretary of State. It can use smart-contract management, and the articles must identify the smart contract used to operate it. ([Wyoming Legislature][11])

### Liability and indemnification

The underlying Wyoming LLC statute provides the familiar LLC liability shield: company liabilities do not become liabilities of members or managers merely because they act as members or managers. Wyoming also expressly requires indemnification of qualifying members/managers for liabilities incurred through company activities and permits insurance. ([Wyoming Legislature][12])

That's strong and conventional.

### Tax treatment is much clearer

A domestic multi-member LLC defaults to partnership treatment, but it can file Form 8832 and elect corporate treatment. The IRS explains this explicitly. ([IRS][13])

So if avoiding K-1s is mandatory, a C-corporation election is a well-established route for an LLC.

That's a major advantage over the UNA/DUNA uncertainty.

### But privacy is the problem

Every Wyoming LLC needs a registered agent. That agent must maintain current names and addresses for LLC managers and people serving in similar capacities, plus a natural-person communications contact. The state can compel production of those records, although records obtained by the Secretary of State are generally confidential except for subpoena/law-enforcement circumstances. ([Wyoming Legislature][14])

This is much better than **publicly listing everybody**, but it conflicts with the hard constraint you just gave me:

> Most Rocket Pool workers will not privately reveal their identities at all.

If we call all ten service workers “managers,” the DAO LLC likely doesn't work culturally.

Could we instead have:

**one known manager + ten pseudonymous agents/contractors?**

Possibly.

But that weakens the reason for choosing the LLC. The Wyoming statutory indemnification provision expressly concerns members/managers, whereas DUNA law expressly addresses administrators and management participants. And an agent remains potentially personally responsible for the agent's own tortious conduct even when acting for a principal.

We'd be taking a conventional LLC and engineering around its conventional management model specifically because Rocket Pool doesn't behave conventionally.

### Bureaucracy

The DAO LLC has an actual state filing:

* $100 formation fee;
* annual report;
* minimum $60 annual Wyoming license fee;
* registered agent; and
* associated maintenance. ([Wyoming Secretary of State][15])

These aren't remotely Cayman-level expenses, but they're more bureaucracy than the association statutes themselves impose.

The old BOI objection, however, is gone. FinCEN's August 2026 final rule permanently exempts U.S.-created entities from federal CTA beneficial-ownership reporting. ([FinCEN.gov][16])

So the DAO LLC has become significantly more attractive than it was when your original paper was written—just not necessarily attractive enough under Rocket Pool's exceptionally strict privacy culture.

---

# 5. Comparative picture

| Issue                                            | Wyoming UNA                 | Opt-in DUNA                                               | DAO LLC                                                   |
| ------------------------------------------------ | --------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| Minimum population                               | **2**                       | **100**                                                   | 1+                                                        |
| Need entire pDAO                                 | No                          | No                                                        | No                                                        |
| Separate legal person / liability shield         | Yes                         | Yes                                                       | Yes                                                       |
| Explicit protection for management participants  | **Yes**                     | **Yes, incl. administrators**                             | Primarily member/manager framework                        |
| Explicit statutory indemnification               | Not in Ch. 22               | **Excellent**                                             | Excellent for members/managers                            |
| Advance defense fees                             | Not expressly in Ch. 22     | **Expressly authorized**                                  | More conventional LLC rules                               |
| Insurance expressly authorized                   | Needs validation            | **Yes**                                                   | Yes                                                       |
| Smart-contract governance expressly supported    | Not specifically            | **Yes**                                                   | Yes                                                       |
| State member-name filing                         | None found                  | None; statute expressly disclaims member-list requirement | No ordinary public member list, but RA holds manager data |
| Members can remain privately pseudonymous        | **Possibly; needs counsel** | **Strong statutory support**                              | More difficult for managers                               |
| 100-person membership problem                    | None                        | **Major complication**                                    | None                                                      |
| Federal tax classification                       | **Needs research/counsel**  | **Still legally novel**                                   | **Well established**                                      |
| Corporate tax election                           | Plausible but confirm       | Used in practice; IRS guidance still unclear              | Established Form 8832 route                               |
| K-1 risk if mishandled                           | Potential                   | **Potentially disastrous with 100 members**               | Easily avoided by corporate election                      |
| State formation bureaucracy                      | Extremely light             | Extremely light                                           | Conventional filing/reporting                             |
| State statutory fee burden                       | $5 optional agent statement | $5 optional agent statement                               | $100 + ≥$60/year                                          |
| Compatibility with hard pseudonymity requirement | **Promising**               | **Very promising**                                        | Questionable                                              |

The **interesting comparison is definitely UNA versus DUNA now**. The DAO LLC shouldn't be discarded, but your private-pseudonymity requirement takes away one of its biggest practical advantages.

---

# 6. The compensation/privacy problem remains common to all three

This is now the most important federal issue.

Suppose the legal architecture becomes:

**pDAO delegates grant administration to Service DUNA**
→ DUNA administrators attend meetings/sign transactions
→ existing RPIP determines compensation
→ GMC multisig sends payment directly from existing funds to each administrator's wallet.

It would be tempting to say:

> “The DUNA didn't pay them, so no W-9.”

But the IRS says a person can become the information-reporting **payor even when another person is the source of the funds** if that intermediary performs management or oversight functions in connection with the payment. ([IRS][1])

Therefore, the precise allocation of authority matters.

One potentially better architecture would have the pDAO's RPIP **completely determine compensation mechanically**, with the service entity having no discretion over amount or eligibility. Whether that is sufficient is a tax-counsel question, but it is considerably cleaner than having the DUNA itself decide “Jason did enough work this month to earn $400.”

We should not solve this by calling $400 a grant. We should solve it by determining **who the federal tax payer actually is**.

There is a notable irony here: formalizing the committees could make an existing reporting question more visible rather than create the underlying income-tax obligation. Committee members already receive taxable compensation; the wrapper merely introduces an identifiable U.S. organization capable of having reporting obligations.

That shouldn't automatically dissuade us from forming one, but we need to know the answer before implementation.

---

# 7. One possibility I now think deserves serious design work

A hybrid **UNA → DUNA** path may be more interesting than I expected.

Wyoming's own 2026 law effectively contemplates movement between the two structures. We even have a current real-world example: Towns Lodge says it began as a three-member Wyoming UNA and transitioned into a DUNA once it reached 100 members. ([Towns Lodge][10])

Rocket Pool could theoretically begin much more modestly:

**Phase 1**

pDAO remains unwrapped
→ forms Rocket Pool Service UNA
→ actual committee/service workers constitute its membership/management
→ pDAO formally delegates defined GMC/IMC/etc. functions
→ main treasury stays outside
→ only designated operating assets enter UNA

Then, **if** counsel concludes DUNA's explicit administrator anonymity, indemnification and insurance provisions materially improve protection enough to justify it:

**Phase 2**

restructure/transition into DUNA
→ recruit 100+ voluntary pseudonymous members
→ service workers become administrators
→ association continues operational role

I don't yet know whether this is preferable to forming the DUNA immediately. But unlike “create a Swiss entity now and migrate everything later,” Wyoming law makes UNA/DUNA transition conceptually native to the statutory system.

And critically, **we could abandon Phase 2 altogether** if counsel says ordinary UNA protection is sufficient.

For Rocket Pool's treasury and manpower situation, that's attractive.

---

# 8. What I would ask paid counsel

We've now narrowed this enough that I would not hire someone for an open-ended “What entity should Rocket Pool use?” consultation. I would give counsel the architecture and ask very specific questions:

1. Can a Wyoming UNA composed of pseudonymous blockchain identities validly exist where the members have mutually consented through signed/on-chain governance records but their underlying natural-person identities are not collected?
2. Does §17-22-106 protect those pseudonymous committee members when they perform GMC/IMC work **as authorized management participants of the UNA**, and can the UNA validly provide contractual indemnification, defense advances and insurance comparable to a DUNA?
3. Can a DUNA's 100 members be established through pseudonymous wallet-based opt-in without collecting legal names, consistent with the statutory mutual-consent requirement?
4. Can the administrators likewise remain unknown by legal name to the association, apart from one genuine IRS responsible party?
5. Is there any reason the optional Wyoming service-agent filing becomes practically necessary, and if so, exactly whose identity becomes public?
6. What is the correct federal tax classification of a Wyoming UNA and DUNA? Can each reliably elect association/C-corporation treatment with Form 8832 without identifying all members and without issuing member K-1s?
7. If pDAO governance independently authorizes and mechanically calculates committee compensation and an existing on-chain multisig pays the wallets directly, does the UNA/DUNA become a §6041 information-reporting payor merely because those recipients perform their committee work on behalf of the association?
8. If yes, is there any legitimate structure that protects pseudonymous administrators without requiring the service entity to collect W-9/W-8 information from them?
9. Can a DAO LLC instead use one identified manager and pseudonymous authorized agents while extending meaningful liability protection and indemnification to those agents, or does that defeat the purpose compared with a UNA/DUNA?
10. Can the main pDAO and its treasury remain expressly outside the service entity while GMC/IMC operational reserves, contracts, insurance and legal-defense assets are held by the entity without undermining the liability separation?

Those questions are concrete enough that counsel should be able to spend their time answering actual legal uncertainties rather than learning the entire history of Rocket Pool.

---

## Where I think we stand now

I would **not** reopen wrapping the whole pDAO yet.

The 100-member DUNA amendment initially looked like it might force us in that direction. After this research, I don't think it does.

The ordinary UNA is much more substantial than I realized: Wyoming expressly gives it separate legal personality and shields not just passive members but people authorized to participate in management. That makes a **committee-only UNA a serious option**, not a consolation prize. ([Justia Law][5])

The DUNA remains attractive because Wyoming has essentially taken that UNA base and added exactly the DAO-specific things Rocket Pool likes: pseudonymous membership, smart-contract governance, administrators, explicit indemnification, advance defense costs and insurance. Its problem is now mostly the artificial requirement to maintain 100 consenting members and the unresolved federal tax/reporting machinery. ([Wyoming Legislature][4])

The DAO LLC has the clearest conventional federal tax path, but requiring private manager identification cuts directly against what you've now told me is a non-negotiable cultural constraint. The disappearance of CTA/BOI reporting makes it better than our old research suggested, but it doesn't solve that registered-agent problem. ([Wyoming Legislature][14])

And one thing has become clearer than when we started: **we shouldn't distort the operational reality merely to avoid tax paperwork.** Calling committee compensation “grants” when it is calculated from attendance and transaction signing would weaken rather than strengthen the credibility of the structure. The better goal is to find out whether the association can protect the people doing the work while keeping the existing pDAO compensation mechanism legally outside the association—or, if not, exactly how much private identification federal tax law actually requires.

I think the next research step should be to go deeper on **ordinary UNA indemnification and federal tax classification**, because those are the two places where the cheap two-member structure currently has question marks. If those answers are favorable, the 100-member DUNA problem may turn out not to be a problem we need to solve at all.

[1]: https://www.irs.gov/instructions/i1099mec?utm_source=chatgpt.com "Instructions for Forms 1099-MISC and 1099-NEC (12/2026) | Internal Revenue Service"
[2]: https://www.irs.gov/instructions/i990si?utm_source=chatgpt.com "Instructions for Schedule I (Form 990) (12/2024) | Internal Revenue Service"
[3]: https://www.wyoleg.gov/2026/Enroll/SF0022.pdf "26LSO-0058"
[4]: https://wyoleg.gov/statutes/compress/title17.pdf "Title 1"
[5]: https://law.justia.com/codes/wyoming/title-17/chapter-22/section-17-22-106/?utm_source=chatgpt.com "Wyoming Statutes § 17-22-106 (2025) - Liability in Tort and Contract. :: 2025 Wyoming Statutes :: U.S. Codes and Statutes :: U.S. Law :: Justia"
[6]: https://www.irs.gov/charities-non-profits/frequently-asked-questions-about-applying-for-tax-exemption?utm_source=chatgpt.com "Frequently asked questions about applying for tax exemption | Internal Revenue Service"
[7]: https://www.irs.gov/instructions/i1023?utm_source=chatgpt.com "Instructions for Form 1023 (12/2024) | Internal Revenue Service"
[8]: https://www.irs.gov/businesses/small-businesses-self-employed/responsible-parties-and-nominees?utm_source=chatgpt.com "Responsible parties and nominees | Internal Revenue Service"
[9]: https://downloads.regulations.gov/IRS-2024-0009-0052/attachment_1.pdf?utm_source=chatgpt.com "Michael J. Desmond"
[10]: https://townslodge.com/docs/q1-2026?utm_source=chatgpt.com "Towns Lodge | Towns Lodge - Q1 2026 Financial Statements and Tax Update"
[11]: https://wyoleg.gov/NXT/gateway.dll/Statutes%2F2021%20Titles%2F879%2F1045%2F1046?utm_source=chatgpt.com "ARTICLE 1 - PROVISIONS"
[12]: https://wyoleg.gov/InterimCommittee/2009/10lso-0044w2.pdf?utm_source=chatgpt.com "Microsoft Word - 00000245.011"
[13]: https://www.irs.gov/businesses/small-businesses-self-employed/llc-filing-as-a-corporation-or-partnership?utm_source=chatgpt.com "LLC filing as a corporation or partnership | Internal Revenue Service"
[14]: https://wyoleg.gov/NXT/gateway.dll/2022%20Wyoming%20Statutes/2022%20Titles/898/1039?utm_source=chatgpt.com "CHAPTER 28 - REGISTERED OFFICES AND AGENTS"
[15]: https://sos.wyo.gov/Forms/Business/LLC/DAOLLC-ArticlesOrganization.pdf?utm_source=chatgpt.com "DAO LLC-Articles of Organization"
[16]: https://www.fincen.gov/boi?utm_source=chatgpt.com "Beneficial Ownership Information Reporting | FinCEN.gov"
