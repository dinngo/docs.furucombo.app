# Debt Swap Tutorial

<figure><img src="https://lh4.googleusercontent.com/t-MYa6JxR7B6in8qRP6Xsqs1Zcyn3hsUk4cn2VlfrxbIcniNJSsyLHRNC-h19SuNcijM_4P7x7huQmonKFaGvjhP5TUG9W6JhM86a7S3Cc45ddpXhE8TgDFqOeXCUQUhM_i_Wnano7IzyyYJqRU5zBM" alt=""><figcaption></figcaption></figure>

This tutorial will help you to create a debt swap on [Furucombo](https://furucombo.app/). A debt swap allows you to switch your debt position without paying back the original debt position without any upfront funds. This is completed through the use of flash loans. The reason to perform a debt swap is to reduce your borrow rate, or to leverage yourself with the borrowed asset. If you are more of a visual learner, you can use our [video tutorial](https://www.youtube.com/watch?v=YJxOAYEkHCc) instead.

## What is a Debt Swap?

A debt swap allows you to swap your debt position to another token. For example, if you have borrowed ETH, and want to switch it to LINK, then a debt swap allows you to manage your position and make that adjustment.

### What are the Advantages of Debt Swap?&#x20;

The advantages of a debt swap are that it can reduce your borrow rate, or to adjust your market risk by borrowing another asset. Additionally, with the power of Furucombo, this can be done without any upfront funds through the power of flash loans, and executed all within one transaction.

### When do I need a Debt Swap?

You can debt swap when you wish to adjust your market risk, or reduce your borrow rate.

### What is the difference between Aave V2 and V3?

The Aave V3 market offers greater capital efficiencies when compared to V2. To learn more about Aave V3, visit the [Aave V3 features page](https://docs.aave.com/faq/aave-v3-features).

## Steps to set up a Debt Swap combination:

1. Connect your wallet, and select the network of your choice on the top right of [create mode on Furucombo](https://furucombo.app/combo). Once connected, click the cube icon in the center of the page, and add a ‘Flashloan’ cube. We will want to take a flash loan out in the token we wish to repay the debt position with. In this example, if our debt position is USDT, we will take a flash loan in USDT. You’’ want to borrow the amount of funds you need to pay back the debt position of your choice. You don't have to pay back the full debt position if you choose.

<figure><img src="https://lh5.googleusercontent.com/vVRAzMtvhpg36MxLntkk8qsUx0lM6ecL7sayqebaZfkSLekMfKsAu3uMLvFBeEz9lDe2wE1juQml-lmdCpbcekBJdjf7XwwVZXUY7Tvy7QJivMvd6KJQ-i0v9rGT2G9WoGansWGDFFNQ90PcdJ3c7rY" alt=""><figcaption></figcaption></figure>

2. Next, we can use the flash loaned funds to repay our debt position. To do this, add a ‘Repay’ cube, and input the amount borrowed from the flash loan. Under the repay cube you can also see important information such as total debt, total collateral, and utilization which can help you to decide how much to repay. If you are repaying the full amount, confirm the number matches what you are repaying with your flash loan. Once confirmed, hit the set button, and add the repay cube above the bottom flash loan cube.

<figure><img src="https://lh6.googleusercontent.com/kQ2z5z2M7xos8CLoGfrL-Z4KlqXBix8G0mVpJ_DtP6LFAId86V2qDRf6NV7Qdjoj1ZvQa88N7K8nCvRw9VhDA7c3tkylv0gPxGkfY_VstL0xS1jnWb5IiWWS9ryxvprDBgAwM10zIx2C4aAPVGnAQ4c" alt=""><figcaption></figcaption></figure>

3. Now we can use the ‘Borrow’ cube to borrow a different kind of debt position. In this example, we will borrow $USDC and hit the set button. Again ensure the borrow cube is above the bottom flash loan cube.

<figure><img src="https://lh3.googleusercontent.com/H046V9e__EJL9WQSZyiwwZes9xOuyF7jaR184bbRdraAZJGHDilRjaasqBndmPGwcdzWx21qLymXGI60RVIkre2Apw1P406NwIWMtwnT4H_7p8y4pHerFY1JpFNF7GMKANOLvBNvyy5wVfY8QvZt19g" alt=""><figcaption></figcaption></figure>

4. Next we need to swap the borrowed asset to pay back the flash loan, or if you borrowed funds in the same denomination, you can skip this step. Add a ‘Swap Token’ cube, such as Paraswap, and swap the new borrowed token to the token borrowed by the flash loan in the first cube. You may have to slightly increase your collateralization ratio in order to pay the small fee from the flash loan cube. In this example, we will borrow an extra 10 USDC to compensate for this.

<figure><img src="https://lh4.googleusercontent.com/ItHilrPvLfOyS2ZPWRg-kOQC2skNEs9QSKz8b6SmiBjk2ol6ofCL62Cu2YioRwgitLoH9ZHzKsWbXQ8id7m3rinr0MjD0-kaqJ3Iq7wq-btHlj9Dv3CRJWIF42WEpv9Ewb9lSooXF6Zvfv-LgIk7BSw" alt=""><figcaption></figcaption></figure>

5. Now the combination is set up, and you can hit approve and execute at the bottom once you are happy with the numbers.

This is how you perform a debt swap using Furucombo. If you have any questions or concerns, please reach out to us on our [community Discord](https://go.furucombo.app/Discord). We hope you enjoyed using our Multi-Send feature.

To learn more about our other position management features, click the following tutorials:

1. [Collateral Swap](https://docs.furucombo.app/using-furucombo/tutorials/collateral-swap-tutorial)
2. [Leveraged Short Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-short-position-tutorial)
3. [Leveraged Long Position](https://docs.furucombo.app/using-furucombo/tutorials/leveraged-long-position-tutorial)
4. [De-Leverage Position](https://docs.furucombo.app/using-furucombo/tutorials/de-leverage-position-tutorial)
