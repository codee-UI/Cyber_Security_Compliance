# Cybersecurity Study Guide: Compliance, Identity, Defense in Depth, and Security Operations

## Module 1 — Industry Standards and Compliance Frameworks

### 1.1 Why standards and frameworks matter

Cybersecurity standards and compliance frameworks help organizations protect information and manage security risks. They support the three core security objectives:

- **Confidentiality:** Information is accessible only to authorized people.
- **Integrity:** Information remains accurate and protected from unauthorized modification.
- **Availability:** Systems and information remain accessible when needed.

### 1.2 Major standards and frameworks

| Framework | Main purpose | Key focus |
|---|---|---|
| ISO/IEC 27001 | Establish and continually improve an Information Security Management System (ISMS) | Risk management and information security controls |
| SOC 2 | Assess controls at service organizations | Security, availability, processing integrity, confidentiality, privacy |
| PCI DSS | Protect payment-card data | Secure payment environments |
| HIPAA | Protect specified health information under U.S. law | Privacy and security of protected health information |

#### ISO/IEC 27001

ISO/IEC 27001 provides a risk-based framework for establishing, implementing, maintaining, and continually improving an ISMS.

The planning activities described in the reading are:

1. Define the ISMS policy.
2. Determine the ISMS scope.
3. Conduct a risk assessment.
4. Manage identified risks.
5. Select control objectives and controls.
6. Prepare a Statement of Applicability (SoA).

The standard addresses areas such as access control, incident management, physical security, environmental security, and communications security.

Organizations use internal audits to evaluate their systems and may undergo external audits by an independent certification body to obtain certification.

#### SOC 2

SOC 2 is based on auditing procedures developed by the American Institute of Certified Public Accountants (AICPA).

It covers five Trust Services Criteria:

- Security
- Availability
- Processing integrity
- Confidentiality
- Privacy

SOC 2 reports help customers evaluate how a service organization manages controls relevant to protecting customer information.

A **Type I report** evaluates the design of controls at a specified point in time. A **Type II report** evaluates control design and operating effectiveness over a period of time.

#### PCI DSS

The Payment Card Industry Data Security Standard protects payment-card data. It applies to organizations that store, process, or transmit cardholder data and to other entities whose systems fall within the applicable scope.

Its security requirements cover areas such as network security, access control, vulnerability management, security policies, monitoring, and protection of payment information.

Maintaining compliance requires ongoing assessment and appropriate security controls.

#### HIPAA

The Health Insurance Portability and Accountability Act is a U.S. law that includes protections for health information.

The HIPAA Security Rule addresses electronic protected health information (ePHI) and requires appropriate:

- Administrative safeguards
- Physical safeguards
- Technical safeguards

HIPAA obligations depend on the organization's role and the information and activities involved.

### 1.3 How the frameworks work together

An organization may need to follow multiple frameworks simultaneously.

Examples:

- A healthcare organization may need to address HIPAA requirements and PCI DSS if it processes payment-card data.
- A cloud service provider may use ISO/IEC 27001 and SOC 2 to demonstrate its security management and control practices.
- An organization can use an ISMS as a foundation for coordinating several compliance requirements.

### 1.4 Benefits and challenges

**Benefits**
- Better security risk management.
- Greater customer and stakeholder confidence.
- Improved accountability and documentation.
- Support for applicable legal and regulatory obligations.

**Challenges**
- Implementation costs.
- Shortages of expertise.
- Complex technical and organizational requirements.
- Continuous monitoring and reassessment.

A risk-based approach, employee training, automation, and specialist assistance can help address these challenges.

---

## Module 2 — General Data Protection Regulation (GDPR)

### 2.1 What is GDPR?

The General Data Protection Regulation is an EU data protection regulation that took effect on **25 May 2018**. It establishes requirements for processing personal data and gives individuals rights concerning their information.

### 2.2 Personal data and processing

**Personal data** is information relating to an identified or identifiable individual. Examples include:

- Name and contact details.
- Identification numbers.
- Online identifiers.
- Employment and financial information.
- Health and genetic information.

**Processing** means performing operations on personal data, whether manually or automatically. Examples include collecting, recording, storing, retrieving, using, sharing, correcting, restricting, and deleting information.

A **data subject** is the individual to whom personal data relates.

### 2.3 Data subject rights

