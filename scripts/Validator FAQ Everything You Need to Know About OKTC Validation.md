# Validator FAQ: Everything You Need to Know About OKTC Validation  

The OKTC blockchain relies on validators to maintain network security and consensus. This comprehensive guide covers essential concepts, responsibilities, and technical requirements for validators and delegators.  

## General Concepts  

### What Is a Validator?  

Validators are crucial participants in the OKTC network, responsible for committing new blocks and maintaining consensus. They broadcast votes signed with cryptographic keys and earn rewards for their work. Validators also participate in governance by voting on proposals, with voting power proportional to their staked OKT.  

Validators must operate full-nodes to ensure transaction validity. While the role requires technical expertise, it offers significant rewards for securing the network.  

### What’s Staking?  

Staking involves locking OKT tokens to secure the network and earn rewards. Validators gain voting power based on staked OKT, which can come from self-delegation or external delegators. To become an active validator, participants must submit a `create-validator` transaction and rank among the top 21 validators by stake.  

### What Is a Full-Node?  

A full-node validates all transactions and blocks, unlike light-nodes that only process headers. Running a full-node ensures network integrity and is mandatory for validators. While resource-intensive, full-nodes can be operated by non-validators to support decentralization.  

👉 [Learn more about OKTC node requirements](https://bit.ly/okx-bonus)  

## Becoming a Validator  

### How to Become a Validator  

To join the validator set, follow these steps:  
1. Generate required keys:  
   - **Tendermint Key**: Signs consensus votes (`okchainvalconspub`).  
   - **Application Key**: Signs transactions (`okchainpub`/`oktc` addresses).  
2. Submit a `create-validator` transaction with:  
   - Validator’s PubKey and address  
   - Moniker (name)  
   - Optional website and description  
3. Accumulate stake: At least 10,000 OKT is required to enter the top 21 validator set.  

Delegators can enhance a validator’s stake, increasing their chances of selection.  

### Validator States Explained  

Validators transition through three states:  
| State | Description |  
|-------|-------------|  
| Bonded | Active validator earning rewards |  
| Jailed | Suspended for misbehavior (e.g., downtime or double-signing) |  
| Unbonded | Inactive; no rewards or slashing risks |  

Jailed validators can recover via an `unjail` transaction if downtime caused the penalty. Double-signing results in permanent removal.  

### Key Management Best Practices  

Validators should use Hardware Security Modules (HSMs) like YubiHSM 2 or Ledger devices to protect private keys. The OKTC team does not endorse specific solutions, encouraging community-driven security improvements.  

## Validator Responsibilities  

### Consensus Participation  

Validators must:  
- Maintain 100% uptime with redundant infrastructure  
- Vote on governance proposals promptly  
- Update software for network upgrades  

Failure to meet these standards risks slashing penalties or removal from the validator set.  

### Governance Involvement  

Validators act as community representatives, voting on proposals for parameter changes, upgrades, and ecosystem decisions. Delegators inherit their validator’s vote if they don’t vote directly.  

### Staking Implications  

Staking requires a 2-week unbonding period to prevent sudden withdrawals during potential misbehavior investigations. Rewards come from block issuance and transaction fees.  

## Technical Requirements  

### Hardware Specifications  

Initially modest, hardware needs will scale with network demand. Key components include:  
- Redundant servers in data centers  
- High-availability firewalls  
- HSM integration for key security  

### Network Infrastructure  

Validators should:  
- Connect only to trusted nodes  
- Implement sentry node architecture to mitigate DDoS attacks  
- Prepare for multi-gigabyte daily bandwidth usage  

### Maintenance and Security  

Regular software updates and security audits are mandatory. Validators must monitor for attacks, maintain network isolation, and respond swiftly to outages.  

👉 [Explore OKTC security best practices](https://bit.ly/okx-bonus)  

## Frequently Asked Questions  

### **What happens if a validator goes offline?**  
Temporary downtime results in missed rewards. Prolonged unavailability leads to jail time and potential removal from the validator set.  

### **Can delegators lose funds?**  
Delegators share slashing risks with validators. However, validators cannot directly access delegated funds.  

### **How often do validators propose blocks?**  
Proposer selection is proportional to stake. A validator with 10% of total bonded OKT proposes ~10% of blocks.  

### **Is validator anonymity allowed?**  
Yes, though transparency builds trust. Validators can register websites to showcase their team and track record.  

### **What’s the minimum stake requirement?**  
The threshold is 10,000 OKT to enter the active validator set.  

## Conclusion  

Becoming an OKTC validator requires technical expertise, operational diligence, and a commitment to network security. By understanding the responsibilities and technical demands, validators contribute to a robust, decentralized ecosystem while earning rewards.  

👉 [Start your validator journey today](https://bit.ly/okx-bonus)  

This guide provides actionable insights for aspiring validators and delegators. Stay updated with OKTC’s evolving protocols to maximize participation and security.