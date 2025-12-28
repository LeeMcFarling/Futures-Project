---
title: "Decentralized Digital Identity"
author: "Lee McFarling"
category: "Technology"
subcategories:
  - Digital Identity
  - Privacy
  - Cybersecurity
status: "Draft"
version: "1.0"
last_updated: "2025-10-05"
tags:
  - decentralized identity
  - verifiable credentials
  - zero-knowledge proofs
  - self-sovereign identity
  - digital privacy
  - data brokers
  - web3
  - quantum resistance
  - modernization
summary: >
  This policy brief explores how a decentralized, cryptographically secure digital identity system—
  rooted in user-controlled verifiable credentials—can eliminate the data brokerage industry, protect
  citizens’ privacy, and serve as a foundation for a modern civic information infrastructure.
linked_policies:
  - Governance/Data_Governance_Framework.md
  - Economy/Data_Dividend_Proposal.md
related_initiatives:
  - Project_Digital_ID
license: "CC BY-NC-SA 4.0"
---

# **Title: Decentralized Digital Identity**
Author: Lee McFarling

## **Executive Summary**

The United States faces an escalating privacy crisis, culminating in the emergence of a surveillance capitalist state. Social media platforms, modern web browsers, smartphones, and computers now collect unprecedented volumes of data on U.S. citizens—continuously, throughout every moment of their day.

This data—ranging from what we see and interact with, to our personality traits, political leanings, financial transactions, and credit card activity—is not only aggregated and used to build highly manipulative algorithms, but is also increasingly being cross-referenced across platforms and sold by data brokers on a sprawling, opaque digital marketplace.

Today, information that would have once required a federal search warrant can often be purchased freely by anyone—corporations, foreign governments, or malicious actors. The ability of these entities to collect, exploit, and sell personal data at scale represents a systemic threat to consumer privacy, digital security, and the functioning of democratic governance itself.

However, emerging technologies offer a path forward.

This brief outlines how a decentralized, quantum-resistant digital identity system can render the legacy data economy obsolete and empower both individuals and regulators to dismantle exploitative surveillance capitalism at its core.

If implemented correctly, this system could also:

- Dramatically reduce healthcare data fragmentation and administrative costs (which in the U.S. are nearly double those of other developed nations)

- Provide a platform to process identity, visa, and other information with near instantaneous speed. 

- Provide a secure, decentralized way to digitally sign content, making it easier to detect and counter deepfake disinformation.

- Enable password-less logins for websites and businesses using decentralized identifiers (DIDs) and zero-knowledge proofs (ZKPs) for secure, privacy-preserving authentication.



## **Policy Proposal**

We propose the development and adoption of a decentralized, encrypted digital identity system rooted in:

- Verifiable Credentials (VCs) issued by trusted institutions (e.g., governments, universities, healthcare providers)

- Zero-Knowledge Proofs (ZKPs) that allow verification of specific facts (e.g., age, citizenship, health status) without revealing full personal information. 

- Encrypted, biometric-secured identity wallets in secure enclaves on users' devices (similar to schemes already offered in Apple Wallet or Google Pay)

- Near-instantaneous, privacy-preserving verification and payments, processed through existing financial infrastructure (e.g., Visa/Mastercard terminals)

- Optional integration of health data from wearables, medical records, and digital health platforms, stored locally and controlled by users. 


----------------------------------------------------------------------------------------

Under this scheme, we would leverage existing secure enclave technologies on smartphones to store digital identity information—credentials traditionally associated with documents like birth certificates, driver’s licenses, and visas.

When accessing a new service, a user’s digital wallet would generate a decentralized identifier (DiD) unique to that service, which is then registered on a public blockchain. When identity verification or login credentials are required, the service initiates a cryptographic handshake. The secure enclave on the user’s device responds with a simple boolean confirmation (“Yes” / “No”), verifying the required attribute without revealing age, identity, or any personally identifiable information (PII).

Rather than storing traditional user profiles, websites and services would maintain non-identifiable user IDs that link to public DiD pairs on the blockchain. Similarly, sensitive healthcare data would be de-identified at the source and linked only to verifiable, pseudonymous DiD keys, drastically reducing the risk of PII leaks or misuse.


## **Implementation Strategy**