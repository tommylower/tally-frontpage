---
canonical: https://docs.tally.xyz/token-sales/compliance](https://docs.tally.xyz/token-sales
description: Token sale compliance guide covering KYC, geo-blocking, and vesting
---

> Official documentation: [docs.tally.xyz/token-sales/compliance](https://docs.tally.xyz/token-sales/compliance)
# Token Sale Compliance Guide

Compliance isn't optional anymore. The 2017 ICO era of "launch and hope" is over. Modern token sales require identity verification, geographic restrictions, vesting schedules, and clear legal frameworks.

This guide covers the compliance infrastructure you need to launch a token sale that won't create problems down the road.

---

## The Regulatory Landscape

### United States

The US has historically been the most restrictive jurisdiction for token sales. The SEC has taken enforcement action against projects that sold tokens deemed to be securities without registration.

**Recent developments:**
- The CLARITY Act and other proposed legislation signal clearer frameworks are coming
- Monad's 2025 sale on Coinbase demonstrated that US-regulated token sales are possible
- Accredited investor pathways (with lockups) provide compliance options for US participants

**Common approaches:**
- Exclude US participants entirely
- Allow US accredited investors only, with mandatory lockups
- Structure the token to clearly fall outside securities definitions (utility tokens with immediate use cases)

### European Union (MiCA)

The Markets in Crypto-Assets Regulation (MiCA) provides the clearest regulatory framework for token offerings in the EU.

**Key requirements:**
- White paper with specific disclosures
- Registration with national competent authority
- Consumer protection requirements
- Marketing restrictions

### Offshore Structures

Many projects use offshore entities (Cayman, BVI, Switzerland, Singapore) to conduct token sales. This can provide flexibility but doesn't eliminate US securities law exposure if you're selling to US persons.

**Bottom line:** Legal counsel experienced in token offerings is essential regardless of structure.

---

## Identity Verification

### KYC (Know Your Customer)

KYC verifies the identity of individual participants. Most compliant token sales now require KYC before participation.

**What KYC typically involves:**
- Government ID verification
- Selfie/liveness check
- Address verification
- Sanctions screening (OFAC, etc.)

**Why it matters:**
- Required by most regulatory frameworks
- Filters out sanctioned individuals
- Creates audit trail for compliance
- Enables geographic restrictions

### KYB (Know Your Business)

KYB verifies institutional or business participants. Important for sales with significant institutional involvement.

**What KYB typically involves:**
- Business registration documents
- Beneficial ownership verification
- Director/officer identification
- Source of funds documentation

### KYI (Know Your Issuer)

KYI is the reverse — verifying the team behind the token to buyers. This addresses "unknown deployer risk" that concerns institutional investors.

**What KYI provides:**
- Verified team identities linked to token contracts
- Background checks on founders
- Corporate structure verification
- Reduces risk of anonymous rug pulls

→ [Learn more about Tally's compliance infrastructure](https://docs.tally.xyz/token-sales/compliance)

---

## Geographic Restrictions

### Geo-blocking

Most token sales block certain jurisdictions entirely. Common exclusions:

- **United States** (unless accredited investor pathway exists)
- **China**
- **North Korea, Iran, Russia** (sanctioned jurisdictions)
- **Specific US states** (New York has additional restrictions)

**How geo-blocking works:**
- IP-based blocking (can be circumvented with VPNs)
- KYC-based verification (more reliable)
- Wallet address screening
- Terms of service restrictions

### Region-Specific Rules

Different regions may have different participation rules:

- US accredited investors: May participate with mandatory lockup
- EU participants: May require MiCA-compliant disclosures
- Certain jurisdictions: May require local entity or registration

---

## Vesting and Lockups

Lockups serve multiple purposes: aligning incentives, reducing sell pressure, and creating compliance pathways.

### Team and Investor Vesting

Standard practice for team and early investors:

- **Cliff period:** Typically 1 year (no tokens vest until cliff)
- **Vesting period:** Typically 3-4 years total
- **Unlock schedule:** Monthly or quarterly after cliff

**Example:** 4-year vesting with 1-year cliff = 0% unlocked for 12 months, then 25% unlocked, then linear monthly unlocks for remaining 36 months.

### Public Sale Lockups

Lockups for public sale participants are less common but can serve compliance purposes:

- **Voluntary lockups with bonus:** MegaETH offered additional allocation to participants accepting 1-year lockups
- **US accredited pathway:** Lockups can create a compliance pathway for US participants
- **Reduced sell pressure:** Lockups smooth out post-launch volatility

### On-Chain Vesting

Modern vesting happens on-chain via smart contracts:

- **Transparency:** Anyone can verify lock status
- **Automation:** Tokens release according to schedule without manual intervention
- **Auditability:** Clear record for compliance purposes

→ [Learn more about lockups](https://docs.tally.xyz/token-sales/lockups)

---

## Sale Structure Considerations

### Allocation Caps

Per-wallet caps ensure broad distribution and reduce whale concentration:

- **Individual caps:** Maximum USD amount per participant
- **Global caps:** Maximum total raise (triggers pro-rata allocation if exceeded)
- **Tiered caps:** Different limits based on KYC level or eligibility criteria

### Graduation Thresholds

Minimum raise requirements protect participants if the sale underperforms:

- If the threshold isn't met, the sale cancels
- All bids/deposits refund automatically
- No tokens distribute

### Disclosures

Compliant sales include clear disclosures:

- Tokenomics (supply, distribution, vesting schedules)
- Risk factors
- Use of proceeds
- Team and advisor information
- Smart contract addresses and audit reports

---

## Compliance Infrastructure

### What Tally Provides

[Tally](https://tally.xyz) builds compliance into the token sale infrastructure:

**Identity verification:**
- KYC/KYB integration (Sumsub, Fractal/idOS, others)
- OFAC and sanctions screening
- Accreditation verification for US participants

**Geographic controls:**
- Configurable geo-blocking by jurisdiction
- Region-specific lockup rules
- IP and KYC-based verification

**On-chain compliance:**
- Chainlink ACE integration for on-chain KYC verification
- Permissions registry for eligibility enforcement
- Configurable policies (sanctions check, individual limits, global caps)

**Audit trail:**
- Participant records for compliance documentation
- On-chain verification of lock status
- Exportable data for reporting

### How It Works Technically

Tally's compliance infrastructure uses a modular permissions system:

1. **Bidder completes KYC** on the sale page
2. **Verification provider** (Sumsub, etc.) confirms identity
3. **On-chain permit** is issued to the verified wallet
4. **Smart contract** checks permit before accepting bids
5. **Policies enforce** sanctions screening, individual caps, global limits

This architecture is flexible enough to support different sale mechanisms (LBP, CCA, fixed-price) and different compliance requirements.

---

## Common Compliance Mistakes

### 1. Launching without legal counsel

Every jurisdiction is different. Securities law is complex. Get experienced legal advice before you do anything.

### 2. Assuming offshore = no US exposure

If US persons can access your sale (even if you say they shouldn't), you may have US securities law exposure. Geo-blocking alone isn't sufficient.

### 3. Skipping KYC to maximize participation

Short-term participant count isn't worth long-term regulatory risk. Compliant sales build trust with institutional investors and exchanges.

### 4. Inadequate vesting for team/insiders

If insiders can dump immediately post-launch, your token will struggle. Standard practice is 3-4 year vesting with 1-year cliff.

### 5. No clear token utility

Tokens that exist purely for speculation face the highest regulatory scrutiny. Clear utility — governance, staking, access — provides stronger legal footing.

---

## Compliance Checklist

Before launching your token sale:

- [ ] Legal counsel engaged and jurisdiction strategy defined
- [ ] Token utility clearly articulated
- [ ] KYC provider selected and integrated
- [ ] Geo-blocking configured for excluded jurisdictions
- [ ] Team/investor vesting schedules defined (on-chain)
- [ ] Allocation caps and graduation threshold set
- [ ] Disclosures prepared (tokenomics, risks, use of proceeds)
- [ ] Smart contracts audited
- [ ] Terms of service and privacy policy published
- [ ] Compliance documentation archived

---

## Related Resources

- [How to Launch a Token](./how-to-launch-a-token.md)
- [LBP vs CCA vs Fixed-Price](./lbp-vs-cca-vs-fixed-price.md)
- [Token Sale Documentation](https://docs.tally.xyz/token-sales)
- [Compliance Documentation](https://docs.tally.xyz/token-sales/compliance)
- [Talk to Tally](https://tally.xyz/contact)