| Right | Meaning |
|---|---|
| Access | Find out whether personal data is being processed and obtain relevant information about it |
| Rectification | Correct inaccurate or incomplete data |
| Erasure | Request deletion in circumstances provided by GDPR |
| Restriction | Restrict processing in specified circumstances |
| Data portability | Receive certain personal data in a structured, commonly used, machine-readable format and transmit it where applicable |
| Objection | Object to certain processing activities in specified circumstances |

These rights have conditions and exceptions; they do not all apply unconditionally in every situation.

### 2.4 Six lawful bases for processing

An organization must identify an appropriate lawful basis for each processing activity.

1. **Consent:** The individual freely agrees to a specified use of their personal data.
2. **Contract:** Processing is necessary to perform a contract with the individual or take requested pre-contractual steps.
3. **Legal obligation:** Processing is necessary to comply with a legal obligation.
4. **Vital interests:** Processing is necessary to protect someone's life or other vital interests.
5. **Public task:** Processing is necessary for a task in the public interest or the exercise of official authority.
6. **Legitimate interests:** Processing is necessary for legitimate interests, provided those interests are not overridden by the individual's rights and freedoms.

Consent is not the only lawful basis, and organizations should not automatically use it when another basis is more appropriate.

### 2.5 Seven data protection principles

1. **Lawfulness, fairness, and transparency:** Process personal data lawfully and explain its use clearly.
2. **Purpose limitation:** Collect data for specified, explicit, legitimate purposes.
3. **Data minimization:** Collect only data that is necessary.
4. **Accuracy:** Keep personal data accurate and correct it when necessary.
5. **Storage limitation:** Retain personal data only as long as necessary, subject to applicable requirements.
6. **Integrity and confidentiality:** Protect data against unauthorized access, loss, destruction, or damage.
7. **Accountability:** Be able to demonstrate compliance with the principles.

### 2.6 Data controllers and processors

- **Controller:** Determines the purposes and essential means of processing personal data.
- **Processor:** Processes personal data on behalf of a controller.

Both can have GDPR obligations, although their responsibilities differ.

### 2.7 Territorial scope and breach notification

GDPR can apply to organizations outside the EU when its territorial-scope conditions are met, including certain activities involving offering goods or services to people in the EU or monitoring their behavior there. It does not automatically apply simply because an organization processes data belonging to any EU citizen.

Under Article 33, a controller generally must notify the relevant supervisory authority of a personal data breach without undue delay and, where feasible, within 72 hours after becoming aware of it, unless the breach is unlikely to result in a risk to individuals' rights and freedoms. Article 34 addresses communication to affected individuals when a breach is likely to result in a high risk, subject to its conditions.

---

## Module 3 — Identity Management and Active Directory

### 3.1 Identity management

Identity management involves managing digital identities, authentication, authorization, roles, and access to organizational resources.

Two central concepts are:

- **Authentication:** Verifying who a user or system is.
- **Authorization:** Determining which actions or resources an authenticated identity is permitted to access.

Authentication does not automatically grant permission to every resource.

### 3.2 Active Directory (AD)

Active Directory Domain Services (AD DS) is a Microsoft directory service used in Windows domain environments. It supports centralized identity and computer management and integrates with technologies such as Kerberos, LDAP, and DNS.

AD can maintain objects representing:

- Users
- Computers
- Groups
- Printers
- Other directory resources

### 3.3 Access control lists (ACLs)

An ACL defines permissions associated with a securable object. Its entries specify which users or groups receive particular access rights.

For example, a shared folder might allow the Finance group to read and modify its files while allowing other employees no access.

Effective access depends on the applicable permissions and the system's access-control rules.

### 3.4 Identity federation and SSO

**Identity federation** enables one identity system to establish trusted identity information for another system.

**Single sign-on (SSO)** lets users authenticate once and access multiple applications or services without repeatedly entering their credentials, subject to each application's access requirements.

Active Directory Federation Services (AD FS) is Microsoft's federation technology for supported enterprise scenarios. It can issue claims-based security tokens that a trusted partner uses to make access decisions.

A simplified flow is:

1. The user requests access to a partner application.
2. The application redirects the user to an identity provider when necessary.
3. The identity provider authenticates the user.
4. It issues a token containing relevant claims.
5. The application validates the token and evaluates authorization.
6. Access is granted or denied.

A valid token proves specified identity claims; it does not mean that every requested action must be authorized.

### 3.5 Group Policy and centralized administration

