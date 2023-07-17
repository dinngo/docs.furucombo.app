# Lending Dashboard

<figure><img src="../.gitbook/assets/lendingdashboard_live_mv_AdobeExpress_051 (1).jpg" alt=""><figcaption></figcaption></figure>

The [Lending Dashboard](http://furucombo.app/lending) is a new feature for [Furucombo](https://furucombo.app/) that allows you to easily manage your positions on lending protocols such as Aave and Compound with the click of a button instead of manually adding each cube.

The following combinations are possible from the new Lending Dashboard:

1. Deposit
2. Withdraw
3. Borrow
4. Repay
5. Collateral Swap
6. Debt Swap
7. Leverage
8. Deleverage

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

Visit our [tutorial page](https://docs.furucombo.app/using-furucombo/tutorials/lending-dashboard-tutorial) for a guide on how to take advantage of these new features. If you are more of a visual learner, you can watch our [Youtube tutorial](https://www.youtube.com/watch?v=ev7cDY7KZ4A) instead.



The Lending Dashboard has a base fee of 0.25% of the positions operation, this includes the initial fee calculation. This fee only applies to collateral swap, debt swap, leverage, and deleverage. For example, if you perform a collateral swap of $2000 USDC total, then the total fee is equal to (2000 \* 0.25%) = $5.
