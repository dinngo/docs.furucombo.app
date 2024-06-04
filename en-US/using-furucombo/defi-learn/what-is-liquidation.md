---
description: What does liquidation mean, and how can you avoid getting rekt?
---

# What Is Liquidation

![](<../../.gitbook/assets/G Copy.png>)

Liquidation occurs when an investor cannot meet the margin requirement for their leveraged position & the underlying collateral tokens will be converted to pay for the liquidation.

## Liquidation vs Forced liquidation <a href="#id-1cc2" id="id-1cc2"></a>

#### **Liquidation:**

Means selling collateral for cash, or its equivalents.

#### **Forced liquidation:**

Occurs when a trader’s position is closed forcibly by lending protocols as the trader ran out of the initial margin used to open the position.

## What causes a forced liquidation? <a href="#id-0ce9" id="id-0ce9"></a>

When the price begins to move against the trader’s expectation (either long or short position), the losses are paid for from the margin provided. If the losses surpass the margin provided, the position gets liquidated.

## How to avoid getting liquidated? <a href="#id-966f" id="id-966f"></a>

1️⃣ Know the liquidation rules before you open a position.

2️⃣ Raise your collateral ratio by depositing more collateral or repaying part of your loan. It’s important to monitor your collateral ratio & keep it high enough to avoid liquidation.

3️⃣ Don’t leverage too much.\
Leveraged positions are prone to volatile price swings, which may cause a trader’s investment to plunge into a negative balance in a very short time period. Measure how much risk can you afford to take before you open a position.

### Know how to self-liquidate! <a href="#id-53f8" id="id-53f8"></a>

4️⃣ Self-liquidation means you repay the loan with the fund generated from the sale of the collateral, and you’ll get the remaining assets at the end of the trading.

### How does self-liquidation work? <a href="#id-0de6" id="id-0de6"></a>

(using Aave flashloan as an upfront fund)

a) Flashloan fund to repay all debt\
b) Withdraw all collateral\
c) Sell collateral to repay flashloan
