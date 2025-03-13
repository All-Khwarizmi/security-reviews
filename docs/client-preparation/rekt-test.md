One of the biggest challenges for blockchain developers is objectively assessing their security posture and measuring how it progresses. To address this issue, a working group of Web3 security experts, led by Trail of Bits CEO Dan Guido, met earlier this year to create a simple test for profiling the security of blockchain teams. We call it the Rekt Test.

The Rekt Test is modeled after The Joel Test. Developed 25 years ago by software developer Joel Spolsky, The Joel Test replaced a Byzantine process for determining the maturity and quality of a software team with 12 simple yes-or-no questions. The blockchain industry needs something similar because today’s complex guidance does more to frustrate than to inform.

The Rekt Test focuses on the simplest, most universally applicable security controls to help teams assess security posture and measure progress. The more an organization can answer “yes” to these questions, the more they can trust the quality of their operations. This is not a definitive checklist for blockchain security teams, but it’s a way to start an informed discussion about important security controls.

At the Gathering of Minds conference earlier this year, a group of industry leaders were challenged to address the lack of cybersecurity standards in the blockchain ecosystem. One of these discussions was led by Dan Guido, CEO of Trail of Bits. Other participants included Nathan McCauley (Anchorage Digital), Lee Mount (Euler Labs), Shahar Madar (Fireblocks), Mitchell Amador (Immunefi), Nick Shalek (Ribbit Capital), and others. Through their discussions, the Rekt Test was created:

The Rekt Test
Do you have all actors, roles, and privileges documented?
Do you keep documentation of all the external services, contracts, and oracles you rely on?
Do you have a written and tested incident response plan?
Do you document the best ways to attack your system?
Do you perform identity verification and background checks on all employees?
Do you have a team member with security defined in their role?
Do you require hardware security keys for production systems?
Does your key management system require multiple humans and physical steps?
Do you define key invariants for your system and test them on every commit?
Do you use the best automated tools to discover security issues in your code?
Do you undergo external audits and maintain a vulnerability disclosure or bug bounty program?
Have you considered and mitigated avenues for abusing users of your system?
The landscape of blockchain technology is diverse, extending beyond blockchains to include decentralized protocols, wallets, custody systems, and more, each with unique security nuances. The subsequent explanations of the Rekt Test questions reflect the consensus of best practices agreed to by this group, and are by no means exhaustive or absolute. The intent of the Rekt Test is not to establish rigid benchmarks but to stimulate meaningful conversations about security in the blockchain community. Thus, consider this interpretation as a stepping stone in this critical dialogue.

1. Do you have all actors, roles, and privileges documented?

Comprehensive documentation of all actors, roles, and privileges affecting the blockchain product is crucial, as this clarifies who can access system resources and what actions they are authorized to perform. Actors refer to entities interacting with the system; roles are predefined sets of permissions assigned to actors or groups; and privileges define specific rights and permissions.

Thorough documentation of these entities facilitates comprehensive testing, allowing developers (and external auditors) to identify security gaps, improper access controls, the degree of decentralization, and potential exposure in specific compromise scenarios. Addressing these issues enhances the overall security and integrity of the system. The documentation also serves as a reference point for auditors to compare the actual access privileges with the documented ones, identify any discrepancies, and investigate potential security risks.

2. Do you keep documentation of all the external services, contracts, and oracles you rely on?

Interactions with external smart contracts, oracles, and bridges are fundamental to many key functionalities expected from blockchain applications. A new blockchain application or service may also rely on the assumed security posture of a financial token developed outside of your organization, which increases its complexity and attack surface. As a result, even organizations that integrate the best security procedures into their software development process can fall victim to a destructive security incident.

It is crucial to document all external services (like cloud hosting services and wallet providers), contracts (like DeFi protocols), and oracles (like pricing information) used by a blockchain system in order to identify risk exposure and mitigate incident impact. Doing so will help you answer the following essential questions:

How will we know when an external dependency suffers a security incident?
What are the specific conditions under which we declare a security incident?
What steps will we take when we detect one?
Answering these questions will help you be prepared when, inevitably, a security incident affects a dependency outside of your control. You should be able to notice any change, innocuous or not, in a dependency’s output, interface, or assumed program state; assess it for security impact; and take the necessary next steps. This will limit the security impact on your system and help ensure its uninterrupted operation.

3. Do you have a written and tested incident response plan?

While security in the blockchain space differs from traditional product security (where more centralized or closed systems may be easier to control), both require an effective incident response plan to help remain resilient in the face of a security incident. The plan should include steps to identify, contain, and remediate the incident through automated and manual procedures. An organization should provide training to ensure that all team members are familiar with the plan, and it should include steps for communicating incidents over internal and out-of-band channels. This plan should be regularly tested to ensure it is up-to-date and effective, especially given how quickly the blockchain security world can change. You should create your own incident response (IR) plan, and can use this Trail of Bits guide as a resource.

