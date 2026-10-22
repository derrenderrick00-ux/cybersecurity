# DAY ONE 21-10-2026 (Wednesday)
This first area gives you the vocabulary and mental models that every other topic builds on. If you truly
understand assets, threats, vulnerabilities, risk, the CIA triad and defence in depth, you can reason about
almost any security problem, even one you have never seen before

## OBJECTIVES 

By the end of this area you will be able to:
• Define cyber security and distinguish it from information security and network security.
• Explain asset, threat, vulnerability, exploit and risk, and how they connect.
• Explain the CIA triad and map any incident to the property it violates.
• Classify controls as preventive, detective or corrective, and as administrative, technical or physical.
• Describe defence in depth and apply it to a real system.
• Name the main security domains and career paths.
• Explain the legal and ethical limits of security work.

## INTRODUCTION
**CYBER SECURITY**: Protecting computers, networks, data, applications and the people use them from attack, unauthorized access and damage.
**INFORMATION SECURITY**: It's the wider goal of protecting information in any form(digital, spoken, paper), cyber security is the digital part of it
    - Case scenerio -----> A corporate finance worker falls for a targeted phishing email disguised as an urgent payroll update
**ASSET**: Anything of value that needs prtection. *(data, digital devices, bank account, software, reputation and people)*
**THREAT**: Anything that can cause harm to an asset *(malware, careless employee, natural disaster, an attacker)*
**THREAT ACTOR**: A person or an organization behind a threat *(hacktivist, crimninal, insider)*
**VULNERALBILITY**: A weakness in the system that could be exploited by a threat actor. *(weak password, careless employee, software bug, untrained employee, misconfiguration, outdated software)*
**EXPLOIT**: Method or tool that takes the advantage of a vulnerability.
**RISK**: potential for loss, damage or destruction of a digital asset of an organination when a vulnerability is exploited *(RISK= THREAT X VULNERALBILITY X IMPACT)*
**ATTACK SURFACE**: Set of points an attacker could try to attack into or extract data. *( an attacker could try to log into the admin dashboard or extract data from a DB)*
**CONTROL (SAFEGUARD)**: Any measure taken to reduce risk. *(password policy, firewall, MFA, antivirus)*
**CONFIDETIALITY**: Only authorized personnel are authorised to view the information. *(if user data is disclosed to unauthorized people then confidetiality is compromised)*
**INTEGRITY**: data should not be modified without the consent of the user(data and information should be correct and accurate and should not be changed)
**AVAILABILITU**: data and information should be available to the user when needed.
**DEFENCE INDEPTH**: Using diferrent layers of control so that if one fails the other still protect the asset.

    --------------------------------CASE SCENERIO---------------------------------------
    An employee accidentally downloads a malicious email attachment, but multiple layers of independent security controls stop the attack at different stages, preventing a data breach. Defense in Depth ensures that if one security measure fails, others are waiting behind it to block the threat.

    The Attack Scenario

    A regional manager receives a sophisticated phishing email that bypasses the company's initial email filters. The email contains a malicious document disguised as a vendor invoice.

    The Layers of Defense in Action

    • Layer 1: Security Awareness (Human Layer) — Failed
        The manager fails to notice the subtle signs of phishing and opens the attachment.
    • Layer 2: Endpoint Protection (Device Layer) — Failed
        The malware is a brand-new variant ("zero-day") that local antivirus software does not immediately recognize, allowing it to execute on the laptop.
    • Layer 3: Endpoint Privilege Management (Identity Layer) — Passed
        The malware tries to install a hidden program to gain administrative control. However, the manager's account operates under the Principle of Least Privilege (non-admin rights). A prompt appears asking for admin credentials, blocking the automatic installation.
    • Layer 4: Network Segmentation (Network Layer) — Passed
        Frustrated, the malware attempts to scan the corporate network to find other computers to infect. Because the department is isolated on its own segmented virtual network (VLAN), the malware cannot see or touch the critical finance or customer databases.
    • Layer 5: Intrusion Detection System (Monitoring Layer) — Passed
        The unusual network scanning traffic triggers an alert in the Security Operations Center (SOC). AI-driven behavioral monitoring flags the laptop as compromised.
    • Layer 6: Incident Response (Operational Layer) — Passed
        The security team receives the alert and automatically isolates the manager's laptop from the network, containing the threat entirely before any data can be stolen or encrypted.

    Summary of Benefits

    By employing a Defense in Depth strategy, the organization did not rely on a single perfect defense. The failure of email filtering and endpoint antivirus was mitigated by strict user permission limits, strong network design, and rapid automated response.


# DAY TWO 22-10-2026 (Thursday)
## TYPES OF SECURITY CONTROLS
**PREVENTIVE**: Stop the incident from happening *(MFA, input validation, firewall policy)*
**DETECTIVE**: Notice that sth is happening or happened *(logs alert, CCTV, intrusion detection)*
**CORRECTIVE**: fix the damage and stop it from spreading *(restore from backup, reseting password, quarantine malware)*
**DETERENT**: discourage attackers *(using cameras, warning banners, legal policies)*
**RECOVERY**: Return to normal activities.

## Security domains and roles
    -Blue team (defence): *SOC (Security Operation Centre) analyst,
                          *incident responder,
                          *security engineer, 
                          *threat hunter.
    -Red team (offence): *penetration tester, 
                         *red team operator, 
                         *exploit researcher.
    -GRC: Governance, Risk and Compliance; policy writers, auditors, privacy officers.
    -Application security / DevSecOps: building security into software and pipelines.
    -Cloud, network and identity security: protecting infrastructure and access.
    -Forensics and malware analysis: investigating what happened after an incident.

## SECURITY ANALYSIS
- you shoud check for:
    -Asset
    -Threat, Threat actor and The vulnerability
    - Risk(risk=Threat X vulnerability X Impact);
    -CIA affected
    -Security controls


## EXERCISES
Draw the defence-in-depth layers for a school computer lab.
-using grilled windows
-using metalic doors
-installing CCTVs
-employing a security guard
-using logs for visitors who enter the lab
-allowing only authorized access
-using passwords on the computers


    