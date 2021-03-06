Program Description
DESCRIPTION

Program Rules
Social engineering (e.g. phishing, vishing, smishing) is prohibited.
Please provide detailed reports with reproducible steps. If the report is not detailed enough to reproduce the issue, the issue will not be eligible for a reward.
Submit one vulnerability per report, unless you need to chain vulnerabilities to provide impact.
When duplicates occur, we only award the first report that was received (provided that it can be fully reproduced).
Multiple vulnerabilities caused by one underlying issue will be awarded one bounty.
Amounts below are the minimum and maximum bounties we will pay per bug based on severity. We aim to be fair; all reward amounts are at our discretion.

Rewards
Our rewards are based on the severity of a vulnerability. TrustToken uses CVSS 3.0 (Common Vulnerability Scoring Standard) and the total percentage of potential capital loss to calculate severity. Please note, however, that reward decisions are up to the discretion of TrustToken and reward amounts may be adjusted during the program. 
Scope
Our scopes are listed in the Smart Contracts Scope section below. More information on each scope, including the types of issues we’re most interested in seeing, is available below.


Out of Scope
Clickjacking on pages with no sensitive actions.
Attacks requiring MITM or physical access to a user's device.
Previously known vulnerable libraries without a working Proof of Concept.
Missing best practices in SSL/TLS configuration.
Denial of service that is not a result of application engineering.
Content spoofing and text injection issues without showing an attack vector/without being able to modify HTML/CSS.
Game theory attacks which are noted already in the whitepaper (e.g parasitic markets, malicious resolution source).
Comma Separated Values (CSV) injection without demonstrating a vulnerability.
Vulnerabilities within “Financial Opportunities” are not covered by this program. However, these vulnerabilities may be eligible for review by our team and we encourage them to be submitted without reward for the security of the ecosystem.
 
 
Special Requirements for Critical Smart Contract bugs
Like the rest of the program, the smart contracts program generally uses the OWASP risk rating methodology for classifying bugs. One exception pertains to Critical bugs which must meet the following requirements:

The bug must allow a user to steal collateral tokens representing at least 10% of the value of all TUSD deposited in TrueRewards
The attack must be triggered through an attack vector that is more than just theoretical.
The system must be in normal operational mode or emergency shutdown mode. This excludes for example any states during deployment or shortly after when the system is not fully initialized.

Note: All Smart Contract bugs must include a POC implementation with reproducible steps. This can be the form of a Solidity or JavaScript test or a list of actions that clearly shows how the bug occurs. We recommend using Dapp tools or Truffle for testing

Smart Contracts Scope
At this time, rewards will be paid out for vulnerabilities discovered in our core smart contracts (and their children) for TrustTokens as listed below.

Exploits may be grouped as following:
Function-level (exploitable through a single entry-point)
Contract-level (combining multiple entry-points)
System-level (combining multiple contracts)
Game-level (attacking the incentive mechanisms) (currently not eligible for reward)

Note: Only exploits within groups 1-3 are currently eligible for rewards in this bug bounty program.

The following smart contracts are included in the bug bounty program. There may be redeployments of the contracts during the duration of the bug bounty program. Please see the section below for more information on the current release eligible for bug bounties.

Smart Contracts
[Link mainnet/testnet & github links to source code]
TrueUSD
TrueRewardBackedToken.sol
RewardTokenWithReserve.sol
RewardToken.sol
AssuredFinancialOpportunity.sol
AaveFinancialOpportunity.sol
TrustToken.sol
Liquidator.sol
ALiquidatorUniswap.sol
StakingAsset.sol
AStakingAsset.sol
 
Eligible Release
true-currencies: https://github.com/trusttoken/true-currencies
trusttokens: 

 
What We Are Interested In
This program has been set up to drive TrustToken’s mission forward. Our goal is to make financial freedom as accessible as the internet. TrustToken is here to help our customer’s safeguard their assets, of primary interest to this endeavor, are their:
crypto holdings
sensitive personal data
fiat currency balances
 
The TrustToken Bug Bounty scope covers all software vulnerabilities in the in-scope services (as detailed in the scoping section of this bug bounty) provided by TrustToken. A valid report is any in-scope report that clearly demonstrates a software vulnerability that harms TrustToken or any of TrustToken’s customers and is reproducible (see special requirement).

What We Are MOST Interested In
Given the non-custodial nature of our relationship with our users. These are the most important class of bugs and are of most interest to TrustToken and will be rewarded accordingly:
Any vulnerability that would cause our users to lose their funds or have them rendered frozen and unusable within their wallets or financial opportunities.
Any vulnerability where an attacker can siphon assets from our users in an unintended way.
Vulnerabilities that can drain our RESERVE pool liquidity.
Exploits that use Uniswap pricing to abuse staking & liquidation mechanisms.
 
 