For blockchain systems, it is especially important that IR plans mitigate key person risk by ensuring the organization is not overly reliant on any single individual. The plan should anticipate scenarios where key personnel may be unavailable or coerced, and outline steps to ensure continuity of operations. Developers should consider decentralizing access controls, implementing quorum-based approvals, and documenting procedures so that multiple team members are prepared to respond.

For blockchain systems, it is especially important that incident response be proactive, not only reactive. The contracts should be designed alongside the creation of the IR plan using strategies like guarded launches to incrementally deploy new code. The developers should consider if they want—or not—pausable features in their contracts, and what part of the protocol should—or should not—be upgradeable or decentralized, as this will influence the team’s capabilities during an incident.

4. Do you document the best ways to attack your system?

By constructing a threat model that documents all potential avenues to attack the system, you can understand whether your existing security controls are sufficient to mitigate attacks. The threat model should visually lay out a product’s entire ecosystem, including information from beyond software development, such as applications, systems, networks, distributed systems, hardware, and business processes. It should identify all of the system’s weak points and clearly explain how an attacker can exploit them, incorporating information from relevant real-world attacks to help you avoid making the same mistakes.

This information will help you understand whether you are concentrating your efforts in the right spots—i.e., whether your current efforts to mitigate attacks are aligned with how and where they are most likely to occur. It will help you understand what a successful attack on your system will look like, and whether you are sufficiently prepared to detect, respond to, and contain it. A good threat model should eliminate surprise and enable your team to deliberately plan mitigations.

5. Do you perform identity verification and background checks on all employees?

Pseudonymous development is commonplace in the blockchain industry, but it impedes accountability, contractual enforcement, and engendering trust in and among stakeholders in a blockchain product. Malicious actors can exploit a lack of identity verification and background checks to interfere with a product’s development, steal funds, or cause other serious harm, and institutions will have no or limited means to punish them. In recent years, North Korean hackers have applied to real positions using fake Linkedin accounts and impersonated companies to offer fraudulent positions. These practices have directly led to severe hacks, including Axie Infinity’s $540 million loss.

As a result, companies must know the identities of and perform background checks on all of their employees, including those who use public pseudonyms. Companies must also reach additional maturity in their access controls and monitoring; for example, they should make prudent decisions surrounding operational security based on an employee’s role, background, and the territory they reside in (i.e., considering local laws and jurisdiction).

6. Do you have a team member with security defined in their role?

There needs to be a person on the team who is accountable for ensuring the safety and security of the blockchain system. Threats against blockchain technology evolve rapidly, and even a single security incident can be devastating. Only a dedicated security engineer has the time, knowledge, and skill set necessary to identify threats, triage incidents, and remediate vulnerabilities, which helps instill trust in your product as it develops.

Ideally, this person will create and oversee a dedicated team with security at the forefront of their job responsibilities, ultimately owning initiatives to get an organization to answer “yes” to other questions on this list. They will oversee cross-departmental efforts, working with developers, administrators, project leads, executives, and others to ensure security practices are included in all aspects of the organization.

7. Do you require hardware security keys for production systems?

Credential stuffing, SIM swap attacks, and spear phishing have nearly neutralized the protective capability of passwords and SMS/push two-factor authentication. For high-risk organizations with value at stake, phishing-resistant hardware keys are the only reasonable option. Special hardware keys should be used to access the company’s resources, including email, chat, servers, and software development platforms. Special care should be taken to protect any operation in production that is very difficult or impossible to reverse.

Using these keys inside your organization is a leading indicator of competent off-chain infrastructure management. Do not be deterred if this seems like a high-volume lift for your IT team. In 2016, Google released a study that showed that implementing these keys was simple, well-received among its 50,000 employees, and strong against malicious attacks. U2F hardware tokens, such as YubiKey and Google Titan, are good choices for hardware keys.

8. Does your key management system require multiple humans and physical steps?

If a single individual maintains the keys that control your system, they can unilaterally make changes that have an outsized impact, without a consensus of the relevant stakeholders. And if an attacker compromises their credentials, they can gain full control of core assets.

Instead, key management should be set up to require a consensus or quorum of multiple people and physical access for important decisions. Multi-person integrity is an effective security policy used in high-risk industries like defense and traditional finance; they protect against compromise via attackers, insider threats (e.g., rogue employees), and coercion, all in one fell swoop. When selecting the trusted set of individuals for a quorum-based setup, it’s crucial to choose those who are both trustworthy and properly incentivized, as including ill-suited or misaligned individuals can undermine the system’s resistance to coercion. By additionally requiring physical key management (e.g., using a physical safe or air-gapped device to store keys), you will significantly reduce the risk of fraud, theft, misuse, or errors by any individual or if any individual’s key or key fragment is compromised.

