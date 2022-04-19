---
    title: 'Module 1, Lab01 - Install and configure Domain Controller, Hyper-V hosts in Azure'
---

# Student lab manual

## Lab scenario

Loremipsum loremipsum Loremipsum loremipsumLoremipsum loremipsumLoremipsum loremipsum

## Objectives

In this lab, you will:

+ Task 0: Activate Your Azure Trial subscription
+ Task 1: Increase subscription vCPU quotas
+ Task 2: Deploy the lab infrastructure
+ Task 3: Basic infrastructure deployment

## Estimated timing: 60 minutes (approx)

## Instructions

### Lab 1

#### Task 0: Redeem Azure Pass Promo Code

1. Open a browser and navigate to: [Microsoft Azure Pass](https://www.microsoftazurepass.com)

> **Note**: It is recommended you close all browsers and open a new **In‐Private (Incognito) Browser** session. Other logins can persist and cause errors during the activation step.

2. Click the **Start** button to get started.
3. Enter your account login information and select **“Sign In”**.

>**Note**: If possible, create a new (dummy) Microsoft Account for activation of Azure Pass voucher.

4. Click **“Confirm Microsoft Account”** if the correct email address is listed.
5. Enter your promo code in the Promo code box and click **“Claim Promo Code”**.
6. It may take few seconds to process the redemption.
7. Enter the mandatory Profile information

>**Note**: There are few fields that are necessary, like Country, Name and contact phone. the rest of the data can be skipped or use generic terms (i.e address)
8. Select the check box - I agree to the subscription agreement, offer details, and privacy statement, and then click on *“Sign up”*.
9. On the feedback page, enter your feedback and click on Submit.
10. It would automatically redirect you to the Azure Portal and now you are ready to use Azure services.

>**Note**: Do not click, close the browser until the process is finished. The system will automatically redirect You to the tenant.

#### Task 1: Increase subscription vCPU quotas

1. For the Labs we would be using multiple compute resources which would require additional vCores, so we need to create a request under the Subscriptions to make sure the lab is executed properly.
2. Login to the [Azure Portal](https://Portal.Azure.com)  and in the **Search bar** type Subscriptions, then select the Subscriptions.
3. Select your subscription from the list.
4. From the **Subscription** menu, on the left side, scroll down to **Settings** blade and select **Usage + quotas**
5. In the **Search** bar area, choose the datacenter location under **Locations**, select *Microsoft.Compute* under **Provider**. Make sure that **Group by** is per Location.
6. It will list the quotas per selected **Location**. Update the following fields, by clicking on edit button:

| Setting | Value |
| --- | --- |
| Total Regional vCPUs | 20 |
| Standard BS Family vCPUs | 20 |
| Standard Dv2 Family vCPUs | 20 |
| Standard DSv2 Family vCPUs | 20 |
| Standard DSv4 Family vCPUs | 20 |
| Standard Ev4 Family vCPUs | 20 |

7. After clicking on **Submit**, repeat step 6, for each VM Family vCPU setting.

>**Note**: It needs to be done per each vCPU setting, by specifying a **New Limit**.

8. Refresh the page few times, to make sure that quota increase was completed.

>**Note**: You might need to wait up to 10min for the refresh.

### Task 3: Basic infrastructure deployment
