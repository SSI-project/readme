# portableID

## What is portableID?

portableID is a mobile-first self-sovereign identity platform built for refugees, displaced persons, and underserved populations who lack access to portable, trusted digital identity. It enables people to own, control, and prove their identity without relying on centralized institutions or governments.

The platform combines a secure mobile wallet with a lightweight blockchain parachain to issue, store, verify, and revoke digital credentials—all while keeping personal data private and under user control.

---

## The Problem We're Solving

Millions of people globally lack recognized identity documents, blocking their access to:
- Healthcare and vaccinations
- Education and job opportunities
- Banking and financial services
- Legal recognition and rights

**Why existing systems fail:**
- Centralized registries are fragile and can be destroyed in crises
- They exclude displaced and undocumented people
- They create surveillance vulnerabilities
- Credentials don't work across different countries or service providers
- Offline verification is impossible in low-connectivity areas

portableID solves this by giving people portable credentials they own and control, usable anywhere, without central authorities.

---

## How It Works

### For Users (Refugees & Underserved Populations)

1. **Create a Digital Identity** - Download the portableID mobile app and generate your personal DID (Decentralized Identifier). This is your digital identity that only you control.

2. **Receive Credentials** - Trusted organizations (NGOs, clinics, schools) issue you digital credentials. Examples:
   - Identity verification
   - Medical records (vaccination status, health history)
   - Education certificates
   - Employment records

3. **Store Safely** - Credentials are encrypted and stored on your phone. You control access and recovery.

4. **Share Selectively** - When you need to prove something (e.g., vaccination status to a clinic), you share only what's needed—not your entire identity. The receiving organization sees just the proof, not your personal data.

5. **Work Offline** - Present your credentials via QR code or NFC without internet. Verification happens offline when possible.

### For Organizations (NGOs, Clinics, Schools)

1. **Onboard Easily** - Register as an issuer through a simple web portal. No complex setup required.

2. **Issue Credentials** - Use the issuer dashboard to create and sign credentials for individuals. Define what information you're certifying.

3. **Revoke When Needed** - If a credential becomes invalid (e.g., expired certificate), revoke it instantly. The revocation is tamper-proof and immutable.

4. **Track & Audit** - See a complete audit trail of who received what credentials and when.

5. **Integrate Simply** - Use our SDKs and APIs to connect portableID to your existing systems (clinics' EMR, NGO databases, etc.).

### For Verifiers (Banks, Employers, Services)

1. **Verify Instantly** - Scan a QR code or receive a digital credential presentation.

2. **Check Status** - Verify the credential is genuine, hasn't been revoked, and was issued by a trusted organization.

3. **No Personal Data Needed** - You only see what the user chooses to reveal. No unnecessary data collection.

---

## Key Features

**For Users:**
- Full control over your identity and credentials
- Privacy-preserving sharing—reveal only what you need to
- Works offline using QR codes and NFC
- Secure key recovery without losing access
- No surveillance or tracking

**For Issuers:**
- Fast, frictionless onboarding
- Developer-friendly APIs and SDKs
- Batch operations to reduce costs
- Tamper-proof credential revocation
- Complete audit logs for compliance

**For the Ecosystem:**
- Built on Polkadot blockchain for security and decentralization
- Interoperable with W3C standards for global compatibility
- Minimal personal data stored on-chain (privacy-first design)
- XCM-ready for cross-chain interactions
- Scalable architecture with batched transactions

---

## The Solution Architecture

**Mobile Wallet** - Native app (iOS/Android) where users manage DIDs and credentials. Generates cryptographic proofs of ownership without revealing sensitive data.

**Issuer Portal & Services** - Web platform for NGOs, clinics, and schools to register, issue credentials, and manage revocations.

**Verifier Service** - Lightweight service that checks if a presented credential is valid and hasn't been revoked.

**Identity Parachain** - Custom Polkadot parachain that anchors:
- Issuer registries (who is authorized to issue)
- Revocation commitments (which credentials are valid)
- Public DIDs (so anyone can discover your identity endpoint)

The parachain keeps data minimal—no personal information stored on-chain. Sensitive data stays on users' phones or in private databases.

**Off-Chain Storage** - Non-sensitive artifacts (schemas, audit logs) stored on IPFS or similar for resilience.

---

## Privacy by Design

- **No PII on blockchain** - Personal data never touches the chain. Only cryptographic hashes and issuer metadata.
- **Selective disclosure** - Users choose exactly what to share with each verifier.
- **Pairwise DIDs** - Generate unique identifiers per verifier to prevent cross-service tracking.
- **Hardware security** - Optional support for hardware wallets and biometric protection.
- **Zero-knowledge proofs** - Prove facts (e.g., "I'm over 18") without revealing your birthdate.

---

## Use Cases

**Healthcare Access** - Refugees prove vaccination status to clinics without revealing full medical history.

**Education Verification** - Students prove course completion to employers without sharing transcripts.

**Financial Inclusion** - Undocumented people prove identity to microfinance providers without traditional documents.

**Legal Recognition** - Displaced persons establish identity for property rights, marriage, or asylum claims.

**Employment** - Workers build portable work history that follows them across jobs and countries.

---

## Who We're Building For

**Primary Partners:** NGOs, humanitarian agencies, refugee assistance organizations, mobile clinics

**End Users:** Refugees, displaced persons, undocumented people, underserved citizens in low-connectivity areas

**Secondary Stakeholders:** Local governments, microfinance providers, schools, employers, telecom providers

---

## Why portableID?

- **User-centric** - You own your identity, not governments or corporations
- **Privacy-first** - Minimal data collection, maximum user control
- **Resilient** - Works offline, survives crises, doesn't depend on centralized infrastructure
- **Inclusive** - Designed for people without traditional documents
- **Standards-based** - Built on W3C Verifiable Credentials and Decentralized Identifiers
- **Blockchain-backed** - Immutable, auditable, transparent, and decentralized

portableID empowers the world's most vulnerable populations with the digital identity they need to access services, build opportunities, and claim their rights.

---

## Get Started

For users: Download the portableID app.

For organizations: Visit the issuer portal to register and start issuing credentials.

For developers: Check our SDK documentation to integrate portableID into your application.

---

**Built on Polkadot. Powered by Self-Sovereign Identity. For Everyone.**