Blockchain organizations should employ the use of multi-signature or multi-party computation (MPC) controls and cold storage solutions for, at a minimum, the central wallets that hold most of their assets, or opt to use a qualified custodian, depending on specific regulations and needs. The keys to unlock a multi-signature wallet should be stored on trusted hardware, such as a hardware security module (HSM), secure enclave, or a tamper-resistant hardware wallet.

It’s imperative that the deployment and configuration of the trusted hardware is done carefully to limit its attack surface. For example, secrets should never be extractable and network connections should be avoided. Organizations should also establish a strict procedure for moving funds based on parameters like thresholds, affected wallets, destination, and key person(s) initiating the transaction.

9. Do you define key invariants for your system and test them on every commit?

An invariant is a condition that must remain true throughout the program’s execution. Invariants can target the system as a whole (e.g., no user should have more tokens than the total supply) or target a specific function (e.g., a compute_price function cannot lead to free assets). Understanding and defining invariants helps developers be explicit about the system’s expected behaviors and helps security engineers evaluate whether those behaviors measure up to expectations. This provides a roadmap for security testing and reduces the likelihood of unexpected outcomes and failures.

Defining invariants starts with documenting the assumptions made about the system in plain English. These invariants should cover a breadth of functional and cryptographic properties and their valid states, state transitions, and high-level behaviors. Well-specified systems may have hundreds of properties: you should focus on the most important ones first and continuously work to improve their depth of coverage. To ensure that the code follows the invariants, they must be tested with an automated tool (such as a fuzzer or a tool based on formal methods) throughout the development process.

10. Do you use the best automated tools for discovering security issues in your code?

Automated security tools are a baseline requirement in a successful security strategy. Fully automated tools, such as static analyzers, automatically find common mistakes and require low maintenance, while semi-automated tools, like fuzzers, allow developers to go one step further and check for logical issues. Many such tools are available, but we recommend using those that are actively used by top-tier security engineers, for which a proven track record of discovered bugs is available.

Trail of Bits’ smart contract security tools use state-of-the-art technology and can be integrated into your CI systems and the edit/test/debug cycle. They include Echidna, a smart contract fuzzer for Solidity smart contracts, and Slither, a static analyzer for Solidity smart contracts. Automating the use of these tools during development and testing helps developers catch critical security bugs before deployment.

11. Do you undergo external audits and maintain a vulnerability disclosure or bug bounty program?

To identify vulnerabilities in blockchain code, it isn’t enough to rely on internal security teams. Instead, organizations must work with external auditors who possess in-depth knowledge of modern blockchain technology, spanning low-level implementations, financial products and their underlying assumptions, and the libraries, services, bridges, and other infrastructure that power modern applications. (Websites that track blockchain security incidents are filled with companies that did not seek external guidance for sometimes complex changes.)

Security auditors help to identify vulnerabilities and provide advice for restructuring your development and testing workflow so these vulnerabilities do not come back. When looking for an audit, it’s important to clarify which components are under review, which are excluded, and the level of effort that should be applied, including through the use of tooling. By understanding the benefits and limitations of an audit, an organization can focus on additional areas needed for improvements once the audit has concluded.

Additionally, a vulnerability disclosure or bug bounty program can enhance your security posture by providing a publicly accessible option for users or researchers to contact you if they uncover a bug. By establishing these programs, organizations show a willingness to engage with independent bug hunters—and without them, they may instead publicly disclose the bugs on social media or even exploit them for their own gain. While these programs offer many benefits, it is important to consider their limitations and pitfalls. For example, bug bounty hunters will not provide recommendations for improving the security maturity of the system nor for reducing the likelihood of bugs in the long term. In addition, your team will still be responsible for triaging bug submissions, which can require constant dedicated resources.

12. Have you considered and mitigated avenues for abusing users of your system?

Many attacks against blockchain, such as phishing, Twitter/Discord scams, and “pig butchering,” attempt to fool users into taking irreparable actions while using your products. Even if an organization has the most expertly designed security system to protect itself, its own users may still be vulnerable. For example, blockchain applications often rely on cryptographic signatures that increase the likelihood of phishing attempts. Developers should consider making the signatures easily identifiable (for example, with EIP-712) and should create and promote guidance for their users to minimize the risk of abuse.

To avoid such attacks, an organization’s security strategy should include abusability testing, where your team considers how attackers can inflict social, psychological, and physical harm. Understanding the risks of significant financial or societal harms will help your team to evaluate necessary processes and mitigations. For example, if your protocol’s users include high-impact stakeholders, such as retirement funds, creating an assurance fund based on the protocol’s fees may help to make the users whole in case of compromise.

Don’t get rekt
These 12 controls are not the only actions that can determine your security posture, but we’re confident that they will enhance every developer’s software and operational security, even as blockchain technology rapidly innovates. This test should not serve as a one-time exercise; these questions have lasting value and should give organizations a roadmap as they continue to grow and develop new products. Answering “yes” to these questions doesn’t mean you will completely avoid a security incident, but it can empower you and your team to steer clear of the worst label in the industry: getting rekt.

---
