---
description: 'Tutorial: Instantly Swap cTokens on Compound'
---

# Instantly Swap cTokens on Compound

![Tutorial | Instantly Swap cTokens](https://miro.medium.com/max/3200/1\*xFGjLBVNOh7TN0p7aTj1Hw.png)

Passive income is the money that you earn in a way that requires little to no effort. In the DeFi world, the easiest way to earn passive income is by supplying/depositing an asset to lending protocols to earn interests in return.

In our previous article, [Passive income combo](https://docs.furucombo.app/using-furucombo/tutorials/passive-income-part1), we introduced you what interest-bearing tokens are and how to get some of them to earn passive income. In this article, we will walk you through further how to swap between [Compound](https://compound.finance/) cTokens to get higher APY in return.

![Compound dashboard](https://miro.medium.com/max/5760/1\*JM8PtcHBI7W3Vnf5P5NpIQ.png)

## How to swap between cTokens? <a href="#id-4c47" id="id-4c47"></a>

There are three ways to swap cTokens. Two of them are for users who don’t have debt on Compound and one for those who do.

### No-debt cToken swapping <a href="#e9f2" id="e9f2"></a>

If you don’t have any debt on Compound and want to swap your cTokens to another cTokens to get higher APY, there are two approaches you can put into practice:

* Basic level: Build combo manually
* Pro level: Instant swap panel. Skip building. Just use Furucombo’s latest feature on the [Learn](https://furucombo.app/explore/combo\_compound\_00001)[ page](https://furucombo.app/explore/combo\_compound\_00001).

### 1) **Basic level:** Build combo manually <a href="#id-6750" id="id-6750"></a>

```
Step 1: Withdraw cToken A from Compound
Step 2: Swap Token A to Token B
Step 3: Supply Token B to Compound and get cToken B
```

![Basic level: Use Furucombo‘s combo to swap cTokens](https://miro.medium.com/max/5760/1\*U5SfOrJosbewoviDQtBd9g.png)

### cToken swapping with debts… <a href="#id-2aa1" id="id-2aa1"></a>

If you have debts on Compound and you want to swap your cTokens from one to another, well… it’s a bit complicated. Get ready to wrap your head around or you may jump to the end of the story → use our [pre-built Compound Collateral Swap Combo](https://furucombo.app/combo/bti7tdi6bifc72uvqpeg?refreshPrice=1) to execute the swapping.

### 2) God Level: [Compound Collateral Swap](https://furucombo.app/combo/bti7tdi6bifc72uvqpeg?refreshPrice=1) <a href="#id-5107" id="id-5107"></a>

You may wonder, why can’t you use the previous swap cToken combo to do the same? The answer is because you have debts on Compound. Your cTokens are, therefore, collaterals, and they are locked until a) your debts are paid or b) you supply more funds to increase the collateralization ratio. The strategy below takes b option. We use flashloan to double your supply volume first and withdraw original collateral to pay back the flashloan. In this case, no upfront funds are needed.

![Compound Collateral Swap](https://miro.medium.com/max/5804/1\*vQA2KaaFdfsOSkbU-op68w.png)

When using this combo set, you may notice two cubes that you don’t see often, _**“Return Funds**_**”** and _**“Add Funds**_**”**. They are there for a reason so please, don’t delete them.

> “Return Funds” cube means moving funds from Furucombo’s proxy contract to user’s wallet. And conversely, “Add Funds” cube means moving funds from user’s wallet to Furucombo’s proxy contract.

In the example here, after you supply USDC to Compound, the cUSDC is on Furucombo’s proxy contract. You need to use the “Return Funds” cube to transfer cUSDC to your wallet so that your supply position can be doubled. Then, because your cBAT is locked in your wallet until you increase your supply position, you need to use the “Add Funds” cube to send cBAT to Furucombo’s proxy contract right after receiving the cUSDC.

Doesn’t it sound like everything is reversed? Because it is. You receive the target cToken first and you send your original cToken later to swap.

```
You hold cBAT and you want to swap them to cUSDC:
Step 1: Flashloan borrow USDC
Step 2: Supply USDC and get cUSDC
Step 3: Return cUSDC to your wallet
Step 4: Send cBAT to Furucombo
Step 5: Withdraw cBAT to BAT 
Step 6: Swap BAT to USDC
Step 7: Repay USDC to flashloan with fee
```

If you have read all the way through here, you’re officially a combo master. Found which way suits you the best?

* Basic level: [Build combo manually](https://furucombo.app/combo)
* God Level: [Compound Collateral Swap](https://furucombo.app/combo/bti7tdi6bifc72uvqpeg?refreshPrice=1)

_🎉 Bravo! You’ve swapped your cTokens. Don’t forget to share your result on Twitter. 🎉_

![](<../../.gitbook/assets/1\_rqJS5Y9tPGUFZxCzib5qbg (3).gif>)
