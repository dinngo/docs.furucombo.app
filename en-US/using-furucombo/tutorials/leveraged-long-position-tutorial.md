# Leveraged Long Position Tutorial

<figure><img src="../../.gitbook/assets/Tutorial Position Management _Leveraged long.png" alt="Leverage Long on Furucombo"><figcaption><p>Leverage Long on Furucombo</p></figcaption></figure>

This tutorial will help you to create a leveraged position on [Furucombo](https://furucombo.app/). This combination will allow you to increase your leveraged position on a lending protocol, such as Aave, to increase your long position on the market. If you are more of a visual learner, you can use our [video tutorial for long positions](https://youtu.be/wocvDAdKq1U) instead.

{% embed url="https://youtu.be/wocvDAdKq1U" %}
Leverage long tutorial video
{% endembed %}

## What is a Leveraged Position?

A leveraged position is one that increases your market exposure over and above the original asset value. For example, a 2x leverage is one that has 2x more exposure than your base position. This is possible with Aave because you can borrow funds from your collateral. For example, if you have ETH as collateral, you can borrow a stable coin, such as USDC, and use that to purchase more ETH, therefore increasing your exposure to the market higher than would otherwise be possible with your original funds amount.

## How to Create a Leveraged Long Position?

A leveraged long position can be created by borrowing a stable coin, and swapping that to the asset you wish to go long on (an asset you expect to increase in value). For example, if you deposit $1000 in ETH into Aave, you can borrow $800 in USDC (a stable token), and swap that USDC to ETH, creating a market exposure of $1800 in ETH. If ETH increases in value, you will have to pay back less of the value that you used to borrow from the USDC because the ETH is a higher value. Always be aware that leveraged positions are subject to liquidation risk if the collateral falls below the loan-to-value ratio of the amount borrowed. The risk in this case would come from a decrease in the value of ETH (because there are less funds to pay back the borrowed funds).

## Steps to set up a New Leveraged Long Position:

1. Connect your wallet, and select the network of your choice on the top right of [create mode on Furucombo](https://furucombo.app/combo). Once connected, click the cube icon in the center of the page to get started. The first step is to make a position on Aave, and to decide which asset to use as collateral to go long on. When you have decided on which asset to deposit, simply add the ‘Deposit’ cube under Aave, and make a deposit in the asset you wish to use as collateral. If you wish to go long on Ethereum, deposit Ethereum.

<figure><img src="https://lh4.googleusercontent.com/d0yU_DaQe-0fD5F8ohFJDlZzKXw_UneYkgU3CsXtAhk3gGYbAmFH2yDfs8yPMIuWOw4rD2elkPNF8HRIvJK1ok44ccNakBbgolIGqi16Jieo3yPwICM28gvuSLuSGRaiS0Wi_jDk9a_nd_hpqQzWhtF4me6IZ8Ion3TPLRPtlDqIvoerdGKwYZ6P9eOG0w" alt="Aave Deposit"><figcaption><p>Aave Deposit</p></figcaption></figure>

2. Next we will use a ‘Return Funds’ cube to add the aToken to the contract in order to borrow an asset in one transaction. In this example, we will add the aEthWETH token in our return funds cube. If you deposit a different asset, simply carry over the aToken and the amount into the return funds cube.

<figure><img src="https://lh3.googleusercontent.com/M5T-WWig0HkfFdHmgBGcO_fpXwnZqCcxcY--xMP_6j5_DZ0TUIfeXqkSvLcYXvMspFkteD8q08zlERVNMFaxsYiPvaozlJRFoGdsrs5Q5nlDHIFnOTIShFOzFI0zop6qzcitjnh17rKBWlPMrgT1hJxOjDVkJ5ItzpbMgNMS0QO-Ehy_gqBOrVVfHbXmtA" alt="Return Funds"><figcaption><p>Return Funds</p></figcaption></figure>

3. Now we can borrow a stable token from Aave. We will borrow USDC in this case, but you can choose any stable token that's available on the lending protocol of your choice. At the time of writing, ETH is worth approximately $1750, so we will borrow 75% of our LTV, therefore we will borrow 1312.50 USDC.

<figure><img src="https://lh4.googleusercontent.com/D6XYzxA3K2_u9eCX3RgjcNo1nFdIpMnfG3j-ybP955ckvBwX97PucuzMrdHxM2yyzrgZB__AFWsIh64jqJ-HQnZByKM_bVfAzwvXEITqPurAnpnp40OL0C_5cYbnkEPVCB14mZjrQ95BzXmeO5hzkFkYKAeICp9DbAsret0Cqi6kTS0_9RvlkwZhvOZWhg" alt="Borrow a fund on Aave"><figcaption><p>Borrow a fund on Aave</p></figcaption></figure>

4. Next we will swap the borrowed USDC to ETH to increase our leverage or exposure to the ETH asset.

<figure><img src="https://lh5.googleusercontent.com/NuTnNvg-saNPl2p3Lka7_JY9W0mrOF_8K3C6YJ1ATvFR80dtgmRyfKcXC0aeEXxLHtNIBF0aUDC0CcQoFNJ9MYupCByHc1lP_PGQPr-Q0OWiBdspOgOAcXhfHCFrJtKY76ao5ravgN20NcUy1WNjjA-ACexHVQ3XzgNyyOdRXyaQSQzWX0QfGWW__eC1ZQ" alt="Swap the borrowed USDC to ETH"><figcaption><p>Swap the borrowed USDC to ETH</p></figcaption></figure>

5. Once you are happy with the numbers, you can hit ‘approve’ & ‘send’ at the bottom of the page. You have now created a leveraged position using Furucombo.



In the above example, we have made a deposit of 1ETH, borrowed USDC, and swapped that to ETH, creating a position of 1.746ETH from a deposit of 1ETH. This means the leverage created in this example is 1.746x, or 174.6%. This means that any 1% increase in Ethereum, will equal a 1.746% increase in value for the leveraged user. This is a powerful way to get additional exposure to the market. Also be aware of the risks of liquidation. If the value of the collateral decreases, you may be subject to liquidation risk. If that risk occurs, you can add more collateral, or perform our de-leverage strategy to reduce your market risk.

## Steps to Adjust your Leveraged Position with a Flash Loan

You can also use the flash loan feature to add a collateral position, and borrow an asset with that collateral to increase your exposure to the market. For example, if you have $1000 in collateral on Aave, and you’ve borrowed $600, or have a debt ratio of 60%, you can use a flash loan to increase your collateral position, and use some of the extra debt you can still incur to pay back the flash loan. Using the aforementioned numbers, let’s assume you want to increase your position by $1000. Assuming an ETH price of $1750, to increase the position by $1000, we need to borrow $800 (as we will borrow the other $200 from Aave in order to make up the difference) in the form of a flash loan.

1. Insert a ‘Flashloan’ cube in the amount you wish to increase your exposure by. Based on the above example, we will take a flash loan for 0.457ETH (or $800 value)

<figure><img src="https://lh5.googleusercontent.com/b5ZHRaaDAGsl5UI1BfO1wlvUqhnImu13WFE-uahsi_V80jJHNkgVhW2n00jgtB6Bg0QM52Elv9s3goRPV3RT5Huog2BRa3UGzSmCk5SrDloIUoktr486sU8qW_3zmcoaB8GC-WcQEbgryhLmOs9b4eK0E96Ch9OO8on_2aWzUIbBGRgfHVVeQZJxCXiUgg" alt="Create a flashloan cube"><figcaption><p>Create a flashloan cube</p></figcaption></figure>

2. Next we will perform the same steps as mentioned above. Simply add the ‘Deposit’ cube under Aave, and make a deposit in the asset you wish to use as collateral, in this case we are using WETH (note: ETH should be wrapped ahead of time using the utility cube ‘WETH’). Ensure the cubes are above the bottom flash loan cube.

<figure><img src="https://lh3.googleusercontent.com/HfP-h3UBj53RebDQBRW2Eyo7o4dRMqoAr_pbxnI6CL4mx4r9wIV-Msnu32cGrgztRwbuqKB1E-NtFEjQIdmawOg6VpaT8OcVmPu98CyonOX2S_KlG0oM_uqEmUV_-qGSSBZJT3Cp7UJC4E7a8wgdt-zBIH2eP4a2kVKySUxCYI6yXMk56SKZokHhvlnALw" alt="Deposit funds to Aave"><figcaption><p>Deposit funds to Aave</p></figcaption></figure>

3. Now we will use a ‘Return Funds’ cube to add the aToken to the contract in order to borrow an asset in one transaction. In this example, we will add the aEthWETH token in our return funds cube. If you deposit a different asset, simply carry over the aToken and the amount into the return funds cube.

<figure><img src="https://lh3.googleusercontent.com/a7PTHnTfii1Dbt6FMm2NncKTTkl4Ew-ki9UuV4r-o7m_X_tAIPbIfH4ef2hPRSLoPQCvMenOSu3YySF_U5UPi7WR2H07EaZZ0-Ueg3upJieD0QHx6Y3-zRXGBkg09Ap_wMCJA2jEgxx4dBBFXoSXPSL94yBYnYrX0qs3YxEea5-YiSx-9_vZgU9Auv7Urw" alt="Return Funds"><figcaption><p>Return Funds</p></figcaption></figure>

4. Now we can borrow a stable token from Aave. We will borrow USDC in this case, but you can choose any stable token that's available on the lending protocol of your choice. Because we made a deposit of $800 in value, we can borrow up to approximately 80% of the value of that, which would be $640. The other value will be made up from the extra debt we can take on from Aave, which will increase our loan-to-value ratio (thus increasing our liquidation risk, or our leverage to the market). In this example, we will borrow at least enough to pay back the flash loan. So we will borrow $850USDC, but how much you borrow will depend on your risk tolerance, collateralization ratio, etc.

<figure><img src="https://lh4.googleusercontent.com/js0hTvrCB_gjU-yt2RbeESW5wbyJPHw6R9C3sGg1mR5WAlIHcP6JJ33GHZFm4SuyAH_waj7ALNsjd2DHrlFeIhWzVfO7ukNr-VUSUb6UApQGSNKRqtrmZH9EtN8kfmitZBkEEbYgNFMK1RgEbWlbj_vAZmY_4fr7BhBzzZy1kkmHoeXNH5KlKDnBia9aqA" alt="borrow a stable token from Aave"><figcaption><p>borrow a stable token from Aave</p></figcaption></figure>

5. Next we will swap the borrowed USDC to ETH to increase our leverage or exposure to the ETH asset.

<figure><img src="https://lh6.googleusercontent.com/OTB1g5k_pZFRARu5NN2V9VuHvm11gtjDFcW7bsImnyo1cZBvMGaXQJzZcN4tfzk4LNbTDoUty60HFt__Q_kMsLdATDE7XvgCQsJP7-q7MyFMv90Gh0O9MIUCJtaaZs_1KwNaIHe6ppVslpGQGMfJqGMYqLRd2dvyJ9awJWGh2mQbmF_hij-F6AK3tsMnlQ" alt="swap the borrowed USDC to ETH"><figcaption><p>Swap the borrowed USDC to ETH</p></figcaption></figure>

6. Once you are happy with the numbers, you can hit ‘approve’ & ‘send’ at the bottom of the page. You have now adjusted your leveraged position with a flash loan using Furucombo.

To learn more about our other position management features, click the following tutorials:

1. [Leveraged Short Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-short-position-tutorial)
2. [Collateral Swap](https://docs.furucombo.app/using-furucombo/tutorials/collateral-swap-tutorial)
3. [Debt Swap](https://docs.furucombo.app/using-furucombo/tutorials/debt-swap-tutorial)
4. [De-Leverage Position](https://docs.furucombo.app/using-furucombo/tutorials/de-leverage-position-tutorial)