Active Directory environments can use Group Policy to manage configurations across users and computers.

For example, an organization can configure company computers to use approved security settings, enforce screen-lock requirements, and apply supported operating-system policies.

---

## Module 4 — Group Policy

### 4.1 Purpose

Group Policy allows administrators to centrally manage many Windows settings in a domain environment rather than configuring each computer individually.

Common uses include:

- Password and account policies.
- User environment settings.
- Security configurations.
- Software deployment in supported scenarios.
- Scripts and administrative settings.
- Update-related policies.

### 4.2 Two configuration categories

**User Configuration** applies settings associated with user accounts, such as certain desktop and application settings.

**Computer Configuration** applies settings to computers, such as system-level security settings and machine configuration.

The exact settings available depend on the Windows version, administrative templates, and policy environment.

### 4.3 How Group Policy is applied

A Group Policy Object (GPO) contains policy settings. Administrators link GPOs to relevant Active Directory sites, domains, or organizational units (OUs).

For example, a company could create an OU for point-of-sale computers and link a GPO that configures appropriate screen-lock and security settings.

Placing a computer in the relevant OU allows the linked policies to apply according to Group Policy processing rules and any filtering or precedence considerations.

### 4.4 Best practices

1. **Plan:** Define the intended security and operational outcomes.
2. **Test:** Validate policies in a controlled test environment.
3. **Keep policies simple:** Avoid unnecessary complexity and overlapping settings.
4. **Document:** Record each policy's purpose, owner, scope, and change history.
5. **Validate:** Confirm that policies actually apply as intended.
6. **Maintain rollback options:** Know how to reverse a change if it causes problems.

Group Policy is powerful, but a poorly scoped policy can affect many systems at once.

---

## Module 5 — Microsoft Entra ID and Cloud Identity

### 5.1 Azure Active Directory's current name

Microsoft renamed **Azure Active Directory (Azure AD)** to **Microsoft Entra ID** in 2023. The older name remains common in learning materials.

Microsoft Entra ID is a cloud identity and access management service. It is distinct from traditional on-premises Active Directory Domain Services, although organizations can integrate them.

### 5.2 Tenants and domains

A **tenant** is an organization's dedicated identity and resource directory in the Microsoft cloud.

A tenant contains objects and configuration such as users, groups, application registrations, domains, and access policies.

A default domain commonly follows this pattern:

`yourorganization.onmicrosoft.com`

Organizations can also associate verified custom domains, such as `example.com`.

### 5.3 Applications

Microsoft Entra ID can support access to:

- Microsoft cloud services.
- Third-party SaaS applications.
- Custom-built organizational applications.
- APIs and integrated services.

Application registrations and enterprise application configurations support identity integration and access management.

OAuth 2.0 is commonly used for delegated or application authorization, while OpenID Connect provides an authentication layer built on OAuth 2.0.

### 5.4 Key identity and access features

| Feature | Purpose |
|---|---|
| SSO | Simplifies access to multiple applications |
| MFA | Requires additional authentication evidence beyond a password |
| Conditional Access | Evaluates signals and policies before granting access |
| Privileged Identity Management (PIM) | Helps control and monitor privileged role assignments and activation |
| Identity Protection | Detects identity-related risks and supports risk-based responses |

MFA reduces the impact of stolen passwords. Conditional Access can require stronger authentication, restrict access, or apply other controls based on factors such as user risk, application, device state, and location.

---

## Module 6 — Defense in Depth

### 6.1 Definition

Defense in depth is a security strategy that combines multiple layers of controls. If one control fails, additional controls can reduce the likelihood or impact of a successful attack.

It combines preventive, detective, and corrective measures.

### 6.2 Main layers

**1. Physical security**
- Controlled entry.
- Security personnel and cameras.
- Door locks and alarms.
- Protection of equipment and facilities.

**2. Identity and access security**
- Strong authentication.
- MFA.
- Least privilege.
- Role-based permissions.

**3. Network security**
- Firewalls.
- IDS and IPS.
- Network access control.
- Network segmentation.

**4. Endpoint security**
- Anti-malware tools.
- Endpoint detection and response.
- Secure configurations.
- Timely patching.

**5. Data security**
- Encryption at rest and in transit.
- Access restrictions.
- Secure key management.
- Data-loss prevention where appropriate.

**6. Monitoring and response**
- Centralized logs.
- Security alerts.
- Incident response procedures.
- Backup and recovery processes.

