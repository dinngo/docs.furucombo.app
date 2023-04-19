# Lending Dashboard Tutorial

<figure><img src="https://lh6.googleusercontent.com/Fll_C_mRXwUYwKqkbHB9vqNG5F9ZlpLB3-fJmP0frAUzlrcw_LVQi7y9OcXGg6OKM3N15dYqV2AKu7Pr0qb2MTpbgydLOEtNjj2Zw8ML2Vrx35IuY2pipv4JXAu_FL44LqeM8caEap3IqjYot-31Wfw" alt=""><figcaption></figcaption></figure>

The [Lending Dashboard](http://furucombo.app/lending) is a new feature for [Furucombo](https://furucombo.app/) that allows you to easily manage your positions on lending protocols such as Aave and Compound with the click of a button instead of manually adding each cube.

This tutorial will guide you through the new features and how to complete each kind of position management.

The following combinations are possible from the new Lending Dashboard. If you already know what kind of combination you are looking to perform, you can jump to the different sections by clicking the link below:

1. [Deposit](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial#deposit)
2. [Withdraw](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial#withdraw)
3. [Borrow](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial#borrow)
4. [Repay](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial#repay)
5. [Collateral Swap](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial#collateral-swap)
6. [Debt Swap](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial#debt-swap)
7. [Leverage](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial#leverage)
8. [Deleverage](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial#deleverage)

### Lending Dashboard Overview

<figure><img src="https://lh6.googleusercontent.com/W_vXGb5VJNWAhNR7qrgmeu2H_BmxVLmFCIEQkTeV-Dis3Z6-zDnVNfE_qViK6Fcpf64J6SoKqbj0WHsM04wqfthEapgsZcV3_u4qujq3Rw2dHA4yM4RTQeeP8tQ1Trx4ruUXCDKVsTKArkNzR_NsIKU" alt=""><figcaption></figcaption></figure>

Click the ‘Lending Dashboard’ at the top to be greeted with the new interface. From here we can do many actions to manage your deposits. The following is a list of terms in order to better understand the dashboard:

* Left hand side shows the assets supplied to the lending protocol, in this case Aave V3
  * Additionally you can see the APY earned from the deposits, in the above example you will earn 2.31%
* Right hand side shows the assets borrowed from the lending protocol, in this case Aave V3
  * Additionally you can see the APY charged for borrowing the assets, in the above example you will be charged at 2.68%
* **Utilization:** Represents the share of borrowed liquidity. As you get closer to 100%, it means more of your collateral is being used by borrowing. Be aware of the liquidation risk if your utilization rate gets higher than the threshold as determined by the lending protocol.
* **Health Rate:** The health rate is a numeric representation of the safety of your deposited assets against the borrowed assets and its underlying value. The higher the value is, the safer the state of your funds are against liquidation. If the health factor reaches 1, a liquidation of your deposits will be triggered.
* **Deposit:** Make a deposit to the lending protocol.
* **Withdraw:** Withdraw some or all of your assets from the lending protocol.
  * Note: You must keep your utilization rate under \~80% depending on the assets LTV ratio. If you want to liquidate your assets, you can use the ‘Deleverage’ button.
* **Collateral Swap:** This allows you to swap your collateral (deposited assets) within the lending protocol without first repaying your debts (requires no upfront funds).
* **Borrow:** This allows you to borrow an asset or assets from the lending protocol based on the amount of collateral you have deposited. Typically, this is around \~80% of the loan-to-value ratio.
* **Repay:** This allows you to repay any outstanding debts you have on the lending protocol.
* **Debt Swap:** This allows you to swap your debts (borrowed assets) within the lending protocol without first repaying your debts (requires no upfront funds).
* **Leverage:** This allows you to increase your exposure to the market (either long or short) by using the existing collateral you have in the lending protocol.
  * Note: This will leverage your position, and also increase your utilization rate. Make sure you understand the risks before taking on leverage.
* **Deleverage:** This allows you to close your position on Aave without first repaying your debts. This is useful to avoid liquidation, or to close your position when you do not have any upfront funds.

### Deposit

In order to borrow an asset from a lending protocol, you must first make a deposit.

1. To deposit, simply click the ‘Deposit’ button on the interface. You will then be greeted with the following screen.

<figure><img src="https://lh6.googleusercontent.com/Qbh4hwecWmFHfKE5RVR-99pp3hfRqz2n6FUr3JjZ1obRa6viaL7pVxSfxBrG3L1r_5n1wkqLGhNqZFlaxc0MQogQ5xsQwlzaMW51lgbpaf8vwANy4akobD0g-KkwLWfUMBuDT1TsHn0PUKenUjy-RWc" alt=""><figcaption></figcaption></figure>

2. Next, you can choose which tokens you want to deposit. Click the drop down menu and choose the token you want to deposit, and the token amount. Also note the ‘+’ button allows you to deposit as many tokens at one time as you see fit. Once you are happy with the selection, your interface will look something like the following.

<figure><img src="https://lh6.googleusercontent.com/g1rJsusvkSAF0ukGQKoGAvNSHF3yalPhY2-VOeLYj0Pg8meP2nzRDTeGEPNb4vgtk2WNwLQEuKyJKlJdym46X3uuJ80g7GtjPFCI9R5nCneFN-83huH_K46vdnM5GcSfWQvMzd7_oUdX-HjkTBEPU2w" alt=""><figcaption></figcaption></figure>

3. Once you are happy with your selection, you can click ‘Appove’ and ‘Send’ to complete the transaction. Once the transaction executes on the blockchain, your deposits will show on the left hand side of the Lending Dashboard. You have now successfully completed a deposit combination.

### Withdraw

You can withdraw your collateral, or deposited tokens, from the lending protocol using the ‘Withdraw’ function. To perform this, you must have enough collateral to cover your debts, or no outstanding debt if you are removing all your collateral. If you want to pay back your debts and remove your collateral in one transaction, you can use the ‘Deleverage’ combination instead.

1. To withdraw your assets on the lending protocol, simply hit the ‘Withdraw’ button on the Lending Dashboard. The list will automatically populate with your deposited assets. You will be greeted with the following interface.

<figure><img src="https://lh3.googleusercontent.com/TnFL2Xp9eBArdPe9BVekNm4xb0BFzXo9yoj0FGPc0wLuP_M_zPB0w92TRFf-0uryGWThKiFbDz69bK-r0qbwvcMG4BGfI2LciCrnkZTbEfbZV6bQKPRcL2Y0erVImt3Df3VO1vYFcUl9yXxF_r2UIn8" alt=""><figcaption></figcaption></figure>

2. Next, decide which tokens you want to withdraw, and the token amount. Also be aware that your Utilization rate and Health Rate will change based on the amount you are withdrawing if you still have outstanding debts. Once you input the values, the interface will update as follows.

<figure><img src="https://lh3.googleusercontent.com/XxFkpAJliX-yFZ9Ty01MTJi5VxVtpxfFK-ZR2ocQP3gJTe8AnycsBSfsJVJFm6aPVSenx4CNqEt9NanpDgoXBgWXleY5a5EnsBsGMAUv9OR0nK6ME1fG7WC8bYIufiE_FZ-o4sGPXQsPODDSPrz9Jaw" alt=""><figcaption></figcaption></figure>

3. Once you are satisfied with the choices you’ve selected, you can hit ‘Approve’ and ‘Send’. Once the transaction is executed on the blockchain, you will have withdrawn your assets from the lending protocol. You have now successfully completed a withdraw combination.

### Borrow

The borrow function allows you to borrow tokens from a lending protocol based on your collateral.&#x20;

1. To perform a borrow combo, click the ‘Borrow’ button on the right hand side of the Lending Dashboard. You will be greeted with the following interface.

<figure><img src="https://lh4.googleusercontent.com/0jaJ3ULPSQ0vQPP0F-MlCQE45aLkieLC34Um2GLBzwdAVSV9ZRh0GV3NsYfcC7Ds7ocgyf9M053iXKiEy6lYUjS7VE2CsmpVx7ofXQz4MlwonkMMEBlcgRbs9qe0eKvrQqymscKZEdW9K_RDK85cXms" alt=""><figcaption></figcaption></figure>

2. From here, you can choose which tokens you wish to borrow, and the token amount. Note the ‘+’ button which allows you to borrow multiple tokens at once. Once you have added the tokens and token amounts, your dashboard will populate similar to the following.&#x20;
   * Note: When borrowing debts, be aware of the changes in Utilization rate, the Health Rate, and your Total Debts.

<figure><img src="https://lh4.googleusercontent.com/yzsgW3yYzz5lKWdUJDNMgCNqvKo9617o4Uvt-7Ffl_rcwatabLqQ4v-wk8laHjWeYITIEklEXk7LCHyETn0Zh-hTM3GI7rpxEc6HO9CdWLg5mqVeArp1n321_HBOtRCzdKYNpw4Geb_bYWJ8n38GLaw" alt=""><figcaption></figcaption></figure>

3. Once you are happy with the selections, simply click the ‘Approve’ and ‘Send’ buttons on the interface, and the transaction will execute on the blockchain. Once completed, the Lending Dashboard will update to show the new data. You have now successfully completed a borrow combination.

### Repay

The repay function allows you to repay any outstanding debts you have on a lending protocol.

1. To start a repay combination, simply click the ‘Repay’ button on the right hand side of the Lending Dashboard. You will be greeted with the following interface. Your outstanding debts will automatically populate.

<figure><img src="https://lh4.googleusercontent.com/-yGbSuYzlIoBLfW8czV2ubXROg-pM66Kr3_HabUxAfw7QthXJvTe6cjkxxMgX0b9mAvbK58UQ4UpMwujqpEc6jGKZtwCkPs3XttlU2uJPeAcmNQCo8ScvJmwgkj_WQ_Fh-2fLNxP6r5cJzFk2JPwKVI" alt=""><figcaption></figcaption></figure>

2. You can choose to repay your debts with the tokens, or choose to swap from a single token to the borrowed tokens, and repay from the swapped token. This means that you do not have to have the token you wish to repay if you have another token you can pay with. For the above example, you can choose to ‘Swap and repay’ using Ethereum as shown below.

<figure><img src="https://lh5.googleusercontent.com/faaDt3ILcDZnwwN8e83ALdzkdsCtzjb-w_30tVG0gkizVh2VDGHd53f98FeGAfqJ4_ch8p4WztJ4LMkow8t2zirHWNK1gYpfld6innDGRaqZ1zCgGePUyhpjkrN6bjDLWLhhrgndUoX18F-FUYqBbYo" alt=""><figcaption></figcaption></figure>

3. Once you have decided the tokens to repay, and the amounts, and whether you want to repay or swap and repay, you can ‘Approve’ and ‘Send’ the transaction. Note that repaying will change your Utilization rate, Health Rate, and Total Debt. Once the transaction has been completed, the Lending Dashboard will update. You have now successfully completed a Repay combination.

### Collateral Swap

This section of the guide will walk you through how to do a collateral swap. A collateral swap is used when you want to swap your collateral (deposited assets) within the lending protocol without first repaying your debts (requires no upfront funds).

1. To start a collateral swap, simply hit the ‘Collateral swap’ button on the Lending Dashboard interface. Here you will be greeted with the following screen.

<figure><img src="https://lh3.googleusercontent.com/l0L8UCWTDREgEGd82CQ7E-dQkVg963Ce9c0ltO5MOGn27sByRagDaShDrRdSa3b8wU_iPo-98dCFRKKnLctx9mV5LSFdK3RzLNBQRu_BG0fGi4iI7-bMn1Tlcw7IdOP_FogK6F1aMUIbaLjI7fn0TD4" alt=""><figcaption></figcaption></figure>

2. Now choose the ‘Current Collateral’ you wish to swap from, and the ‘New Collateral’ you wish to swap to. Also note the following as some as the values might have changed:
   * Utilization Rate
   * Heath Rate (before and after)
   * Net APY (before and after)
   * Can be collateral (before and after)
   * Liquidation threshold (before and after)
3. Once you are happy with the choice, you are ready to ‘Approve’ & ‘Send’. And that’s it, you can see your new collateral on the Lending Dashboard once the transaction has completed. You have now successfully completed a Collateral Swap combination.

To learn more about how this trade works, or to create this combination as an advanced user, you can find more details on our [Collateral Swap](https://docs.furucombo.app/using-furucombo/tutorials/collateral-swap-tutorial) tutorial.\


### Debt Swap

This section of the guide will walk you through how to do a debt swap. A debt swap is used when you want to swap your debts (borrowed assets) within the lending protocol without first repaying your debts (requires no upfront funds).

1. To start a debt swap, simply hit the ‘Debt swap’ button on the Lending Dashboard interface. You will then be greeted by the following screen.

<figure><img src="https://lh5.googleusercontent.com/HjHBTgp7KQp2GRqgf3P8M_8ABJ1gyvJatqw48iexbJjrNvsKuGDvXSExUtFHSFkfTaH75wrt9pZhRKaXgbuxHgX0lXkBDnMuzc2cmfo805tclh8ByX4yinvLP8nXAMH2dkB2em5zx6jy2v0E89ujEZs" alt=""><figcaption></figcaption></figure>

2. Now you can choose the ‘Current Debt’ you wish to swap from, and the ‘New Debt’ token you wish to swap to. Also note the following as some as the values might have changed:
   * Utilization Rate
   * Heath Rate (before and after)
   * Net APY (before and after)
   * Can be collateral (before and after)
   * Liquidation threshold (before and after)
3. Once you have decided which token to swap to, and the amount to swap, all that’s left to do is ‘Approve’ and ‘Send’. And that’s it, it’s easy to perform a debt swap with the new Lending Dashboard.

To learn more about how this trade works, or to create this combination as an advanced user, you can find more details on our [Debt Swap](https://docs.furucombo.app/using-furucombo/tutorials/debt-swap-tutorial) tutorial.

### Leverage

Ensure you understand the risks of taking on a leveraged trade before you complete this combination. You should also understand the differences between going long or short.

**What is a Leveraged Position?**

A leveraged position is one that increases your market exposure over and above the original asset value. For example, a 2x leverage is one that has 2x more exposure than your base position. This is possible with Aave because you can borrow funds from your collateral. For example, if you have ETH as collateral, you can borrow a stable coin, such as USDC, and use that to purchase more ETH, therefore increasing your exposure to the market higher than would otherwise be possible with your original funds amount.

This section of the guide will walk you through how to perform a leverage trade using the Lending Dashboard.

1. To start a leverage trade, simply hit the ‘Leverage’ button on the Lending Dashboard interface. Here you will be greeted with the following screen.

<figure><img src="https://lh3.googleusercontent.com/QuzF771MhgOTt_6Hv4o_gXmIfe5Ut-YDwNn16oLZL-I4fGefxjH8ONPC2bUU4WgJyU_TJvPY1NpXPDGCZj4ZjePDjAjpcQmoqxky3-t57bZYxzqogbbUt3E5E0klbgPf-E97TZR8bNMNvuf-40vG_vo" alt=""><figcaption></figcaption></figure>

2. From the leverage page, you can choose to long an asset (you believe the price is going to go up in the future), or short an asset (you believe the price is going to go down in the future). How much you long or short will determine your leverage, utilization ratio, health rate, net APY, and total debt. Input values and determine the best choice for you.&#x20;
   * Note: Make sure you understand the risks before taking on leverage.

<figure><img src="https://lh6.googleusercontent.com/xWgYFtfSPkDlVswvdnGkQCF1VnY5jLiS1VgOr9qzbpG5sI4N9BMHCSUW-apLKRzmt9V5D-6_FNURzuSnBkA1A2pFC13p2r429fRV_u3J5kkRtYhC4qEdlFaq7RzMWzNIBhWPvTKtWKqelSCkmVoKolo" alt=""><figcaption></figcaption></figure>

3\. Once you are happy with your decision, all that’s left is to ‘Approve’, and ‘Send’. You have now completed a leveraged trade using the Lending Dashboard. Once the transaction executes, you can see the updated information on the Lending Dashboard. You have now successfully completed a Leverage combination.

To learn more about how this trade works, or to create this combination as an advanced user, you can find more details on our [Leveraged Long Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-long-position-tutorial) or [Leveraged Short Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-short-position-tutorial) tutorials.

### Deleverage

This combination will allow you to withdraw your position from a lending protocol, such as Aave, without any upfront funds. This is because it uses your collateral position, which is higher than your debt, to repay the debt and unlock the remaining principal.

This section of the guide will walk you through how to perform a deleverage trade using the Lending Dashboard.&#x20;

1. To deleverage a position, hit the ‘Deleverage’ button on any of your borrowed assets.
2. Next we will choose an asset to repay (pay back the debt borrowed), and an asset to withdraw (withdraw a collateral token). Once you have chosen the assets, input the amount you wish to repay. Also note the following as some as the values will change when completing this combo:
   * Utilization Rate → will decrease with this combo
   * Heath Rate (before and after) → will increase with this combo
   * Net APY (before and after)

<figure><img src="https://lh4.googleusercontent.com/rjgBf-jN9Xj5TdC6fSgqp13KzOq69Kod07ZWIzOTuzvxaBg_KXbOhvysG41hV54LMqZHWuzM-HCr1zxt63W7YfgWsAh2rfO7zhc0L3nlORQEIFJWhVUyEjsDwP8Rg67RmE5U-oAGX1-OAe0SM1s7Ugk" alt=""><figcaption></figcaption></figure>

3. Once you are happy with your selection, simply hit ‘Approve’ and ‘Send’. You have now completed a deleverage combo. The information will be updated on the Lending Dashboard once the transaction executes. You have now successfully completed a Deleverage combination.

To learn more about how this trade works, or to create this combination as an advanced user, you can find more details on our [Deleverage](https://docs.furucombo.app/using-furucombo/tutorials/de-leverage-position-tutorial) tutorial.



This is a tutorial and summary on how to utilize the Lending Dashboard developed by the Furucombo team. If you have any questions, please let us know on our [community Discord](https://go.furucombo.app/Discord), we are always happy to assist!

\
