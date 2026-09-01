# Selected Works — Raw Research

Compiled list of Bernhard Mueller's published work. Grouped by project/theme, with reference links.

**Status:** DRAFT — needs review for accuracy and completeness.

---

## Mobile Security

### OWASP MASTG (Mobile Application Security Testing Guide)
- **Role:** Creator and lead author
- **What:** The definitive industry-standard guide for mobile app security testing and reverse engineering. 703 pages, 24,600+ readers. OWASP Flagship project.
- **GitHub:** https://github.com/OWASP/mastg (12,700+ stars)
- **Official site:** https://mas.owasp.org/MASTG/
- **Leanpub:** https://leanpub.com/owasp-mastg
- **Co-authors:** Sven Schleier, Jeroen Willemsen, Carlos Holguera
- **Notable:** The [Reverse Engineering and Tampering chapter](https://github.com/boblone19/OWASP-MSTG/blob/master/Document/0x05c-Reverse-Engineering-and-Tampering.md) was primarily written by Bernhard. Ties into the obfuscation measurement research below.

### OWASP MASVS (Mobile Application Security Verification Standard)
- **Role:** Creator and lead author
- **What:** Industry standard defining security requirements for mobile applications. Adopted by enterprises and regulators worldwide.
- **GitHub:** https://github.com/OWASP/masvs (2,300+ stars)
- **Official site:** https://mas.owasp.org/MASVS/

### Hacking Soft Tokens (Paper + Talk)
- **What:** Research demonstrating attacks against mobile 2FA/OTP tokens on iOS and Android — from classical reverse engineering to custom kernel sandboxes and full-system emulation. Included PoC exploits for tokens from major banking vendors.
- **Talk:** HITB GSEC 2016 Singapore — "Attacking Software Tokens"
- **Paper:** https://regmedia.co.uk/2016/09/02/hacking_soft_tokens_-_bernhard_mueller.pdf
- **Speaker page:** https://gsec.hitb.org/sg2016/speakers/bernhard-mueller/
- **Talk video (Internet Archive):** https://archive.org/details/youtube-wvxjpRvwa0U

### Frida Detection
- **What:** Reference implementations for detecting the Frida dynamic instrumentation framework on Android. Foundational for OWASP MASTG anti-tampering content.
- **GitHub:** https://github.com/muellerberndt/frida-detection (493 stars)

### Android App Security Checklist
- **What:** Widely-referenced security checklist for Android app developers and testers.
- **GitHub:** https://github.com/muellerberndt/android_app_security_checklist (891 stars)

### apkx
- **What:** One-step APK decompilation with multiple backends. Streamlines mobile reverse engineering.
- **GitHub:** https://github.com/muellerberndt/apkx (290 stars)

### Obfuscation Metrics
- **What:** Framework for measuring and evaluating code obfuscation effectiveness. Related to the MASTG Reverse Engineering chapter.
- **GitHub:** https://github.com/muellerberndt/obfuscation-metrics (55 stars)

### Uncrackable Apps (Mobile Crackmes)
- **What:** Challenge applications for practicing mobile reverse engineering, used in OWASP MASTG training.
- **GitHub:** https://github.com/muellerberndt/uncrackable_app (13 stars)

---

## Smart Contract Security

### Mythril
- **Role:** Creator (transferred to ConsenSys)
- **What:** Pioneering open-source security analysis tool for EVM bytecode. Uses symbolic execution, SMT solving, and taint analysis. "The nmap of Ethereum."
- **GitHub:** https://github.com/ConsenSysDiligence/mythril (4,200+ stars)
- **Announcement:** https://medium.com/hackernoon/introducing-mythril-a-framework-for-bug-hunting-on-the-ethereum-blockchain-9dc5588f82f6

### Smashing Smart Contracts (Paper + Talk)
- **What:** Research paper and talk on symbolic-execution-based analysis of EVM smart contracts. Introduced Mythril's symbolic analysis approach.
- **Talk:** HITB SecConf 2018 Amsterdam — "Smashing Ethereum Smart Contracts for Fun and ACTUAL Profit"
- **Whitepaper:** https://conference.hitb.org/hitbsecconf2018ams/materials/WHITEPAPERS/WHITEPAPER%20-%20Bernhard%20Mueller%20-%20Smashing%20Ethereum%20Smart%20Contracts%20for%20Fun%20and%20ACTUAL%20Profit.pdf
- **Slides:** https://conference.hitb.org/hitbsecconf2018ams/materials/D1T2%20-%20Bernhard%20Mueller%20-%20Smashing%20Ethereum%20Smart%20Contracts%20for%20Fun%20and%20ACTUAL%20Profit.pdf
- **GitHub:** https://github.com/muellerberndt/smashing-smart-contracts (177 stars)
- **Pwnie nomination:** Nominated for Pwnie Award 2018

### The Ether Wars (DEF CON 27 Talk)
- **What:** Talk on the adversarial landscape on Ethereum — exploits, counter-exploits, and honeypots. Demonstrated Scrooge McEtherface auto-exploitation bot.
- **Talk:** DEF CON 27 (August 2019), co-presented with Daniel Luca
- **Slides:** https://media.defcon.org/DEF%20CON%2027/DEF%20CON%2027%20presentations/DEFCON-27-Bernhard-Mueller-The-Ether-Wars.pdf
- **Demo videos:** https://media.defcon.org/DEF%20CON%2027/DEF%20CON%2027%20presentations/DEFCON-27-Bernhard-Mueller-Demo-Videos/

### Scrooge McEtherface
- **What:** Ethereum auto-looter using symbolic execution and Z3 solver to automatically extract ETH from vulnerable contracts.
- **GitHub:** https://github.com/muellerberndt/scrooge-mcetherface (153 stars)
- **Article:** https://blog.goodaudience.com/automating-smart-contract-exploitation-and-looting-d43e9740b41c

### SolFuzz
- **What:** Hybrid fuzzer combining grey-box fuzzing with symbolic analysis for Solidity assertion violations.
- **GitHub:** https://github.com/muellerberndt/solfuzz (32 stars)

### DeFi Hacking Playground
- **What:** Local testing environment for experimenting with flash loan attacks and DeFi exploits.
- **GitHub:** https://github.com/muellerberndt/defi-hacking-playground (32 stars)

### Rektosaurus
- **What:** Test suite for detecting XSS via malicious NFT metadata injection on marketplace platforms.
- **GitHub:** https://github.com/muellerberndt/rektosaurus (51 stars)

### Storm
- **What:** Blockchain node stress-testing/fuzzing tool that finds DoS vulnerabilities in EVM node implementations.
- **GitHub:** https://github.com/muellerberndt/storm (39 stars)

---

## AI & Autonomous Agents

### Hound (Paper + Tool)
- **Role:** Creator (transferred to scabench-org)
- **What:** Language-agnostic AI code security auditor that builds adaptive knowledge graphs for deep iterative reasoning. Uses two-model architecture (junior agent + senior guidance).
- **GitHub:** https://github.com/scabench-org/hound (716 stars)
- **arXiv paper:** https://arxiv.org/abs/2510.09633 — "Hound: Relation-First Knowledge Graphs for Complex-System Reasoning in Security Audits" (Oct 2025)
- **Results:** On ScaBench: 31.2% micro recall vs 8.3% baseline; F1 14.2% vs 9.8%

### ScaBench
- **Role:** Creator (transferred to scabench-org)
- **What:** Benchmarking framework for evaluating AI smart contract audit agents against real-world vulnerability datasets.
- **GitHub:** https://github.com/scabench-org/scabench (100 stars)

### MiniAGI
- **What:** Minimal autonomous AI agent based on OpenAI API. Went viral during the 2023 AI agent wave — one of the simplest yet most capable early agent frameworks.
- **GitHub:** https://github.com/muellerberndt/mini-agi (2,906 stars)

### Darwin GPT
- **What:** Experiment in AI self-replication — a GPT-based agent that can spawn copies of itself.
- **GitHub:** https://github.com/muellerberndt/darwin-gpt (62 stars)

### Legion
- **What:** AI-assisted web3 bug bounty hunting assistant. Tracks live bounties and deploys autonomous agents to find vulnerabilities.
- **GitHub:** https://github.com/muellerberndt/legion (129 stars)

### Mancala Deep-Q
- **What:** Solving the ancient board game Mancala using deep Q-learning (reinforcement learning). Includes OpenAI Gym environment, agent vs. agent self-play, and PyGame UI.
- **GitHub:** https://github.com/muellerberndt/mancala-deepq
- **Stack:** Python, DQN, PyGame

### Rage of the Machine (Metal MIDI Transformer)
- **What:** Polyphonic, multi-instrument music transformer trained on 3,604 metal/grunge/punk MIDI songs (augmented to ~18,000 via pitch transposition). Custom MIDI tokenizer supporting multiple instruments and percussion. Trained 200 hours on 4× Nvidia T4 GPUs using TransformerXL.
- **Article:** https://muellerberndt.medium.com/rage-of-the-machine-an-ai-makes-metal-music-f299dc1f706a
- **Note:** Repository may be private or unpublished.

---

## Medium Articles (Technical)

### Smart Contract Security
- [Introducing Mythril](https://medium.com/hackernoon/introducing-mythril-a-framework-for-bug-hunting-on-the-ethereum-blockchain-9dc5588f82f6) — Oct 2017
- [Analyzing Ethereum Smart Contracts for Vulnerabilities](https://medium.com/hackernoon/scanning-ethereum-smart-contracts-for-vulnerabilities-b5caefd995df) — ~2018
- [What Killed the Parity Multisig Wallet](https://medium.com/hackernoon/what-caused-the-latest-100-million-ethereum-bug-and-a-detection-tool-for-similar-bugs-7b80f8ab7279) — ~2017
- [Practical Smart Contract Security Analysis and Exploitation (Part 1)](https://medium.com/hackernoon/practical-smart-contract-security-analysis-and-exploitation-part-1-6c2f2320b0c) — Nov 2018
- [Detecting Integer Arithmetic Bugs (batchOverflow)](https://media.consensys.net/detecting-batchoverflow-and-similar-flaws-in-ethereum-smart-contracts-93cf5a5aaac8) — ~2018
- [Catching Weird Security Bugs with Global Invariant Checks](https://muellerberndt.medium.com/catching-weird-security-bugs-in-solidity-smart-contracts-with-invariant-checks-435582dfb5bd)
- [Automated Smart Contract Looting with SMT Solvers](https://blog.goodaudience.com/automating-smart-contract-exploitation-and-looting-d43e9740b41c) — ~2019
- [Advanced Smart Contract Security Verification in Remix](https://medium.com/coinmonks/advanced-smart-contract-security-verification-in-remix-9630b43695e5)
- [Ethereum Security Tools Built by ConsenSys Diligence](https://medium.com/consensys-diligence/all-ethereum-security-tools-built-by-consensys-diligence-dd918248f978) — ~2019

### Web3 Malware Analysis
- [A Brief Analysis of Angel Drainer](https://muellerberndt.medium.com/a-brief-analysis-of-angel-drainer-1660d15c9248) — 2024
- [Reverse Engineering Inferno Drainer](https://muellerberndt.medium.com/a-peek-inside-inferno-drainer-0a69647b85ca) — 2024

### NFT / DeFi Security
- [Building a Secure NFT Gaming Experience (Herdsman's Diary)](https://muellerberndt.medium.com/building-a-secure-nft-gaming-experience-a-herdsmans-diary-1-91aab11139dc) — 2022
- [Wolf Game Herdsman's Report](https://muellerberndt.medium.com/wolf-game-herdsmans-report-5802c9d477bd) — 2022
- [Is Tether a Black Swan?](https://muellerberndt.medium.com/is-tether-a-black-swan-51095720b01c) — Jun 2021

### AI & Music
- [Rage of the Machine: An AI Makes Metal](https://muellerberndt.medium.com/rage-of-the-machine-an-ai-makes-metal-music-f299dc1f706a)

### AI Security Auditing
- [Unleashing the Hound: AI Agents Find Deep Logic Bugs](https://muellerberndt.medium.com/unleashing-the-hound-how-ai-agents-find-deep-logic-bugs-in-any-codebase-64c2110e3a6f) — 2025
- [Hunting for Security Bugs with AI Agents: Full Walkthrough](https://muellerberndt.medium.com/hunting-for-security-bugs-in-code-with-ai-agents-a-full-walkthrough-a0dc24e1adf0) — 2025

### Zero-Knowledge Proofs
- [The Security Researcher's Guide to Mathematics](https://muellerberndt.medium.com/the-security-researchers-guide-to-mathematics-000dc0c98a0f) — Nov 2025
- [STARK Lab: An Interactive Deep Dive into ZK Proofs](https://muellerberndt.medium.com/stark-lab-an-interactive-deep-dive-into-zero-knowledge-proofs-d5894121b22e) — Dec 2025
- [A Practical Guide to Finding Soundness Bugs in ZK Circuits](https://muellerberndt.medium.com/finding-soundness-bugs-in-zk-circuits-ea23387a0e1e) — Jan 2026

### Misc / Satire
- [I Asked GPT-3 for the Question to "42"](https://muellerberndt.medium.com/i-asked-gpt-3-for-the-question-to-42-i-didnt-like-its-answer-and-neither-will-you-33f425a4d60f)
- [The Definitive Guide to Becoming a Crypto Maximalist](https://medium.com/hackernoon/the-definitive-guide-to-becoming-a-crypto-maximalist-82b64d02c707) (satire)
- [How to Become a Cryptocurrency Thought Leader on Twitter](https://medium.com/coinmonks/how-to-become-a-cryptocurrency-thought-leader-on-twitter-f10ac1c26488) (satire)
- [To Fork or Not to Fork? Bitcoin/Ethereum Community Survey](https://medium.com/hackernoon/to-fork-or-not-to-fork-results-of-a-bitcoin-and-ethereum-community-survey-d46abe1d15dc) — ~2017

---

## Whitepapers & Research (Pre-Blockchain Era)

### From 0 to 0Day on Symbian (2009)
- **What:** Demonstrated that classic vulnerability analysis and exploitation techniques are feasible on Symbian OS smartphones, despite OS obscurity and lack of tooling. Showed how to find low-level vulns in Nokia phones exploitable via MMS.
- **SEC Consult PDF:** https://sec-consult.com/fileadmin/user_upload/sec-consult/Statisch/Vulnerability_Lab/Studies_and_Whitepapers/SEC-Consult_Whitepaper_pwning_symbian_v105_public.pdf
- **Scribd mirror:** https://www.scribd.com/document/17217176/From-0-to-0day-on-Sybian
- **Won Pwnie Award 2009 "Best Research"**

### Improved DNS Spoofing Using Node Re-Delegation (2008)
- **What:** Technique to make DNS cache poisoning more reliable. SEC Consult was among the first to write a working "fast cache poisoning" exploit after Dan Kaminsky's coordinated multi-vendor disclosure.
- **Full Disclosure:** https://seclists.org/fulldisclosure/2008/Aug/103
- **PDF:** https://sec-consult.com/fileadmin/user_upload/sec-consult/Statisch/Vulnerability_Lab/Studies_and_Whitepapers/SEC-Consult_Whitepaper_whitepaper-dns-node-redelegation.pdf

### FireWire-Hack in Windows Vista (2008)
- **What:** Demonstrated that the FireWire DMA unlock attack works against Windows Vista. PoC disables password authentication in the default Vista login routine.
- **Co-author:** Peter Panholzer
- **Bugtraq:** https://seclists.org/bugtraq/2008/Mar/42

---

## Vulnerability Advisories

### SEC Consult Era (2005–2013)

- **Macromedia Flash Player ActionDefineFunction Memory Corruption** (Nov 2005) — SA-20051107-1. Parameters to ActionDefineFunction not properly sanitized, crash/code execution. flash.ocx ≤7.0.19.0. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/macromedia-flash-player-actiondefinefunction-memory-corruption/)
- **toendaCMS Multiple Vulnerabilities** (Nov 2005) — SA-20051107-0. Username/password theft, session theft, directory traversal, arbitrary file upload. Versions <0.6.2.
- **Symantec Enterprise Firewall Internal IP Leak** (May 2006) — SA-20060512-0. Leaks internal IPs of NATted machines. Version 8.0.
- **Opera Browser CSS Attribute Integer Wrap** (Apr 2006) — SA-20060413-0. Integer wrap and buffer overflow in Opera ≤8.52.
- **PHP exec/system/popen File Descriptor Bug** (Oct 2006) — PoC exploit that overwrites Apache's log file.
- **MySQL Information Schema DoS** (Mar 2007) — SA-20070309-0. Null-pointer dereferenciation when using functions with subselects on information_schema + ORDER BY. MySQL <5.0.37. Co-discovered with S. Streichbier.
- **Perdition IMAP Proxy Format String** (Oct 2007) — SA-20071031-0. CVE-2007-5740. Arbitrary code execution without auth via null-byte bypass. Fixed in v1.17.1. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/perdition-imap-proxy-str-vwrite-format-string-vulnerability/)
- **SonicWALL SSL-VPN ActiveX Vulnerabilities** (Nov 2007) — SA-20071101-0. Multiple vuln in ActiveX controls for SonicWALL SSL-VPN.
- **SonicWALL Global VPN Client Format String** (Dec 2007) — SA-20071204-0. Format string via crafted config file. Versions <4.0.0.830.
- **Fujitsu-Siemens WebTransactions Command Injection** (Dec 2008) — SA-20081219-0. Remote command injection via unvalidated input passed to system(). No auth required.
- **Microsoft SQL Server sp_replwritetovarbin Memory Overwrite** (Dec 2008) — SA-20081209-0. CVE-2008-5416. Write to controlled memory locations. Exploitable via authenticated connection or SQL injection. MS09-004. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/microsoft-sql-server-sp-replwritetovarbin/) / [CERT/CC](https://www.kb.cert.org/vuls/id/696644)
- **Nortel Contact Center Manager Auth Bypass** (May 2009) — SA-20090525-0. Client-side cookie-based auth bypass. Version 6.0. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/nortel-contact-center-manager-server-authentication/)
- **SonicWALL Global VPN Client Local Privilege Escalation** (May 2009) — SA-20090525-3. Installation folder permissions Everyone:Full Control. Versions ≤4.0.0.835.
- **IBM Director CIM Server DoS** (Mar 2009) — SA-20090305-1. Remote DoS. IBM Director ≤5.20.3 SU2. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/ibm-director-cim-server-remote-denial-of-service-vulnerability/)
- **IBM Director CIM Server Local Priv Esc** (Mar 2009) — SA-20090305-2. IBM Director ≤5.20.3 SU2. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/ibm-director-cim-server-local-privilege-escalation-vulnerability/)
- **Symbian S60 / Nokia Media Codecs Memory Corruption** (Jul 2009) — SA-20090707-0. Multiple memory corruption flaws in Nokia multimedia codecs, exploitable via MMS. 7 vulnerable DLLs. Tested on E61, E71, N96. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/symbian-s60-nokia-firmware-media-codecs/)
- **IBM System Director Agent DLL Injection** (Dec 2012) — Arbitrary DLL injection via wmicimsv service. Metasploit module. Co-credited with juan vazquez, Kingcope.
- **ModSecurity Multipart Bypass** (Oct 2012) — SA-20121017-0. POST parameter validation bypass via parsing discrepancy between ModSecurity and PHP. ModSecurity ≤2.6.8. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/modsecurity-multipart-invalid-part-ruleset-bypass/) / [Full Disclosure](https://seclists.org/fulldisclosure/2012/Oct/113)
- **Sybase EAServer Multiple Vulnerabilities** (Jul 2013) — SA-20130719-0. Directory traversal, XML entity injection, OS command execution. EAServer ≤6.3.1. Co-discovered with Gerhard Wagner. [SEC Consult advisory](https://sec-consult.com/vulnerability-lab/advisory/multiple-vulnerabilities-in-sybase-easerver/)

### Vantage Point Security Era (2014–2016)

- **SysAid Server Arbitrary File Disclosure** (Dec 2014) — VP-2014-004. Unauthenticated file disclosure, LDAP credential theft. Versions <14.4.2. [Exploit-DB #35593](https://www.exploit-db.com/exploits/35593) / [Full Disclosure](https://seclists.org/fulldisclosure/2014/Dec/99)
- **Cisco Unified Communications Manager Multiple Vulns** (Aug 2015) — VP-2015-001. Shellshock command injection, LFI, unauthenticated ping execution, hardcoded session ID bypass. CUCM <9.2/10.5.2/11.0.1. [Exploit-DB #37816](https://www.exploit-db.com/exploits/37816) / [Full Disclosure](https://seclists.org/fulldisclosure/2015/Aug/47)

### dotDefender WAF Format String (Nov 2012)
- Applicure dotDefender WAF ≤4.26. Format string vulnerability.

---

## Theoretical Physics

### Observer Patch Holography
- **What:** Theory-of-everything reconstruction program based on observer-like self-reading systems: finite patches compare overlap-visible records, repair mismatch, and stabilize public records. The corpus proves exact finite precursors for informational order, quantum records, rank-three carrier geometry, Lorentz algebra, and gauge structure, then gives explicitly conditional branches toward effective 3+1 spacetime, smooth Einstein gravity, particles, and physical observers. Faithful causal attachment, manifold and volume recovery, continuum limits, and laboratory realization remain named requirements rather than recovered outputs.
- **GitHub:** https://github.com/FloatingPragma/observer-patch-holography (19 stars)
- **Overview:** https://floatingpragma.io/oph/
- **Textbooks:** https://learn.floatingpragma.io/
- **Technical paper:** https://floatingpragma.io/oph/papers/from-observer-consensus-to-standard-physics/
- **Lab:** https://oph-lab.floatingpragma.io/
- **Applications:** https://omega.floatingpragma.io/
- **Challenge:** https://challenge.floatingpragma.io/
- **Paper index:** https://floatingpragma.io/oph/papers/
- **License:** https://github.com/FloatingPragma/observer-patch-holography/blob/main/LICENSE
- **Anti-patent covenant:** https://github.com/FloatingPragma/observer-patch-holography/blob/main/PATENTS.md
- **Article:** https://muellerberndt.medium.com/answering-10-of-the-hardest-questions-in-physics-and-some-bonus-questions-51222bf2419f — Jan 2026

---

## Awards & Recognition

- **Pwnie Award 2009 "Best Research"** — Won for "From 0 to 0Day on Symbian" (BlackHat)
- **Pwnie Award 2018 Nomination** — Nominated for "Smashing Ethereum Smart Contracts for Fun and ACTUAL Profit"
- **OWASP Flagship Project Leader** — MASTG and MASVS

---

## Career Roles

- **AI Research Lead** — Sherlock (Web3 audit contest platform)
- **Security Engineer** — ConsenSys Diligence (smart contract auditing)
- **Vantage Point Security** — Published advisories under VP-20xx-xxx series
- **SEC Consult** — Published advisories under SA-20xxxxxx-x series (2005–2013)

---

## Interactive Learning Platforms (floatingpragma.io)

- **STARK Lab** — Interactive STARK proof tutorial: https://floatingpragma.io/starklab/
- **Awesome ZK Proofs** — Curated ZK learning path: https://floatingpragma.io/awesome-zk-proofs/
- **Awesome AI Security** — AI security learning path: https://floatingpragma.io/awesome-ai-security/

---

## TODO / Needs Review

- [ ] Confirm Sherlock blog post URL: https://sherlock.xyz/post/inside-the-lab-berndt-on-the-sherlock-ai-v2-upgrade
- [ ] Confirm "Rage of the Machine" repo status (private/deleted/unpublished?)
- [ ] Check if any more Medium articles are missing (only public search was used)