### 6.3 Network segmentation and least privilege

Network segmentation divides a network into smaller security zones. Communication between zones is controlled according to business requirements.

For example, payroll systems can be separated from guest Wi-Fi and point-of-sale networks. If one zone is compromised, segmentation can make unauthorized movement to other zones more difficult.

The **principle of least privilege** means that each user, device, and service receives only the access necessary for its legitimate tasks.

### 6.4 Encryption

Encryption protects information by transforming readable data into a form that requires the appropriate key to recover.

- **Data at rest:** Information stored on disks, databases, or backups.
- **Data in transit:** Information travelling between systems.

Encryption is not a complete substitute for access control. If an attacker obtains an authorized session or the necessary keys, encrypted data may still be exposed.

### 6.5 Incident response

Defense in depth assumes that preventive controls can fail. Incident response therefore helps organizations:

1. Prepare for incidents.
2. Detect and analyze suspicious activity.
3. Contain affected systems.
4. Eradicate the cause.
5. Recover services safely.
6. Review lessons learned and improve controls.

---

## Module 7 — Cloud Security and Shared Responsibility

### 7.1 Shared responsibility model

Cloud security responsibilities are divided between the cloud service provider and the customer. The exact division depends on the service model and provider.

The provider generally secures the underlying cloud infrastructure, while the customer retains responsibilities for appropriate use and configuration of cloud services.

| Area | Typical responsibility |
|---|---|
| Physical data-center security | Cloud provider |
| Underlying cloud infrastructure | Cloud provider |
| User identities and permissions | Customer, with provider tools |
| Data classification and appropriate use | Customer |
| Cloud resource configuration | Customer, depending on service |
| Application and operating-system security | Shared or customer-led, depending on service model |
| Endpoints and customer networks | Customer |

### 7.2 IaaS, PaaS, and SaaS

- **Infrastructure as a Service (IaaS):** The customer generally has more responsibility for guest operating systems, applications, identities, and configuration.
- **Platform as a Service (PaaS):** The provider manages more of the underlying platform, while the customer remains responsible for application logic, data, access, and service configuration.
- **Software as a Service (SaaS):** The provider manages the application platform, but customers still need to manage identities, permissions, data handling, and their own devices.

**Key principle:** Moving data to the cloud does not transfer every security responsibility to the provider.

---

## Module 8 — Security Operations and Monitoring

### 8.1 Security Operations Center (SOC)

A Security Operations Center is a team or function responsible for monitoring and improving an organization's security posture. Its work can include:

- Monitoring systems and networks.
- Investigating alerts.
- Using threat intelligence.
- Responding to incidents.
- Coordinating containment and recovery.
- Supporting security reporting and compliance.

### 8.2 Intrusion Detection Systems (IDS)

An IDS monitors systems or network traffic for suspicious activities and potential policy violations.

Common detection approaches include:

- **Signature-based detection:** Identifies patterns associated with known threats.
- **Anomaly-based detection:** Identifies activity that deviates from an established baseline.

An IDS typically generates alerts. An intrusion prevention system (IPS) can also take configured actions to block or limit detected activity.

### 8.3 Security Information and Event Management (SIEM)

A SIEM collects and correlates security-relevant data from multiple sources, such as servers, endpoints, identity systems, firewalls, and cloud services.

It can help security teams identify patterns that are difficult to see in individual logs.

Example: An unusual sign-in, followed by a privileged account change and suspicious data transfers, may become more concerning when the events are correlated.

### 8.4 Log management

Log management focuses on collecting, storing, organizing, searching, and reporting log data.

Logs support:
- Troubleshooting.
- Auditing.
- Incident investigations.
- Detection engineering.
- Compliance evidence.

A log repository is useful only if records are sufficiently complete, protected from inappropriate modification, retained appropriately, and reviewed when needed.

### 8.5 Effective security operations practices

**Automation and machine learning:** Help process large amounts of telemetry, prioritize alerts, and support investigation. Automated detections can still produce false positives or miss threats.

**Continuous training:** Keeps security staff familiar with changing threats, tools, procedures, and legal and ethical responsibilities.

**Incident response planning:** Defines responsibilities, escalation paths, communications, containment, recovery, and review procedures.

**Patch management:** Tracks vulnerabilities and updates, assesses risk, tests changes when appropriate, deploys patches, and verifies successful installation.

