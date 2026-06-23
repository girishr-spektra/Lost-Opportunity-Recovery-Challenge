## Getting Started with Challenge

We've prepared a seamless environment for you to explore and learn. Let's begin by making the most of this experience.

### Accessing Your Challenge Environment

Once you're ready to dive in, your virtual machine and challenge guide will be right at your fingertips within your web browser.

![](./media/know-ent-gs-g12.png)

### Exploring Your Challenge Resources

To get a better understanding of your challenge resources and credentials, navigate to the Environment tab.

![](./media/gs-leave-2.png)

### Utilizing the Split Window Feature

For convenience, you can open the challenge guide in a separate window by selecting the Split Window button from the Top right corner.

![](./media/gs-leave-3.png)

### Managing Your Virtual Machine

Feel free to start, stop, or restart your virtual machine as needed from the Resources tab. Your experience is in your hands!

![](./media/gs-leave-4.png)

> **Note:** If the VM is not in use, please **deallocate** it to avoid unnecessary resource consumption.

## Let's Get Started with Microsoft Azure

1. In the JumpVM, click on **Azure Portal** browser shortcut which is created on the desktop.

   ![](./media/know-ent-gs-g11.png)

1. On the **Sign into Microsoft** tab, you will see the login screen. Enter the provided email or username and click **Next** to proceed.

   - Email/Username: <inject key="AzureAdUserEmail"></inject>

     ![](./media/gs-lab3-g2.png)

1. Now, enter the following Temporary Access Pass and click on **Sign in**.

   - Temporary Access Pass: <inject key="AzureAdUserPassword"></inject>

     ![](./media/gs-lab3-g3.png)

1. If you see the pop-up **Stay Signed in?**, click No.

   ![](./media/gs-4.png)

---

## Download the Opportunity Dataset

Two data files have been prepared for this lab. Download the zip archive now — it contains both files you will need across the challenges.

1. Download the dataset archive:

   ```
   https://github.com/CloudLabsAI-Azure/hack-in-a-day-data/archive/refs/heads/lost-dropped-opportunities.zip
   ```

1. Once downloaded, extract the zip. Inside you will find two files:
   - **`opportunities.csv`** — 20 closed-lost opportunity records across five loss-reason categories (Pricing, Competitor, Product Fit, Long Approval Cycle, Delayed Response). You will upload this to Azure Blob Storage in Challenge 1 and import it into Dynamics 365 in Challenge 2.
   - **`accounts.csv`** — the 20 company (Account) records that correspond to the opportunities. You will import this into Dynamics 365 in Challenge 2 **before** importing the opportunities file, so that the Potential Customer lookup field resolves correctly.

   Save both extracted files to your Desktop or Downloads folder.

---

## Setup Copilot studio

1. Open a new browser tab and navigate to the Power Platform admin center by entering the following URL:

   ```
   https://admin.powerplatform.microsoft.com
   ```
   
1. In the **Power Platform admin center**, select **Manage (1)**, choose **Environments (2)**, and then click **ODL_User <inject key="DeploymentID" enableCopy="false"/>'s Environment (3)**.

   ![](./media/uppowadminimg1.png)

1. In the environment page, click on **See all** under **S2S apps**.

   ![](./media/pro-activ-gg-g3.png)

   > <span style="color:red"><strong>Important:</strong> Check whether <code>https://sandboxailabs1001.onmicrosoft.com/cloudlabs.ai</code> is already added. If either one is present, <strong>skip to Step 12</strong>. Otherwise, proceed with the steps below.</span>

   ![](./media/powerplat.png)

1. In the next pane, click on **+ New app user**.

   ![](./media/uppowadminimg3.png)

1. In the create a new app user pane, under **App**, click on **+ Add an app**.

   ![](./media/pro-activ-gg-g4.png)

1. In the **Add an app from Microsoft Entra ID** pane, enter `https://sandboxailabs1001.onmicrosoft.com/cloudlabs.ai` in the search box **(1)**, select whichever app is available from the results **(2)**, and then click **Add (3)**.

   ![](./media/pro-activ-gg-g5.png)

   > <span style="color:red"><strong>Important:</strong> If you cannot find the app in the search results, it is likely that it has already been added. Return to the <strong>Step 3</strong> and verify whether the app is listed. If it is present, skip to <strong>Step 12</strong>.</span>

1. Under **Business unit**, select the available business unit from the list **(2)**.

   ![](./media/pro-activ-gg-g6.png)

1. Beside **Security roles** click on **Edit** icon.

   ![](./media/pro-activ-gg-g7.png)

1. In the **Sync Permissions** pane, select **System Administrator (1)**, and then click **Save (2)**.

   ![](./media/pro-activ-gg-g8.png)

1. In the pop-up window, select **save**.

   ![](./media/pro-activ-gg-g9.png)

1. Review all the details and click on **Create**.

   ![](./media/pro-activ-gg-g10.png)

1. Navigate to **Microsoft Copilot Studio** by opening a new browser tab and entering the following URL:

   ```
   https://copilotstudio.microsoft.com
   ```

1. On the **Welcome to Microsoft Copilot Studio** screen, keep the default **country/region** selection and click **Get Started** to continue.

   ![](./media/pro-activ-gg-g11.png)

1. If the **Welcome to Copilot Studio!** pop-up appears, click **Skip** to continue to the main dashboard.

   ![](./media/gs-travel-g3.png)

1. If the **We've updated you to the latest version of Microsoft Copilot Studio** pop-up appears, click **Got it!**.

   ![](./media/pro-activ-gg-g12.png)

1. If the **What's new in Copilot Studio** pop-up appears, click the **Close (X)** icon to dismiss it.

   ![](./media/pro-activ-gg-g13.png)

1. In Copilot Studio, open the environment picker **(1)**, expand **Supported environments (2)**, and select **ODL_User <inject key="Deployment ID" enableCopy="false"></inject>'s Environment (3)** to switch.

   ![](./media/ex1-travel-g6.png)

Click **Next** at the bottom of the page to proceed to the next page.

## Happy Hacking!!