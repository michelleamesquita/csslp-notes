# Exam Outline Review

## 1. Secure Software Concepts

### 1.1 Core Concepts

- **Confidentiality**
  - Covert channel: communication path that is intentionally hidden. Leaves almost no trace. Receiver has to be actively listening for message
  - Overt channel: communication path that is not hidden. Leaves evidence behind but receiver doesn't have to be listening for message
  - Side channel: unintentional communication. Think power consumption changes to get information about encryption used
- **Integrity**
  - Also includes stability and reliability for authorized subjects
- **Availability**
- **Authentication**
- **Authorization**
- **Accountability**
- **Nonrepudiation** 
 - denying a previous action with an object   

### 1.2 Security Design Principles

- **Least Privilege**
- **Separation of duties**
- **Defense in depth**
- **Resiliency**
  - fail safe, fail secure, no single point of failure
- **Economy of mechanism**
  - less complexity is better
  - eliminate nonessential services and protocols
- **Complete mediation**
  - authorization cannot by bypassed
  - authorization checked every time subject requests access to an object
- **Open design**
  - security of a system is independent of the design (don't rely on security by obscurity)
  - Kerckhoffs's principle: security of a cryptosystem is reliant on choice of keys, not algorithm
- **Least common mechanism**
  - isolation to protect against sharing of information
- **Psychological acceptability**
- **Component reuse**
- **Diversity of defense**
  - layers of defense should be diverse
- **Safeguard**
  - _Proactive_ controls to protect assets
  - controls can be physical, administrative, or technical
- **Countermeasure**
  - _Reactive_ controls to protect assets
  - controls can be physical, administrative, or technical

## 2. Secure Software Requirements

### 2.1 Define Software Security Requirements

- **Functional**
  - business requirements
  - use cases
  - user stories
- **Non-functional**
  - operational
  - deployment
  - systemic qualities
  - performance, security , scalability ,usability and maintainance 

### 2.2 Identify and Analyze Compliance Requirements

- **FISMA**
  - an agency-wide information security program is required for federal agencies
- **Sarbanes-Oxley**
  - internal control measures for financial accounting
- **Gramm-Leach-Bliley**
  - protection of PFI (Personal Financial Information)
  - protects against falsely pretending to obtain PFI
- **HIPAA and HITECH**
- **Payment Card Industry Data Security Standard (PCI DSS)**

### 2.3 Identify and Analyze Data Classification Requirements

- **Data ownership**
- **Labeling**
  - sensitivity and impact
  - primarily driven by cost
- **Types of data**
  - structured, unstructured
  - categories: security sensitive, PII, hidden
- **Data life-cycle**
  - if persistent, data needs to be classified, labeled, assigned retention policy
  - retention policies include backups, DR sites, legal holds
  - legal hold data is excluded from normal disposal procedures

### 2.4 Identify and Analyze Privacy Requirements

- **Data anonymization**:remove personal identity info and replace with unique identifier
- **User consent**
- **Disposition**
  - right to be forgotten
- **Data retention**
- **Cross borders**

### 2.5 Develop Misuse and Abuse Cases

- it helps to find vulnerability and identify points of failure

- **Use cases**
  - helpful for clarifying complex/confusing/ambiguous situations
  - not intended for all subject-object relationships

### 2.6 Develop Security Requirement Traceability Matrix (STRM)

- it is used to identify the relationship between: security requirements, design and implementation components

- document relationships between security requirements, controls, and test/verification efforts

### 2.7 Ensure Security Requirements Flow Down to Suppliers/Providers

## 3. Secure Software Architecture and Design

### 3.1 Perform Threat Modeling

- **Understand common threats**
- **Attack surface evaluation**
- **Threat intelligence**

### 3.2 Define the Security Architecture

- **Security control identification and prioritization**
- **Distributed computing**
- **Service-oriented architecture**
- **Rich internet applications**
- **Pervasive/ubiquitous computing**
  - IOT
  - RFID
  - NFC
- **Embedded**
  - Field-programmable gate array (FPGA) security features
- **Cloud architecture**
- **Mobile applications**
- **Hardware platform concerns**
- **Cognitive computing**
  - machine learning, AI
- **Control systems**

### 3.3 Performing Secure Interface Design

- **Security management interfaces, out-of-band management, log interfaces**
- **Upstream/downstream dependencies**
- **Protocol design choices**

### 3.4 Performing Architectural Risk Assessment

### 3.5 Model (Non-Functional) Security Properties and Constraints

### 3.6 Model and Classify Data

### 3.7 Evaluate and Select Reusable Secure Design

- **Credential management**
- **Flow control**
  - proxies, firewalls, protocols, queueing
- **Data loss prevention**
- **Virtualization**
- **Trusted computing**
- **Database security**
- **Programming language environment**
- **Operating system controls and services**
- **Secure backup and restoration planning**
- **Secure dat retention, retrieval, and destruction**

### 3.8 Perform Security Architecture and Design Review

### 3.9 Define Secure Operational Architecture

### 3.10 Use Secure Architecture and Design Principles, Patterns, and Tools

## 4. Secure Software Implementation

### 4.1 Adhere to Relevant Secure Coding Practices

- **Declarative vs imperative (programmatic) security**
- **Concurrency**
- **Output sanitization**
- **Error and exception handling**
- **Input validation**
- **Secure logging & auditing**
- **Session management**
- **Trusted/Untrusted APIs and libraries** : Attacks to API can be mitigated with Analisys of attack surface and threat model. It is a problem to architectural and design, because can expends attack surface
- **Type safety**
- **Resource management**
- **Secure configuration management**
- **Tokenizing** : method to obfuscate data to prevent unauthorized access
- **Isolation**
- **Cryptography**
- **Access control** : it's a simple security state: you have to be authorized to view an object.action is performed in object
- **Processor micro-architecture security extensions**

### 4.2 Analyze Code for Security Risks

- **Secure code reuse** - it can increase attack surface of software
- **Vulnerability databases/lists**
- **Static application security testing**
- **Dynamic application security testing**
- **Manual code review**
- **Look for malicious code**
- **Interactive application security testing**

### 4.3 Implement Security Controls

### 4.4 Address Security Risks

- **Risk response**

### 4.5 Securely Reuse Third-Party Code or Libraries

### 4.6 Securely Integrate Components

- **Systems-of-systems integration**

### 4.7 Apply Security During the Build Process

- **Anti-tampering techniques**
- **Compiler switches**
- **Address compiler warnings**

## 5. Secure Software Testing

### 5.1 Develop Security Test Cases

- **Attack surface validation**
- **Penetration tests**
- **Fuzzing**
- **Scanning** --> automated enumeration test
- **Simulation**
- **Failure**
  - break testing
  - fault injection: introducing faults to see how software behaves. Test error handling code paths
- **Cryptographic validation**
- **Regression tests**
- **Integration tests** --> test interface between modules
- **Continuous**
  - synthetic transactions: write code to mimic user behavior using a browser
  - real-user monitoring: collect data based on actual user data (e.g. Google Analytics)

### 5.2 Develop Security Testing Strategy and Plan

- **functional security testing**
- **nonfunctional security testing**
  - reliability
  - performance
  - scalability
- **testing techniques**
  - white box
  - black box
- **environment**
- **standards**
  - ISO
  - Open Source Security Testing Methodology Manual (OSSTMM)
  - Software Engineering Institute (SEI)
- **crowd sourcing**
  - bug bounty

### 5.3 Verify and Validate Documentation

### 5.4 Identify Undocumented Functionality

### 5.5 Analyze Security Implications of Test Results

### 5.6 Classify and Track Security Errors

- **Bug tracking**
- **Risk scoring**
  - CVSS
  - understand the severity error
  - assign priorities for defect remediation

### 5.7 Secure Test Data

- **Generate test data**
- **Reuse of production data**

### 5.8 Perform verification and validation testing

## 6. Secure Software Lifecycle Management

- operation phase begins when software is release from development

### 6.1 Secure configuration and version control

- its important to automated transparent test

### 6.2 Define strategy and roadmap

### 6.3 Manage security within a software development methodology

### 6.4 Identify security standards and frameworks

### 6.5 Define and develop security documentation

### 6.6 Develop security metrics

### 6.7 Decommision software

- **End of life policies**
- **Data disposition**

### 6.8 Report security status

### 6.9 Incorporate integrated risk management (IRM)

### 6.10 Promote security culture in software development

### 6.11 Implement continuous improvement

## 7. Secure Software Deployment, Operations, and Maintenance

### 7.1 Perform operational risk analysis

- **Deployment environment**
- **Personnel training**
- **Safety criticality**
- **System integration**

### 7.2 Release software securely

- **Secure continuous integration and continuous delivery pipeline**
- **Secure software tool chain**
- **Build artifact verification**

### 7.3

- **Credentials**
- **Secrets**
- **Keys/certificates**
- **Configurations**

### 7.4 Ensure secure installation

- **Bootstrapping**
- **Least privilege**
- **Environment hardening**
- **Secure activation**
- **Security policy implementation**
- **Secrets injection**

### 7.5 Perform post-deployment security testing

- Configuration managment is after deployment and post-release assurance

### 7.6 Obtain security approval to operate

### 7.7 Perform information security continuous monitoring (ISCM)

- **Collect and analyze observable data**
- **Threat intel**
- **Intrusion detection/response**
- **Secure configuration**
- **Regulation changes**

### 7.8 Support incident response

- firts thing: determine the nature of the incident

- **strategically planned***. team with variety of skill is better

- **Root cause analysis**
- **Incident triage**
- **Forensics**

### 7.9 Perform patch management

### 7.10 Perform vulnerability management

### 7.11 Runtime protection

### 7.12 Support continuity of operations

- **Backup, archiving, retention**
- **Disaster recovery**
- **Resiliency**

### 7.13 Integrate service level objectives and service level agreements

## 8. Secure Software Supply Chain

### 8.1 Implement software supply chain risk management

- **Identify**
- **Assess**
- **Respond**
- **Monitor**

### 8.2 Analyze security of third-party software

### 8.3 Verify pedigree and provenance

- **Secure transfer**
- **System sharing/interconnections**
- **Code repository security** --> its important to intelectual property
- **Build environment security**
- **Cryptographically-hashed, digitally-signed components**
- **Right to audit**

### 8.4 Ensure supplier security requirements in teh acquisition process

### 8.5 Support contractual requirements

### 8.6 Security Evaluation

- It evaluates integrations process and individual components 

### 8.7 Risk Governance

- it's the sum of executive actions to managing risk

### 8.8 Risk

- contract is a specific area of the risk that can have potential punitive consequences 

### 8.9 EULA

- the first propose of end-user licence agreement is clearfy the permited users and restriction to software 

### 9.0 Errors

- flaw is error in design, behavour anomaly is operational issue and vulnerability is bug that can me manipulated in Operational System

### 9.1 Obfuscation

- its a security measure to eliminates vulnerability that can be present in code

### 9.2 WAF

- it protects against known vulnerabilities and common attacks

### 9.3 Flow

- moviment of information across system 

### 9.4 Memory Management Routine

- garbage collection and memory allocation (allocation, deallocation, cleaning up)

### 9.5 ASSET (automated security self-evaluation)

- its a framework, quantitative. it automates the process of completing security system self assessment to NIST. it focuses risk in various aspects (threat, vulns,secure posture)

### 9.6 OWASP and CWE, SANS top 25

- focus on identifing common software vulnerabilities

### 9.7 Prioritizing the mitigation of security vulnerabilities based on test

- considerer context, potentital impact, exploitability and risk to prioritize

### 9.8 Estabilish environment for test allows

- interoperability of artifacts

### 9.9 Capable development process

- training and awareness

### 10.0 Software contract

- it is legal basis to communicate functions required and all necessary terms and conditions for acceptance 

### 10.1 Contract-based plan 

- code-level tests have been performed and documented

### 10.2 SAST

- focus on identifying vulnerabilities and secure weakness in the code

### 10.3 RFP (request for proposal)

- comunicates about statement of function required. its sent to all bidders for a formal response

### 10.4 Code-walk though/code review

- it serves to check code and find cryptographic functions, libs call depreceated and logic bombs

### 10.5 Cyclometic complexity

- it mesuares of the number of independent code path in program, in code review

### 10.6 SCADA (supervisory control and data acquisition)

- it important to have security protection to internet

### 10.7 External obligation

- statutory, regulatory and contractual obligation

### 10.8 Risk management

- likehood(probability) and impact

### 10.9 SIEM

- purpose: improving acuracy and efficiency of log analysis 

### 10.10 Management risk

- do nothing, mitigate, transfer, remidiate
- its quantitative with test, and qualitative with reviews

### 10.11 qualitative assessment

- its broder scope,priorizing the scope

### 11.0 Destructive test

- envolves analysing software vulnerabilities by gradually building them until breaks , then identyfing weak points

### 11.1 Activies in incident responde plan

- triage, forensics,remeadiation and root cause analysis

### 11.2 Secure development

- all elements of the software are constructed and operate securely

### 11.3 TCB e TCM

- TCB (Computing base): hardware,software and firmeware that ensure security in trusted computing
- TCM (platform module): chip-based provides hardware-level encryption for secure data , like encryption keys

### 11.4 Impact of the risk

- systematic of unsystematic

### 11.5 Audit of vendor security policy

- verify with the vendor the aderence to relevant security standards and regulation

### 11.6 Acceptance criterea 

- based on : test, audit and review

### 11.7 Mearure effectiveness of security controls

- KPI

### 11.8 Security accreditation

- formal declaration that envolves risk acceptance and sign-off by design authority

### 11.9 Security authorization

- refers to official management decision to allow the operation and acceptance risk

### 11.10 Security assessment

- envolves to evaluate the security controls, if they are implemented correctly and operating as expected

### 11.11 Security verification

- evaluates the implementation of security controls, through test and examination

### 12.0 Buffer overflow

- its when buffer memory is exceed and causes malicious attack

### 12.1 Stack overflow

- address (ret) points to memory address wrong

### 12.2 Heap overflow

- its a corruption in heap memory space

### 12.3 API

- weakness: 3third party because can be simple to code

### 12.4 Atack surface in the code

- is any point in the system that can be subject to unauthorized access

### 12.4 Software configuration Management

- includes documentation to all components, software build , version

### 12.5 EOL

- END of life -> remove credentials

### 12.6 Cryptographic risk

- broken algorithm , missing encryption of sensitive data

### 12.7 Architecture n tiered

- facilitates security because separates functionalities

### 12.8 cve

- enumerate software vulnerabilities

### 12.9 input and sanitization

- input validates data is correct and sanitization protects against malicious input

### 12.10 secure software attributes

- reliability,resiliency and recoverability 

### 13.0 security objectives

- legal and contract obligation and corporate standards and objectives

### 13.1 kerkhoff principal 

- about secrecy of a key rather than algorthim

### 13.2 object

- interacts with the system

### 13.3 n-tier architecure

- used to distrbute processing task among network devices while providing scalable and fault-tolerant architecture

### 13.4 description test case

- doesn't have business objective. just test conditions,input requirements and test case identifier

### 13.5 supply chain

- document: component tree

### 13.4 FITSAF (federal information technology security assessment framework)

- 1- policy, 2- implement policy, 3-procedement has been implemented,4-procedure was tested,5-asset has procedure and controls fully integrated

### 13.5 configuration audit

- is a component of configuration management, which involves checks to completeness accounting info and confirm all confg management policies are followed

### 13.6 status account

- supports the functional and physical atributes of software at the time. performs control of accounting to identify and mantain software integrity and traceability in development lofe cycle

### 13.7 configuration control

- is a set of process and approval stages to change configuration attributes and re-baseline them. change functional and physical attribute of software 

### 13.8 configuration identification

- is a product (hardware/software), are recorded in documentation and baseline(forces a formal change to be effected)

### 13.9 documentation control

- ensure system changes to be agreed upon before being implemented,its acurate

### 13.10 disaster recovery

- reliable actions to be taken before, during, after disruptive event that causes a considerable loss of information system resources.

### 13.11 contigency plan

- just when something is wrong

### 13.12 C&A (certification and accredition) before prod

- 1-initiation,2-security certification,3-security accrediation,4-continuous monitoring

### 14.0 structed walk though test

- table top exercises. identify area before conduct challenge exercises

### 14.1 teardrop

- its ip attack fragment  