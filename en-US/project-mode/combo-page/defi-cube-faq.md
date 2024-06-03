# DeFi Cube FAQ

● Uniswap V3 cubes

### I can't find the token/pool I want

We support import token feature on Uniswap V3 cubes. Simply paste the token address/pool token address onto the search bar.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2024-06-03 at 2.47.53 PM.png" alt=""><figcaption></figcaption></figure>

### What is the slippage set up on Uniswap?

The default slippage is set at 3%.

## ● Aave cubes

### How to use flashloan

We have a thorough tutorial guiding to create a flashloan combo. [Read here](https://medium.com/furucombo/create-flashloan-combo-on-furucombo-c7c3b23267f0)&#x20;

### Why does it say "something's wrong inside the flashloan cubes"?

When you hit send button, Furucombo runs an estimate of your combo in the sequence of your cubes setup. When you see the error message "something's wrong inside the flashloan", that means the transaction will fail when executing cubes inside the flashloan pair.&#x20;

The most common error is that the price has changed in the cubes inside the flashloan pair. Hit the refresh price button in this case.&#x20;

You may also try deleting the flashloan cubes and hit send again to see which cube comes in error.&#x20;

### Why do I have to pay 0.05% fee?

A 0.05% fee is paid for using the flashloan aggregator feature.

### Why can't I put Aave cubes inside flashloan?

This is a limitation setup by Aave. When you use flashloan, you're taking the liquidity from Aave. It doesn't make sense to use the borrowed funds with the borrowed pool right?

### How do I borrow from Aave?

Before borrowing, you need to deposit first any asset which will be used as collateral on Aave. Then, you can use the Aave borrow cube to borrow funds. Select the asset you want to borrow and set the amount you need based on your available deposits used as collateral for the loan.

### **How do I repay my debt on Aave?**

You can simply use the Aave repay cube to repay your debt. Select the asset, set the amount to pay back, and confirm the transaction.

### **What is Aave Borrow (Borrow-Variable)?**

Furucombo supports Aave's Borrow-Variable feature, which is a rate based on the offer and demand in Aave. It'll change depending on market conditions.

## ● Compound cubes

### How do I repay all debt on Compound?

Set a higher repay amount that exceeds debt and Furucombo will exactly repay all debt then return the rest of token to you.