---

## Module 9 — Practical Integrated Scenario

### Scenario: Sam's Scoops

Sam's Scoops operates three stores. Employees use point-of-sale computers, shared business applications, and a cloud-based inventory service. The organization also stores employee information and processes customer payments.

A sensible security design could include:

1. **Compliance:** Identify which legal obligations and payment-security requirements apply.
2. **Identity:** Give each employee an individual account rather than a shared administrator account.
3. **Authentication:** Require MFA for sensitive administrative and cloud access.
4. **Authorization:** Give cashiers, managers, and administrators different permissions.
5. **Group Policy:** Apply suitable Windows security configurations to domain-managed computers.
6. **Segmentation:** Separate point-of-sale systems from guest Wi-Fi and other less-trusted networks.
7. **Endpoint protection:** Maintain supported software, security tools, and appropriate configurations.
8. **Cloud security:** Review permissions, protect stored data, and understand provider/customer responsibilities.
9. **Monitoring:** Collect relevant logs and investigate suspicious sign-ins or payment-system activity.
10. **Incident response:** Prepare procedures for containing compromised accounts, investigating incidents, and restoring services.

These controls complement each other. For example, MFA may prevent some account takeovers, segmentation may limit an attacker's movement, and monitoring may help detect activity that bypasses prevention.

---

## Module 10 — Knowledge Check

### Questions

1. What is the main purpose of ISO/IEC 27001?
2. Name the five SOC 2 Trust Services Criteria.
3. What is the purpose of PCI DSS?
4. What type of information does the HIPAA Security Rule address?
5. What is the difference between a data controller and a data processor?
6. Name the six lawful bases for processing personal data under GDPR.
7. What is the difference between authentication and authorization?
8. How do ACLs help enforce access control?
9. What is identity federation, and how does it relate to SSO?
10. What are the two main Group Policy configuration categories?
11. What is the difference between Active Directory Domain Services and Microsoft Entra ID?
12. How do network segmentation and least privilege reduce risk?
13. What is the difference between an IDS and an IPS?
14. What is the role of a SIEM in security operations?
15. Which cloud security responsibilities commonly remain with the customer?

### Answer key

1. To establish and continually improve a risk-based information security management system.
2. Security, availability, processing integrity, confidentiality, and privacy.
3. To protect payment-card data and the systems in scope that handle it.
4. Electronic protected health information (ePHI).
5. A controller determines the purposes and essential means of processing; a processor handles data on the controller's behalf.
6. Consent, contract, legal obligation, vital interests, public task, and legitimate interests.
7. Authentication verifies identity; authorization determines permitted access.
8. ACLs define which identities can perform specified actions on an object.
9. Federation allows trusted identity information to be accepted across systems; SSO enables convenient access to multiple applications after authentication.
10. User Configuration and Computer Configuration.
11. AD DS is an on-premises Windows domain directory service; Entra ID is Microsoft's cloud identity and access management service.
12. Segmentation limits unnecessary communication between zones; least privilege limits each identity's permissions.
13. An IDS detects and alerts; an IPS can also block or prevent configured threats.
14. It collects and correlates security events to support detection, investigation, and response.
15. Common examples include identity permissions, data handling, endpoint security, and secure resource configuration, depending on the service model.

---

## Essential Glossary

| Term | Definition |
|---|---|
| ISMS | Information Security Management System |
| SoA | Statement of Applicability |
| ePHI | Electronic Protected Health Information |
| GDPR | General Data Protection Regulation |
| Data subject | Individual whose personal data is processed |
| ACL | Access Control List |
| AD DS | Active Directory Domain Services |
| GPO | Group Policy Object |
| SSO | Single Sign-On |
| MFA | Multi-Factor Authentication |
| IAM | Identity and Access Management |
| SIEM | Security Information and Event Management |
| IDS | Intrusion Detection System |
| IPS | Intrusion Prevention System |
| SOC | Security Operations Center; in the compliance context, SOC also refers to System and Organization Controls |
| EDR | Endpoint Detection and Response |
| IaaS | Infrastructure as a Service |
| PaaS | Platform as a Service |
| SaaS | Software as a Service |

**Final takeaway:** Effective cybersecurity combines governance and compliance, privacy protection, controlled identities and permissions, layered defenses, secure cloud configuration, continuous monitoring, and tested incident response. No single framework or tool replaces the need for a coordinated security program.