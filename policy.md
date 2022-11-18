# Grafana Labs bug bounty policy

## Introduction

With this bug bounty program (the “Program”) Grafana Labs aims to provide a stellar experience to security researchers and others (the “Participants”) who wish to submit reports to Grafana Labs regarding security vulnerabilities.\
To do so participants must **create a security advisory via our [dedicated GitHub page](https://github.com/grafana/tobechanged/security/advisories)**.\
As a condition to participating in the Program all Participants acknowledge and agree to the following terms and conditions:

## Terms and Conditions

1. Participants must follow the following guidelines in order to be eligible to receive any payouts pursuant to this Program:.
    * **Only local testing of In-Scope products detailed in the section titled “Scope” below is allowed** (either via installing local development environments or running the publicly available Docker images)
    * Do not disclose any issue publicly before a fix has been released by Grafana Labs (even if you have already received the reward)
    * Participants may at no time disrupt any Grafana Labs service
    * Participants may not access any accounts or data other than their own
    * Do not post attachments or Proof Of Concepts (POCs) on a 3rd party website, instead participants must include them in the [security advisory](https://github.com/grafana/tobechanged/security/advisories)
    * Participants must comply with all applicable laws
    * Submissions must be made in English
    * All actions must be performed strictly during participation in the Program and in adherence with this Policy
    * All actions must be performed as good faith security research, with the intent to report to Grafana Labs
2. All payouts made pursuant to this policy shall be calculated and paid at the sole discretion of Grafana Labs. All payments made by Grafana Labs are final and binding. Participants in this program shall be solely responsible for the payment of all applicable taxes. 
3. Grafana Labs reserves the right to change the rules of this program at any time in its sole discretion
4. By providing a report to Grafana Labs pursuant to this policy, you grant Grafana Labs an irrevocable, perpetual, royalty free, worldwide license to use and exploit the report.
5. Any report can be made public at the discretion of Grafana Labs 
6. Eligibility of Participants to participate in the Program shall be determined at the sole discretion of Grafana Labs. Individuals located in any country subject to a U.S. embargo or listed on any sanctioned persons list shall not be permitted to participate.
7. Safe harbor: Activities conducted in a manner consistent with this Policy will be considered authorized conduct and we will not initiate legal action against you for breach of any applicable license provisions. Note that you are still responsible for compliance with any local laws, and that this safe harbor does not extend to breach of any laws applicable to you.
8. Current or former (in the last 12 months) Grafana Labs employees and contractors are not permitted to participate in this program. 
9. We target an initial response to requests within 1 business day and triage within 2 business days. Payouts should happen as soon as the vulnerability is confirmed (i.e. at triage time). Payouts are based on CVSS score and bonus points and are calculated by Grafana Labs in its sole discretion.
10. Grafana Labs reserves the right to make a determination of whether a violation of this policy is accidental or in good faith. When in doubt, please contact us at legal@grafana.com.
11. Governing Law; Limitation of Liability: The law that will apply in any dispute or lawsuit arising out of or in connection with this Program, and the courts that have jurisdiction over any such dispute or lawsuit will be New York, USA. In no event shall Grafana Labs be liable for any damages relating to the Program greater than USD$1,000.

## Scope

### In scope:
* [Grafana OSS](https://github.com/grafana/grafana) (i.e. core, not plugins)
* [Mimir](https://github.com/grafana/mimir)

Valid vulnerabilities on any product not explicitly listed in scope will be accepted but not eligible for a reward.

### Out of scope:
* Our customers’ Grafana installs
* Automated scanning or reporting of any kind
* Reports about security weaknesses with no proven impact will be processed as public issues and not be eligible for a reward.\
  This category includes but is not limited to:
    * CVE in an outdated dependency
    * Defense in depth option not implemented (e.g. missing cookie attribute or HTTP header, clickjacking included)
    * Secure coding best practice not used
    * TLS configuration with older ciphersuites
    * Logout CSRF
    * Self exploitation (e.g. Self XSS or token reuse)
* Brute forcing and enumeration attacks
* Denial of service with a temporary impact on performance
* Social engineering with a Low CVSS score (i.e when CVSS score is under 4.0 and User Interaction (UI) is Required)
* [Grafana plugins](https://grafana.com/grafana/plugins/)
* [Viewer role in Grafana](https://grafana.com/docs/grafana/latest/setup-grafana/configure-security/#limit-viewer-query-permissions) tampering dashboard queries

## Rewards


