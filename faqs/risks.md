# Risks

Taking out a loan, no matter whether it is in DeFi (Decentralized Finance) or from a bank, involves risk. At Ambos, we want to be as transparent as possible, and provide you with the full information required to know if taking an Ambos loan is right for you.

The below is a list of the main risk factors to consider when taking out an Ambos loan, along with mitigations we have put in place.

### Smart Contract Risk

Unique to DeFi, smart contract risk reflects the fact that bugs in smart contract code may lead to a loss of funds, either from a hack or a logical error.

**Mitigations:**

* Under the hood, Ambos uses the Aave protocol for lending. Aave has several billion USD in value secured in its platform, and is considered best-in-class for lending security in DeFi.&#x20;
* Ambos also works with other partners, such as Biconomy, for handling smart wallets. Such partners have audited contracts that have been verified for key risks by independent security assessments.

### Liquidation Risk

When you deposit into Ambos, your ETH has a certain value in USD, and you borrow USD against it.

If the value of ETH falls sufficiently, you are at risk of having at least some of your deposited ETH _liquidated_ to ensure that lenders of the USD can be repaid.&#x20;

**The exact numbers can be seen on the Ambos app** but typically a liquidation occurs when _the value of your loan + interest is greater than 80% of the value of your ETH._

**For example:**

* 1 ETH is worth $1000 on January 1st
* Alice deposits 10 ETH into Ambos, worth $10,000
* Alice borrows $5,000 (including Ambos chargess) at 5% interest
* In 1 year, Alice's debt is $5,250 (including interest)
* $5,250 is 80% of $6,562.50 -> **this is the minimum value of Alice's collateral required to avoid liquidation**
* If ETH holds it value, or increases, Alice is safe
* If ETH falls in value:
  * To $900/ETH -> Alice is safe
  * To $800/ETH -> Alice is safe
  * ...
  * To $657 -> Alice is right on the risk threshold
  * To $656 -> Alice is at risk of a liquidation event

If Alice is then liquidated, 50% of her ETH will be sold to offset her loan, and her debt will be reduced accordingly. If ETH falls too far, Alice may lose 100% of her ETH.

At this point, however, her debt is fully repaid, she does not have to repay the loan.

**Mitigations:**

* Ambos by default places limits on borrowing at 50% of the value of deposited capital (not including fees), this is a protection to ensure users don't take out excessively risky loans.

### Stablecoin Depeg Risk

In Ambos, loans are denominated in Stablecoins. These are coins that expect to maintain a rough 1:1 peg with a fiat currency (typically the US Dollar). Generally speaking, stablecoins are backed by assets (either crypto or treasuries) at least 1:1, to keep the value of them secured.

There are notable cases, however, where stablecoins have deviated from their peg, and either trade significantly above or below 1:1 value.&#x20;

* In the case that a stablecoin depegs downwards, a user's debt, in USD terms will also be reduced. For example, if 1 USDC is now worth $0.70, your Ambos debt will be reduced by 30% in dollar value.
* In the case that a stablecoin depegs upwards, the opposite is true. So if 1 USDC is worth $1.10, the value of your debt will increase by 10%.
* These changes are not permanent, if the peg returns to $1.00, your debt is back to $1.00&#x20;

**Mitigations**

_All examples below assume a USD stablecoin_

* Ambos uses industry standard stablecoins such as USDC, which have been used for hundreds of billions of dollars in transactions safely. However it should be noted, that USDC has had periods of depegs in its history, and users should be aware and comfortable with such risks.

### Risk of Losing Access/Compromised Accounts

Ambos is a non-custodial solution. This means that if you lose access to the account with which you take out the loan, there are limited options for us to help you (conversely though, this means we cannot steal your funds). If your account is lost, or compromised to an attacker, this may result in your funds being lost.

**Mitigations:**

* Ambos uses login methods such as Google OAuth, or AppleID, that secure billions of devices worldwide. This means you do not have to worry about managing a private key or seed phrase, as with other wallets.
* Nonetheless, be careful when using the Ambos app that it was downloaded from the real Ambos domain (app.ambos.finance)

## Further Reading

See the Aave docs: [https://docs.aave.com/faq/liquidations](../)

&#x20;
