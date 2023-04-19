# Collateral Swap Tutorial

<figure><img src="https://lh5.googleusercontent.com/K8db4uKO1QxWvNCgBsP3QEnu-cxJzZVfLr9TPxpADlGRjbybBI-0GtdMu7TG6aIZ7icpgmj1XJf9RnUoS3T_j4N7CJncOtJN3yO0P48DicC3XHzrXnPcx7a6zjWoI26ylDiJ5LJztKTBCg4--x3mwCg" alt="Collateral Swap Tutorial"><figcaption><p>Collateral Swap Tutorial</p></figcaption></figure>

This guide is to help you understand the utility, and how to set up a collateral swap combination on [Furucombo](https://furucombo.app/). The collateral swap combination on [Furucombo](https://furucombo.app/) allows you to change your collateral position on a lending protocol, such as Aave, without paying back your current debts, and without having any upfront funds by using the flash loan feature. This can be done to change your LTV ratio, your collateral earn percentage, or to change your market risk by switching assets. If you are more of a visual learner, you can use our [video tutorial](https://youtu.be/NaZgZTO41M0) instead.

## What is a Collateral Swap?&#x20;

A collateral swap allows you to swap your collateral position within the protocol without first liquidating your position. This means you can swap collateral without paying back your debts.

### What are the Advantages of a Collateral Swap?

The advantages of a collateral swap are that you are able to switch your position without any upfront funds using flash loans. This is beneficial because it allows you to change your loan-to-value ratio, change your collateral earn percentage, or adjust your market risk by switching assets.

### When do I need a collateral swap?

You can use a collateral swap whenever you wish to take advantage of the above benefits.

## Steps to perform a collateral swap:

1. Connect your wallet, and select the network of your choice on the top right of [create mode on Furucombo](https://furucombo.app/combo). Once connected, click the cube icon in the center of the page, and add a ‘Flashloan’ cube. We will want to take a flash loan out in the token we are removing the collateral position with. In this example, if our collateral position is currently USDT, we will take a flash loan in USDT. You can choose how much collateral you want to swap, and take a flash loan of that amount. You don't have to swap the full collateral position if you choose.

<figure><img src="https://lh3.googleusercontent.com/a_TcxVhVm-jfmtfASBVIZtNUJi97fTL2FJ3R36aa8xajewNNNwoalVMneDXHaxEbkcsEgXcJuU7KAywB0CW2ox-z7HE-wtuY53XZTOlpYzte3MMnxP_5dyP9C25MEdIe3gGtF_j8kBA9LOPQ14n7AN4" alt=""><figcaption></figcaption></figure>

2. Next we will swap to the token you wish to deposit as collateral. If that token is ETH, swap the flash loaned USDT to ETH using a ‘Swap Token’ cube, such as Paraswap. Ensure that the swap token cube is above the bottom flash loan cube.

<figure><img src="https://lh6.googleusercontent.com/cZNyHfnbsUoeF8uyLy9hFJuOItvatvSi5CviOCsaBNL6tX3fpyqkXnKlm4SKzWrz19V5_IbtrWYUPpN5ZTkr1dKhHFf3Y4T8gweh7Tmmn5_htQPIOGs0q9X_T1iKUzT7s1Apx5PP_l4NauDQsE-et6w" alt=""><figcaption></figcaption></figure>

3. Now we can deposit the new collateral into the lending protocol, such as Aave. To do this, use the ‘Deposit’ cube under Aave, and add in the token amount after you perform the swap. In this example, that will be ETH. Again ensure that the deposit cube is above the bottom flash loan cube.

<figure><img src="https://lh6.googleusercontent.com/hlbVZzxcr9VNXT48kTJaAirS-VSjXH8hKBczSkimjTN-vyEmJBZt-8uR5X7bTwN-0kUJWe7R0UntO0fDoE336feKJKzYCeHq_61aJuyegTsRR2VhdO3T7YOifgggZHUjPJAiQjHc15zSOLTgaD2xLqE" alt=""><figcaption></figcaption></figure>

4. The next step is to return the funds to our wallet, so that the system knows that we have additional collateral in the denomination of aTokens, or aWETH in this example. Add the ‘Return Funds’ cube and add the aToken, or aWETH in this example, and add it just above the bottom flash loan cube.

<figure><img src="https://lh5.googleusercontent.com/VgmY9Eyd8xLczqV51TiF2rTQGMv5JWPAOjR4h9pbZGOC2gPkfd0ibTrGfdAOPZwrTKXdMyM2avczTab0g0GIa9tSVCQ72RL6vW-BfnUpa3YDrAc8uCnu1JnzHnYRItnWReC9K_YXo0CSiyG07PfQPAI" alt=""><figcaption></figcaption></figure>

5. Now the system will recognize our new collateral. We can add our old collateral to the contract so that we are able to remove it from Aave. To do this, add a ‘Add Funds’ cube, and input the original collateral token, and token amount. In this example, it will be aUSDT in the amount of 2000. Add it above the bottom flash loan cube.

<figure><img src="https://lh5.googleusercontent.com/ba4ITz0ibjAL38OH0ihrRoQuqTz7jHwjozl2xlzdnxj_XCN9aqcd5EL02ArzPG-DbEoe0jihpUsY7tgjSvfNttWCRFmiCJLAfNkFfn8RUEL5ASP4m80tSAMMKd7OGqP8YvjP-9ACs2SS_6GmZ-oTIOA" alt=""><figcaption></figcaption></figure>

6. With the funds added, we can now remove the original collateral position. To do this, add a ‘Withdraw’ cube, and input the aUSDT to withdraw the position, and get USDT tokens back. This will allow us to complete the collateral swap, and to pay back our flash loan. Again, add it above the bottom flash loan cube.

<figure><img src="https://lh6.googleusercontent.com/64aTKHxo8g85vctleLaGLTMaJfTsjgC-Hx9mJwehx5cyoUq8-z-ldQkxNp58o2dCqwlV6tfaHPRPuzWSgZm5ZHeY-X__J7h-YPP6hqgfQwTVjEK6DLRl-N4Y3iDQMIo1bvTxGIPXldu0it2pHc68UzY" alt=""><figcaption></figcaption></figure>

7. Once you are happy with the results, click approve and send at the bottom to complete your transaction.\


This is a quick and simple guide on how to perform a collateral swap on Furucombo. If you have any questions or concerns, please reach out to us on our [community Discord](https://go.furucombo.app/Discord).



To learn more about our other position management features, click the following tutorials:

1. [Debt Swap](https://docs.furucombo.app/using-furucombo/tutorials/debt-swap-tutorial)
2. [Leveraged Long Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-long-position-tutorial)
3. [Leveraged Short Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-short-position-tutorial)
4. [De-Leverage Position](https://docs.furucombo.app/using-furucombo/tutorials/de-leverage-position-tutorial)
