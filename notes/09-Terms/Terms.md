# Terms

## Secure Design Tenets

### Good Enough Security

Appropriate level of security for any given system.

### Least Privilege

Programs and users (subjects) should only have the bare minimum rights and privileges to perform current task

### Separation of Duties

More than one person needs to be involved for any given task so no single person can abuse the system

### Defense in Depth

A.k.a. layered security or diversity defense.

Software should have multiple layers of defenses that are dissimilar in nature. ❗ True goal of security is to make the cost/time/effort of exploiting a system more than it is worth to an adversary.

### Fail-safe

When a system fails, it should fail to a safe state. E.g. explicit deny

### Economy of Mechanism

Greater system or software complexity generally results in worse security. Troubleshooting issues gets more difficult the more complex something is. This also includes turning off/disabling protocols and services that are not needed.

### Complete Mediation

When a subject is authorized, verification should occur every time access to an object is requested.

### Open Design

❗ Security by obscurity does not provide actual security!

### Least Common Mechanism

Multiple, different processes that share common mechanisms can lead to inadvertent sharing of information. Better to keep processes completely separate.

### Leverage Existing Components

Reuse components so the attack surface of a system is reduced. ❗ This often results in a larger footprint when errors occur.

### Psychological Acceptability

When securing a system or software, the controls should not obstruct the user and ease-of-use enough that the user is motivated to circumvent the controls.

### Weakest Link

This is the common point of failure for all systems. A system is only as strong as its weakest link.

### Single Point of Failure

An entire system should not fail if a single aspect fails.

## Access Control Models

### Mandatory Access Control

Restrict access based on sensitivity of the information in the object and whether the subject is authorized to access information with that level of sensitivity.

### Discretionary Access Control

The owner of an object specifies which subjects have access and what level of access each subject has.
❗ It is optional (discretionary) and requires owner to define access for all objects under its control.

### Role-based Access Control

A user is assigned to any number of potentially overlapping roles. Roles are then assigned access.

### Rule-based Access Control

Building rules into ACLs. Examples include time-of-day or network restrictions.

### Attribute-based Access Control

- technique relies on set of rules to determine the object will be granted

Grant access based on attributes associated with the subject.

### Simple Security Rule

Subjects can only read objects they are authorized to read.

## Risk Management Terms

### Risk

Possibility of suffering harm/loss

### Inherent risk

product of likelihood and impact prior to implementing controls

### Residual risk

Remaining risk after control is utilized. Residual risk is owned by the entity

### Total risk

Sum of all risks associated with an asset, process, or even a business

### Risk management

Decision-making process of identifying threats and vulnerabilities, potential impacts, determining costs to mitigate, and deciding what actions are cost-effective

### Risk assessment (risk analysis)

- Analyze environment to identify threats and vulnerabilities and mitigating actions to determine impact of an event
- include specific threats, risk/impact for each threat, relationship between assets

### Asset

Any resource or information an org needs to conduct business

### Vulnerability

Any characteristic of an asset that can be exploited by a threat to cause harm

### Attack

Attempting to perform undesired or unauthorized activities via a vulnerability

### Impact

Resulting loss when a threat exploits a vulnerability

### Threat

Any circumstance or event with the potential to cause harm to an asset

### Mitigate

An action taken to reduce the likelihood of a threat occurring

### Control (a.k.a. countermeasure or safeguard)

A measure taken to detect, prevent, or mitigate the risk associated with a threat.

### Qualitative risk assessment

Subjectively determine impact of an event - involves experts and group consensus

## Quantitative Terms

### Quantitative risk assessment

Objectively determine impact of an event - involves use of metrics and models

### Single loss expectancy (SLE)

monetary loss or impact of each occurrence of a threat

### Exposure factor

measure of magnitude of loss of an asset, used to calculate SLE

### Annualized rate of occurrence (ARO)

how many times expected to occur annually

### Annualized loss expectancy (ALE)

how much an event is expected to cost per year

## Supply Chain Terms

### COTS

commercial off the shelf

### ICT

information and communications technology

### TOE

target of evaluation

## Secure Software Testing

### Entropy

randomness collected by an OS or application for use in cryptography. High entropy results in a random number being generated with more randomness (e.g. not related to date/time) 

## Secure Software Lifecycle Management

### Cumulative failure profile

graphical method used to predict reliability, estimate additional testing time, identify modules/subsystems that require additional testing

## Secure Software Supply Chain Terms

### Provenance

origin and license of third-party components used in software