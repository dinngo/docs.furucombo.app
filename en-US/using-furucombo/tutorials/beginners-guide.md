---
description: A step-by-step guide on how to build a combo on Furucombo!
---

# Beginner’s Guide

![](<../../.gitbook/assets/image (3) (1).png>)

Welcome to Furucombo. In this guide, we’ll walk through all the basics you need to know to successfully create a combo. Before we begin, let’s talk about “what is Furucombo?”.

## What is [Furucombo](https://furucombo.app/)?

Furucombo is a tool built for end-users to optimize their DeFi strategy simply by drag and drop. Just like building your own DeFi legos, but you don’t need to know how to code. It visualizes complex DeFi protocols into cubes. Users just need to enter inputs/outputs and set up orders of the cubes (we call this a “combo”), then Furucombo will package all the cubes into one transaction and send out. This is a great tool for people who want to perform actions across different protocols, especially those who want to leverage flashloan. (We cover flashloan in the article [here](https://medium.com/furucombo/create-flashloan-combo-on-furucombo-c7c3b23267f0).)

Now you get the idea of what Furucombo is, let’s get started!

## Furucombo Interface Guide <a href="#229e" id="229e"></a>

### ・DeFi Menu <a href="#e7c5" id="e7c5"></a>

To start creating a combo, first, you’ll need to select a DeFi protocol. Click the “＋” cube then a menu of DeFi protocols will pop up. Here you can choose which DeFi protocol you want to put in your combo. Each button represents a cube to be set up. Each cube means an action to be executed. The search feature at the top lets you search by defi name, defi action (e.g. swap, add liquidity, etc) or name of the token that is supported under certain defi.

![DeFi menu](<../../.gitbook/assets/image (27).png>)

### ・Quick Menu <a href="#e7c5" id="e7c5"></a>

If you are interested in utilizing pre-built combo strategies on Furucombo, you can easily access them by clicking the "Quick" menu button. Our team has compiled a list of the most popular trading strategies used by Furucombo users, which can save you time and effort in building everything from scratch. This menu is especially helpful for those who are new to Furucombo and want to get started quickly, or for those who prefer to use established strategies instead of creating their own. Give it a try and see how it can streamline your trading experience on Furucombo.

<figure><img src="../../.gitbook/assets/Screenshot 2023-05-15 at 4.00.57 PM.png" alt=""><figcaption><p>Quick menu</p></figcaption></figure>

### ・Initial Funds <a href="#1bcf" id="1bcf"></a>

![](<../../.gitbook/assets/image (31).png>)

When you start setting up cubes, you may see a section at the top left called “Initial Funds”. It means the funds that you must provide at the beginning of the combo to initiate the transaction.

Initial funds are sent directly _**from your wallet.**_ That been said, you must have enough balance of the token(s) in your wallet otherwise the transaction will _**NOT**_ be executed. When your wallet is connected, the wallet balance of each token will be displayed here so you can always check before sending out the combo.

### ・You will receive <a href="#5cd0" id="5cd0"></a>

![](<../../.gitbook/assets/image (22).png>)



On the left, you see a “_**You will receive**_” section. These are the funds to be returned back to your wallet at the end of the transaction. It is the result of all the inputs and outputs you’ve built on the right, which are updated every time you make a change of a cube.

```
👩🏻‍🏫 Just think that 
“Initial Funds” is how much you put and, 
"You will receive" is how much you get at the end.
```

## Step by step <a href="#2fb4" id="2fb4"></a>

### Step 1: Setting up cubes ⚙️ <a href="#0903" id="0903"></a>

![](<../../.gitbook/assets/image (19).png>)

When you select a protocol, you’re led to enter the details of the cube. Here you will frequently see the terms “Input” & “Output”.

```
Input means how much token you'll spend upon executing this action.
Output means how much token you'll receive upon executing this action.
```

Source of input can be tokens you have in your wallet or it can be outputs of previous cubes. Once you set up the cube, you can always edit/delete it by clicking the pen/trashcan icon at the top right of each set.

### Step 2: Drag and drop 🖱 ✋🏻 📦 <a href="#5853" id="5853"></a>

![](../../.gitbook/assets/1\_IoY6IDMU4sMF-3GcuoeBMw.gif)

All cubes you set up are draggable. Simply _**drag**_ them in the order you wish. When the combo is sent, actions are executed according to the order of the cubes.

> Example: When you create flashloan, you’ll see a pair of two cubes appear. (1st cube means “borrow” and 2nd cube means “payback”.) The next thing you need to do is adding more cubes (actions you wanna do with the borrowed tokens) and **drag** them between the flashloan pair.

### Step 3: Connect Your Wallet 👛 <a href="#f5ac" id="f5ac"></a>

![](../../.gitbook/assets/1\_OQuSodPu0Ues59xxPALG0Q.gif)

You can create a combo without connecting to your wallet. But if you want to send out the combo, you must connect your wallet. Simply click the cube with a wallet icon. Then choose your wallet to connect.

### Step 4: Sending Out a Combo 🔗 🎉 🎁 <a href="#bafb" id="bafb"></a>

![](../../.gitbook/assets/1\_N7oVqm9E2XX-Z8VaWws52A.gif)

The complete flow of sending out a combo would be:

1️⃣ Click “_**Approve**_” when your initial funds are ERC20 tokens. You only need to do this once per token.

2️⃣ Click “_**Send**_”, then Furucombo will run an estimate of your combo. If the transaction will fail, a message will pop out as a reminder so you can modify your combo. Conversely, you will see a request pop-up on your wallet to sign the transaction.

3️⃣ Once your combo is sent out successfully, the button changes to “_**New Combo**_” and a message with the transaction link pops up. When you see these changes, congrats!

You’ve completed a combo! Don’t forget to share your result on Twitter simply by clicking the Twitter icon.

We’ve also made a video tutorial of this guide. Check it out 👇🏻

{% embed url="https://www.youtube.com/watch?v=wCfMm2a91qs" %}

## &#x20;<a href="#c2c7" id="c2c7"></a>
