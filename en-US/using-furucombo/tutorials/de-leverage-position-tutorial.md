# De-Leverage Position Tutorial

<figure><img src="https://lh5.googleusercontent.com/4xV6kaVZiuOBnMPY1xMW0Mkv7pTktvPe8XV8NDOaC2TVCPmAhTEV4jAr_dpuIVgAHh_aRpgMYwVx-0-EoiMF5i8RDj_23Jr-dciCcUqyfzpqsxw4kvGsJQ03-_C-lwsooAdw_XgKXKUV3IJ-LVgLZxY" alt=""><figcaption></figcaption></figure>

This tutorial will help you to create a de-leveraged position on [Furucombo](https://furucombo.app/). This combination will allow you to withdraw your position from a lending protocol, such as Aave, without any upfront funds. This is because it uses your collateral position, which is higher than your debt, to repay the debt and take the remaining principal. If you are more of a visual learner, you can use our [video tutorial](https://www.youtube.com/watch?v=y7S-QwD81rE) instead.

## What is Leveraging and De-Leveraging?

Aave allows a user to borrow some funds from their collateral position. This means if you make a deposit on Aave, you’ll earn interest on your deposit, as well as open the possibility to borrow from your collateral. This is based on the loan-to-value ratio determined by the protocol. You can borrow up to some percentage of your collateral position depending on the asset deposited. To learn more about the borrow ratios, visit the [risk parameters page](https://docs.aave.com/risk/asset-risk/price-discovery) on Aave and select the network that pertains to you.

Leveraging allows you to borrow an asset, and swap that to the collateral asset to leverage your position. For example, if a user deposits ETH, and borrows USDC, and swaps that USDC to ETH, they’ve now created a leveraged position. De-leveraging allows you to adjust your position to reduce your debts, or your exposure to leverage on the market.

### When to Use a De-Leverage Strategy?

You can use a de-leverage strategy when you wish to reduce your risk to the market, or to reduce your liquidation risk.

### What is the Advantage of a De-Leverage Strategy?

The advantage of the de-leverage strategy is that it doesn’t require any upfront funds to execute, and allows you to take advantage of the benefits listed above.

## Steps to set up a De-Leverage combination:

1. Connect your wallet and select the network of your choice on the top right of [create mode on Furucombo](https://furucombo.app/combo). Once connected, click the cube icon in the center of the page, and add a ‘Flashloan’ cube. We want to flashloan the amount to repay the debt position, either by selecting the same token, or swapping before repaying. If for example you have a $1000 debt of USDC, we will flashloan $1000 USDC as shown below.

<figure><img src="https://lh5.googleusercontent.com/SJXki13Ag9aXexCs7VEBUJ46ScT6goT8ZLufcncD12wJb4Yny7UcupHQSh3pgbUB51_EJ6k3NSgNCcz3mQuMozxIMTyi96d9VyJjctxoeFc-bnnJeolaLQlH_p_IGQKHil2n2j-w6aKDoGg12GCqDnY" alt=""><figcaption></figcaption></figure>

2. Next we will add the ‘Repay’ cube to repay the debt position. We will use the flash loan funds to repay this amount. Once the repay cube is added with the token amount, set it above the bottom flash loan cube.

<figure><img src="https://lh6.googleusercontent.com/x57yEZz77TJJe3_NJazbWaWT8lQjV0fJ0NxMWTY-FVvITtg9qBxKIAdyniM1_5ykqaRtCIusELPiqGTv1jYbo67UkLFmLkPsgc6u5qbZF01H4tcOkBehz2EDnk_0qcitoLg0rtfUKV9Cr_xgL2a4wok" alt=""><figcaption></figcaption></figure>

3. Next, we will add the total collateral funds to the Furucombo proxy contract using the ‘Add Funds’ cube so that we can withdraw our position. For example, if I had 1500DAI as collateral, my add funds cube will be for 1500aPolDAI (depending on the network). The add funds cube must be in the amToken that you have provided to Aave as collateral. In this example, our collateral is DAI, so we will use the aPolDAI token (depending on the network) to add funds back to the contract.  Again ensure the add funds cube is above the bottom flash loan cube.

<figure><img src="https://lh4.googleusercontent.com/exiFBuiFhxSGdExrnp198jWuCw0YL9hNW9h4MPxo8SW9JrTWyJeq3hJRBmxpPq8QpPDOB7nND_GLgRpeQEIYJTsjftBIugjhEpj1fnuthjmoWSofOghtW4ZLYs2_yZvkh2uums3_muPM5dmKbZlawuE" alt=""><figcaption></figcaption></figure>

4. With the add funds cube in place, we can withdraw the collateral. Next we will use a ‘Withdraw’ cube, and withdraw the collateral position. Add the withdraw cube, and add the amToken as your input in order to withdraw the collateral from Aave. In this example, we will withdraw the aPolDAI to DAI.

<figure><img src="https://lh4.googleusercontent.com/mB2qXOqF1mDZ3tkIIiGBgRJ1t8TGijYAhNdDJIrJAczWe95DMsU7gPWRGxQ1itgeGa0OTmVNInnpLc1j03nnblCQ4Mhhgm-CfLwYTYjJNU-_sR4T32P2OdZSgRAV5W0DeHHmYZ_XYCKpnl95n2m_xzE" alt=""><figcaption></figcaption></figure>

5. (optional) With the funds withdrawn, we now need to swap the DAI to USDC in order to pay back the flash loan that was borrowed. Because the collateral in Aave is higher than the debt position, it allows us to pay back the flash loan with extra collateral to spare.

<figure><img src="https://lh5.googleusercontent.com/uZeRw--jnsl58fWnbwmkiW04sBLrChwjop1Q5b9JKWeT8-i7gMmTLqqBceCha1q7zoaHYLNdtHcoLt2qH7tVPnzqNxlCdLEPNP0SqhXZK2l1-tvZk_w5S9BJ3dO9rnXAWFqaoL1rnYITCjqOQHdhbGs" alt=""><figcaption></figcaption></figure>

This is how you perform a De-Leverage strategy on Furucombo. If you have any questions or concerns, please reach out to us on our [community Discord](https://go.furucombo.app/Discord).

To learn more about our other position management features, click the following tutorials:

1. [Collateral Swap](https://docs.furucombo.app/using-furucombo/tutorials/collateral-swap-tutorial)
2. [Debt Swap](https://docs.furucombo.app/using-furucombo/tutorials/debt-swap-tutorial)
3. [Leveraged Long Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-long-position-tutorial)
4. [Leveraged Short Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-short-position-tutorial)
