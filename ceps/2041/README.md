# CEP 2040: CDEV Red Team Tradecraft Best Practice

## Abstract
This CEP outlines the requirements and best practice for CDEV red team attack chain development. Notable items include outlining a tier list to map level of tradecraft and sophistication of the emulated threat, the requirement for MITRE ATT&CK Framework items to each part of the attack chain, and a documented proof of concept (POC) walkthrough for CDEV red team engagements.

## Rationale
This CEP aims to solidify many of the practices already in place with the CDEV red team in order to improve the development cycle of attack chains for CTFs and exercises. It recommends a set of guidelines to improve the quality and efficacy of CDEV's red side engagements to provide realistic threat scenarios.

### Attack Chain Development and MITRE ATT&CK Framework
Threat presentation constantly evolves and CDEV must evolve with it. 

To provide the most realistic training scenarios possible for our clients, CDEV must stay current with the present state of cybersecurity threat groups and tactics, techniques, and procedures (TTPs). CDEV Red Team attack chains be designed with clear mappings from threat presentation to the MITRE ATT&CK Framework for all phases of the attack. These mappings must be documented throughout the development process and documented when the attack chain is finalized.

An example of a MITRE ATT&CK Framework mapping is below:
MITRE ATT&CK Mappings

````
Nmap scan
https://attack.mitre.org/techniques/T1046/

Fallback Channels
https://attack.mitre.org/techniques/T1008/

C2 Beacon implant: 
Signed Binary Proxy Execution
https://attack.mitre.org/techniques/T1218/
Rundll32.exe
https://attack.mitre.org/techniques/T1218/011/
````

There is no prescribed format for this mapping but the MITRE items must be clearly tied to each phase of the attack chain. This document should be kept on the Confluence page of the CTF or exercise.

### Attack Chain Walkthrough Documentation
At a minimum, each attack chain should have a set of POC steps that allow for replication of the attack from a technical standpoint. When finalized, this document should also be kept on the CTF's Confluence page. The POC must be written in such a way that an author of comparable technical competency can recreate the attack from the steps alone. This document can also be a narrative of the attack chain to provide further context for the actions. Note that this document and the MITRE ATT&CK Framework mapping document should be the same item to simplify the record keeping process.

An except from an attack chain narrative example is below:


>.....
>
>Site.lan has a new site-guest subnet at 172.16.5.0/24, located between the firewall and core router.This guest subnet is notionally located in a common area inside of the company that is accessible to the public. An adversary has dropped “RaspberrySpy” into an ethernet port within this common area and hidden it away from sight. RaspberrySpy has Responder, Impacket, and some other red teaming tools....
>
>The Spy runs Responder and NTLMRelayx and waits for a user to connect...
> 
>Philip.holt makes a DNS mistake or clicks on a link to the malicious Spy server at 172.16.5.15
>
> Username: Philip.holt, Password: s$i3@7G$Jt8K
>
> Red operator uses these creds to psexec onto DC
>
>....


### TTP Levels and Characteristics
During attack chain development, it is important to identify the level of threat presentation and their capabilities. The level of sophistication of the threat should match the intended audience and their skill levels.

For example, an instructional module may train a student on the use of Wireshark by presenting more obvious indicators of compromise, including a foreign IP address, a strange DNS request name, or an executable called "evil.exe." In a beginner level instructional module, it is beneficial to keep the tradecraft sophistication level low to reinforce the concepts of the module itself.

Contrast this with an exercise or challenge module in the same series, where the student is now attempting to identify more sophisticated tradecraft and may find geographically similar IP addresses, DNS names that resemble actual companies, and executables named "msftupdater.exe" or "svchost.exe."

It is important to design attack chains with this in mind to fit the level of tradecraft to the content module, exercise, or CTF that is in development.

The tier list below is used by the SimSpace Red Team during their engagement design phase and should assist in tailoring the level of tradecraft to the scenario. Scenario development should identify a tier of TTPs to emulate during an attack chain development and use this list below as a starting point on how to emulate the threat actor's level of sophistication

````
Below are some of the most commonly outlined TTPs for each threat tier:

Low Tier
    
* Commonly used, open sourced Remote Access Tools (RATs)
* Command and Control (C2) use IP addresses only 
* IP addresses from foreign countries
* The use of the same IP address from payload delivery and callbacks
* External DMZ scanning
* Poorly written phishing & spearphishing emails
* Simple web shells
* Exploitation of web facing servers
* Target non-admin users/accounts
* No lateral movement
* Exfiltrate opportunistic data 

Medium Tier
   
* Lesser known open source or commercial RAT
* Command and Control (C2) resolve to domains/IPs
* Domains resolve to US IP addresses
* Separate domains for payload delivery and callbacks
* Internal network reconnaissance
* Legitimate looking spearphishing emails
* Custom web shells
* Endpoint exploitation
* Target all users, particularly domain admins
* Multiple lateral movement techniques
* Exfiltration of sensitive data; possibly staged
* The use of obfuscated and self-signed payloads

High Tier

* Anything from Medium tier, just slower and stealthier
* Lesser known open source, commercial, and custom developed tools
* Command and Control (C2) resolves to multiple domains
* Redundant callback domains for fail-over
* Separate domains/C2 used for delivery, callbacks, and exfil
* Previous knowledge of or even access to internal network
* Pre-staged beaconing implants
* Lateral movement
* Use of encrypted tunnels
* Targeted exfiltration of sensitive data
* Use of 0-day exploits
* Use of obfuscated & digitally signed payloads
````


### Requirements
- Content authors must design red teaming engagements for CTFs to emulate real world threats. Each phase of a given attack chain must be mapped to items from the MITRE ATT&CK Framework. This mapping must be documented on the module's Confluence page.
- Content authors must document a set of proof of concept steps for each attack chain written in such a way that an author of comparable technical competency can recreate the attack from the steps alone.
- The POC document may also be written as a general attack narrative that provides additional context to the actions and tradecraft considerations. Brief text descriptions of the attack chain phases are good additions to the step by step POC document.
- Content authors will make effort to tailor the tradecraft and sophistication levels of the emulated threats to the module's intended audience and their skill levels. A list of TTPs and their general sophistication levels is available in the section above.


## References and Footnotes

