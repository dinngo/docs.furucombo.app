# Leveraged Short Position Tutorial

<figure><img src="../../.gitbook/assets/Tutorial Position Management 1.png" alt="Leverage Short on Furucombo"><figcaption><p>Leverage Short on Furucombo</p></figcaption></figure>

This tutorial will help you to create a leveraged short position on [Furucombo](https://furucombo.app/). This combination will allow you to increase your leveraged position on a lending protocol, such as Aave, to increase your short position on the market. If you are more of a visual learner, you can use our [video tutorial for short positions](https://www.youtube.com/watch?v=HdBJuUtO0\_o) instead.

{% embed url="https://youtu.be/HdBJuUtO0_o" %}
Aave Leverage Short Position
{% endembed %}

## How to Create a Leveraged Short Position?

A leveraged short position can be created by borrowing an asset you wish to go short on (an asset you expect to decrease in value), and swapping that to a stable coin. For example, if you deposit $1000 in USDC (a stable token), you can borrow $800 in ETH and swap that ETH to USDC therefore creating a $1800USDC position from $800 in borrowed ETH. If the value of ETH goes down, you’ll have more stable coins to buy ETH with to pay back your debts, and therefore have created a leveraged short position. Always be aware that leveraged positions are subject to liquidation risk if the collateral falls below the loan-to-value ratio of the amount borrowed. The risk in this case would come from an increase in the value of the borrowed ETH.

## Steps to set up a New Leveraged Short Position:

1. Connect your wallet, and select the network of your choice on the top right of [create mode on Furucombo](https://furucombo.app/combo). Once connected, click the cube icon in the center of the page to get started. The first step is to make a position on Aave using a stable coin. Once you’ve decided which stable coin to use, simply add the ‘Deposit’ cube under Aave, and make a deposit in the asset you wish to use as collateral. In this example we will use USDC.

<figure><img src="https://lh3.googleusercontent.com/GstmFbCMDDRvZIL24OxuQ4E2rWCLEHcWMt-X-iDEuCBNpEqJyTheokFIDjvR70c0RM7uKv1fOzTejIB5_AlI_RejS7Ag3PP47J5c0APd7_kbhu5LJLmIoYQtl0GywOozdV21vtQf--LjCdlULcUSozo" alt="Make a position on Aave using a stable coin"><figcaption><p>Make a position on Aave using a stable coin</p></figcaption></figure>

2. Next we will use a ‘Return Funds’ cube to add the aToken to the contract in order to borrow an asset in one transaction. In this example, we will add the aUSDC token in our return funds cube. If you deposit a different asset, simply carry over the aToken and the amount into the return funds cube.

<figure><img src="https://lh3.googleusercontent.com/ZhlJxF-U0-7yngqDTM7axiC8gyFO5GFV-VbisvFJTUuHOi263W4F9t-CXc3w6l-kfkXMyoGXatsa9Xe_1S5HQyvX-NMBtarg_OVHwc1RSQUvsRj47tGBkAgg7v2Buhx3dvFFPft567zICX0yJqssVrQ" alt="Return Funds"><figcaption><p>Return Funds</p></figcaption></figure>

3. Now we can borrow a token we wish to go short on from Aave. You can choose any token available from Aave. If you decide for example to short ETH, then borrow ETH. At the time of writing, ETH is worth approximately $1750, so we will borrow 75% of our LTV, therefore we will borrow $750 worth of ETH, or 0.4285.

<figure><img src="https://lh3.googleusercontent.com/eHiq7AX_PshrARyrctaPURUYa0jhqhwqeBGYvC9ml2PPus6oowaoJnBtkeukZyiuVM3a-HGrlywe1FyvAKoA2u6EOIJ9ZpG13A5x2KMekJGh4mr2wsEK62gaFFYRuoJOMWVmsqU_Ub3E_DnuWCoYWv0" alt="Borrow a token from Aave"><figcaption><p>Borrow a token from Aave</p></figcaption></figure>

4. Next we will swap the borrowed ETH to USDC to short the ETH asset. This is because if ETH goes down in value, then it takes less USDC to buy the asset back to repay the debt.

<figure><img src="https://lh5.googleusercontent.com/ZgP_hJ5xFa8R6zpl4Ew0sZTpVYRN3bYpgX4NJE5oKVZXmyVCl361SrmDWsHuwl-oCCkISID-8sEhKOv1cBtxqtq7ae0nTLcr4btMoHx6DfC19t-KSw8A1uQ4gVg8aK1mkoQ4OyxcPyybT2XJ08kOf2s" alt="Swap the borrowed ETH to USDC"><figcaption><p>Swap the borrowed ETH to USDC</p></figcaption></figure>

5. Once you are happy with the numbers, you can hit ‘approve’ & ‘send’ at the bottom of the page. You have now created a leveraged position using Furucombo.

In the above example, we have made a deposit of 1000USDC, borrowed ETH, and swapped that to USDC, creating a position of 1751USDC from a deposit of 1000USDC. This means the leverage created in this example is 1.751x, or 175.1%. This means that any 1% decrease in Ethereum, will equal a 1.751% increase in value for the leveraged user. This is a powerful way to get additional exposure to the market. Also be aware of the risks of liquidation. If the value of the debt decreases, you may be subject to liquidation risk. For example, if Ethereum increases in value, the collateralization ratio will decrease, putting the user at risk of liquidation. If that risk occurs, you can add more collateral, or perform our de-leverage strategy to reduce your market risk.

## Steps to Adjust your Leveraged Position with a Flash Loan

You can also use the flash loan feature to add a collateral position, and borrow an asset with that collateral to increase your exposure to the market. For example, if you have $1000 in collateral on Aave, and you’ve borrowed $600, or have a debt ratio of 60%, you can use a flash loan to increase your collateral position, and use some of the extra debt you can still incur to pay back the flash loan. Using the aforementioned numbers, let’s assume you want to increase your position by $1000. Assuming an ETH price of $1750, to increase the position by $1000, we need to borrow $800 (as we will borrow the other $200 from Aave in order to make up the difference) in the form of a flash loan.

1. Insert a ‘Flashloan’ cube in the amount you wish to increase your exposure by. Based on the above example, we will take a flash loan for 800USDC

<figure><img src="https://lh6.googleusercontent.com/p0xzyubQ7pRD7g3_EoMWh-xQE0j7eXLYqTZPe1_F5PNBQkD30svAor0Opda4wWtMx-uKtPELsD3JuHXWnuYRCvsDoeJHH7MWyIeVi3y9GIFvzgGj-_i_8v0Ju1wczI1rUuj02PUsSGH9iSOEkjlBxSo" alt="Flashloan a Fund"><figcaption><p>Flashloan a Fund</p></figcaption></figure>

2. Next we will perform the same steps as mentioned above. Simply add the ‘Deposit’ cube under Aave, and make a deposit in the asset you wish to use as collateral, in this case we are using USDC. Ensure the cubes are above the bottom flash loan cube.

<figure><img src="https://lh6.googleusercontent.com/iwrhNC9RpcihuaQm4thb9Kl78FHkRSPvYfh7SoiBZc5_xk-dY0vwLdwpHoGWU9OhvznhQdyj_lr-Vn2QyvBK1EzzHp9x7EQgmTW2Jr5inkUsSWqkFXoHQYjFufy94_iHz1V6ORYhGWIQME38menDupw" alt="Deposit on Aave"><figcaption><p>Deposit on Aave</p></figcaption></figure>

3. Now we will use a ‘Return Funds’ cube to add the aToken to the contract in order to borrow an asset in one transaction. In this example, we will add the aUSDC token in our return funds cube. If you deposit a different asset, simply carry over the aToken and the amount into the return funds cube.

<figure><img src="https://lh4.googleusercontent.com/KTcnLaaI6qfJacaUJPqZBTYBQt7qkIl6RaOoHnU3lGVGcEKblOUqpR2zNWHVRb_UNjoYmxXqkw2f0HP07cNcoue1YfusVMur9X5edazESD7pYd5igtffIz7rYKAlHe02ie7AT2kqqyIWKtTnuCuX0xM" alt="Return Funds"><figcaption><p>Return Funds</p></figcaption></figure>

4. Now we can borrow a debt token from Aave. In keeping with the previous example, we will borrow ETH. You can choose any token that's available on the lending protocol of your choice. Because we made a flash loan deposit of $800 in value, we can borrow up to approximately 80% of the value of that, which would be $640. The other value will be made up from the extra debt we can take on from Aave, which will increase our loan-to-value ratio (thus increasing our liquidation risk, or our leverage to the market). In this example, we will borrow at least enough to pay back the flash loan. So we will borrow $850 worth of ETH, or 0.485, but how much you borrow will depend on your risk tolerance, collateralization ratio, etc.

<figure><img src="https://lh3.googleusercontent.com/yslH8bbw-DPMASPZPXk511WcqDwN9QLz4yZh-NriErQGQOtphny_gQAUHF7mewxMjmDdym7gss1NPRHLGZIIhNaIK73CQEfhDZVJSdc3_6R1eXxhKfXznC3UdE2Hhr9_9j8EO8wAgNnViJbqIiNMdJE" alt="Borrow a debt token from Aave"><figcaption><p>Borrow a debt token from Aave</p></figcaption></figure>

5. Next we will swap the borrowed ETH to USDC to short the ETH asset. This is because if ETH goes down in value, then it takes less USDC to buy the asset back to repay the debt.

<figure><img src="https://lh4.googleusercontent.com/Wa01u-tWKZg9scMe1BMIAvb-ewGg6sHLGaZGFo5vY2Ghyk4bRwYXtpsrCU7kFABYYgunBvz6AP30DSCodfCtRjFF9WNZcjrsDjSOu6wuc5W0Htbm1vNAp77lcZkpS3EsoXhZsWpk7tZ6n36d3VFCT-I" alt=""><figcaption><p>Swap the borrowed ETH to USDC to short the ETH asset</p></figcaption></figure>

6. Once you are happy with the numbers, you can hit ‘approve’ & ‘send’ at the bottom of the page. You have now adjusted your leveraged position with a flash loan using Furucombo.

\


To learn more about our other position management features, click the following tutorials:

1. [Leveraged Long Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-long-position-tutorial)
2. [Collateral Swap](https://docs.furucombo.app/using-furucombo/tutorials/collateral-swap-tutorial)
3. [Debt Swap](https://docs.furucombo.app/using-furucombo/tutorials/debt-swap-tutorial)
4. [De-Leverage Position](https://docs.furucombo.app/using-furucombo/tutorials/de-leverage-position-tutorial)
