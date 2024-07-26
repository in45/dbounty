# DBounty

## Overview
DBounty is a blockchain-based bug bounty platform deployed on Ethereum. It connects organizations needing cybersecurity with a community of vulnerability researchers. The platform offers a sustainable vulnerability prevention system that rewards researchers for discovering vulnerabilities in a bug bounty program. Rewards are based on various factors such as severity and potential impact.

## Features
- **Blockchain Integration:** Ensures transparency and integrity of data.
- **Zero-Knowledge Proofs (ZKP):** Validate report authenticity without revealing sensitive details.
- **Real-Time Communication:** Facilitated by WebSocket for immediate interaction.
- **Reputation System:** Motivates researchers and maintains quality.

## Demo Video
Watch the [demo video](https://drive.google.com/file/d/1Mjv1wyezJLD5-SLrYFihwhNxiS5xQNa3/view?usp=drive_link).

## Repositories
DBounty is divided into several repositories, each handling a different aspect of the platform:

1. [Admin Frontend](https://github.com/in45/dbounty-front-admin)
2. [Admin Backend](https://github.com/in45/dbounty-back-admin)
3. [User Frontend](https://github.com/in45/dbounty-front-user)
4. [User Backend](https://github.com/in45/dbounty-back-user)
5. [Manager Frontend](https://github.com/in45/dbounty-front-manager)
6. [Manager Backend](https://github.com/in45/dbounty-back-manager)
7. [Node.js Communication Service](https://github.com/in45/dbounty-nodejs)

## Roles and Responsibilities
- **Admin:** Manages the entire platform and oversees all actions.
- **Company Manager:** Manages company programs and researcher reports.
- **Bounty Hunter:** Submits reports and communicates with managers for rewards.

## Tools and Technologies
- **Backend:** Laravel,NodeJS
- **Frontend:** Vue.js
- **Database:** MySQL
- **Blockchain Development:** Ganache, Web3.js, MetaMask

## Authentication
- **Admin and Manager:** JWT with RSA Algorithm.
- **User:** MetaMask for authentication.

## Real-Time Communication
- **Protocol:** WebSocket for real-time updates and communication.

## Email System
- **Framework:** Laravel's Mailable class for email functionality.

## Roles
### Administrator
- **sudo:** Full permissions
- **Owner:** Owner of smart contracts
- **Sysmanage:** Manages reports
- **Sysmoni:** Monitors the system

### Company Manager
- **SysAlpha:** Can reward submissions
- **Sysbeta:** Can view and modify submissions

### Bounty Hunter
- Submit and manage bug reports
- Communicate with company managers

## Report States
- **Saved:** Preliminary save before final submission
- **Pre-submission:** Initial review by a security analyst
- **New:** Unread report
- **Pending:** Awaiting program review
- **Triaged:** Evaluated but unresolved
- **Needs more info:** Additional information required
- **Informative:** Contains useful info but not critical
- **Not applicable:** No valid issue found
- **Accepted:** Report accepted by the manager
- **Resolved:** Report validated and issue resolved
- **Duplicate:** Issue already reported

## Vulnerability Scoring
- **System:** Common Vulnerability Scoring System (CVSS) for calculating report severity.

## Smart Contracts
- **AdminContract:** Manages administrators.
- **CreateHTTContract:** Creates the ERC20 token (HTT).
- **DBountyContract:** Manages payments and ZKP implementation.

## Scoring and Reputation System
Reputation points are awarded based on the validity and severity of reports. Maintaining a good reputation grants privileges like invitations to private bug bounty programs.

### Reputation Points
- **Informative:** No change
- **Duplicate (Low):** +2
- **Duplicate (Medium):** +5
- **Duplicate (High):** +8
- **Duplicate (Critical):** +10
- **Not Applicable:** -5
- **Accepted (Low):** +5
- **Accepted (Medium):** +10
- **Accepted (High):** +20
- **Accepted (Critical):** +40

## License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

---

For detailed documentation on each module, please refer to the respective repository.

---

## Contact
For any inquiries, please reach out to [INAS HASNAOUI](mailto:inashasnaoui1802@gmail.com).

