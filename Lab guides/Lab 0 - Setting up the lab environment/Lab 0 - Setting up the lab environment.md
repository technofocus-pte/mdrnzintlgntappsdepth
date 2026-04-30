**Lab 0: Setting up the lab environment**

**Objective:** In this lab, you will acquire a Power Apps trial license
and create a team in Microsoft Teams.

**Exercise 1: Assign a Power Apps trial license**

1.  Open a web browser on your VM and go to
    +++[**https://powerapps.microsoft.com/en-us/free/**](https://powerapps.microsoft.com/en-us/free/)+++.

> ![](./media/image1.png)

2.  Select **Start free**.

> ![A person with his arms crossed Description automatically
> generated](./media/image2.png)

3.  Enter your **Office 365 admin credentials**, check the checkbox to
    **accept the agreement,** and click on **Start free**.

> ![](./media/image3.png)

4.  Enter the **password of your Office 365 tenant ID** and then select
    **Sign in**.

> ![](./media/image4.png)

5.  Select **Yes** on **Stay signed in?** pop-up window.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image5.png)

6.  Keep the **United States** as your **country/region** and then click
    on the **Get started** button.

> ![](./media/image6.png)

7.  You can now see the **Home page of Power Apps** and the developer
    environment – **Dev One,** which has been created for you.

> ![](./media/image7.png)

8.  Open the new tab and go to the **Power Platform admin center** by
    navigating to
    [**https://admin.powerplatform.microsoft.com**](https://admin.powerplatform.microsoft.com)
    and, if required, sign in using your given Office 365 admin tenant
    credentials.

> ![](./media/image8.png)

9.  From the left navigation pane, select **Manage** \>
    **Environments,** and then you can see that **Dev One** is your
    Dataverse environment.

> ![](./media/image9.png)

**Exercise 2: Create a team in Microsoft Teams **

1.  Sign in to Microsoft Teams
    using [**https://teams.microsoft.com/**](https://teams.microsoft.com/) with
    your Office 365 tenant credentials.

2.  On the **Get to know Teams** pop-up window, select **Get Started**.

> ![](./media/image10.png)

3.  Close the window that asks for scanning the QR code.

> ![](./media/image11.png)

4.  On the left side of the app, select **Chat**.

> ![](./media/image12.png)

5.  Select **New items** from the Chat section. Select **New team**. 

> ![](./media/image13.png)

6.  Enter the Team name as **Dev Team,** First channel name as
    **DevChannel,** and click **Private**.

> ![](./media/image14.png)

7.  Select **Org-wide**.

> ![](./media/image15.png)

8.  Select **Create**.

> ![](./media/image16.png)

9.  You can now see the **Dev Team** team has been created.

> ![](./media/image17.png)

**Exercise 3: Assign a Copilot Studio trial license**

1.  Sign in to **Microsoft Copilot Studio** with your **Office 365 admin
    tenant** credentials
    using <https://go.microsoft.com/fwlink/?LinkId=2107702>**.** Select
    **Sign in** or **Continue**.

> ![](./media/image18.png)
>
> ![](./media/image19.png)

2.  Fill in the following required information and then select **Get
    Started**.

> **Country or Region** – United States
>
> **Job title** – Your job title
>
> **Business phone number** – Your phone number
>
> ![](./media/image20.png)

3.  Under the **Confirmation details** step, select **Get Started**.

> ![](./media/image21.png)

4.  Select the **United States** as your country/region and then
    select **Get** **Started**.

> ![](./media/image22.png)

5.  If you see the pop-up regarding the latest version of Copilot
    Studio, select **Got it**.

> ![](./media/image23.png)

6.  Select the **Dev One** environment from the environment selector.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image24.png)
>
> **Note**: If you're unable to select the **Dev One** environment as
> shown in the image below, then follow the steps below.
>
> ![](./media/image25.png)
>
> Open the Power Platform Admin Center using
> +++<https://admin.powerplatform.microsoft.com/+++>. From the left-hand
> menu, select **Manage**, then choose **Environments** \> **Dev One**.
> Copy the **Environment ID**, and update the Copilot Studio link
> accordingly, as shown in the image below.
>
> ![image](./media/image26.png)
>
> Navigate back to the Copilot Studio tab and open
> +++<https://copilotstudio.microsoft.com/environments/>**\<
> EnvironmentID \>**/home+++ (Replacing **\< EnvironmentID \>** with the
> value fetched above)
>
> ![](./media/image27.png)

7.  On the **Welcome to Copilot Studio** pop-up, select **Skip.**

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image28.png)

## **Exercise 4: Create a Security group and assign the Bot author role** **to MOD Administrator**

1.  Open a web browser on your VM and go to the Azure portal using
    +++https://portal.azure.com/+++. Sign in with the given **Office 365
    admin credentials.** Complete the authentication process.

2.  Select **Next** on the Let’s keep your account secure pop-up window.

> ![](./media/image29.png)

3.  Select **Next** on the Install Microsoft Authenticator pop-up
    window.

> ![](./media/image30.png)

4.  Select **Next** to set up your account in app.

> ![](./media/image31.png)

5.  Scan the QR code and then select **Next**.

> ![](./media/image32.png)

6.  Enter the number that appears on your screen into the Authenticator
    app.

> ![](./media/image33.png)

7.  Select **Done**.

> ![](./media/image34.png)

8.  On the Microsoft Azure portal, in the search bar, enter +++Microsoft
    Entra+++ and select **Microsoft Entra ID** from the suggestions.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image35.png)

9.  From the left navigation pane, expand **Manage** and then select
    **Groups**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image36.png)

10. Select **New group**.

> ![](./media/image37.png)

11. On the **New Group** page, provide the following information.

> Group type: Security
>
> Name: Agentgrp
>
> ![](./media/image38.png)

12. To select owners, click on the **" No owners selected**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image38.png)

13. **Check** the **checkbox** of **MOD Administrator** and then click
    on the **Select** button.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image39.png)

14. To select members, click on the **no members selected**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image40.png)

15. **Check** the **checkbox** of **MOD Administrator** and then click
    on the **Select** button.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image41.png)

16. Select **Create**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image42.png)

17. Navigate to Power Platform admin center. From the left navigation
    pane, select the **Manage** tab. Then select **Tenant settings**. In
    the search box, enter +++Copilot Studio+++ and then select **Copilot
    Studio authors**.

> ![](./media/image43.png)

18. Click on the **Edit** icon (pencil) next to the **None** option.

> ![](./media/image44.png)

19. Select **Agentgrp** and then click on the **Done** button.

> ![](./media/image45.png)

20. Select **Save**.

> ![](./media/image46.png)

21. From the left navigation pane, select **Manage** \> **Environments**
    and then click on the **Dev One** environment.

> ![](./media/image47.png)

22. In the **Access** section, click on the **See all** below the
    **Users** option.

> ![](./media/image48.png)

23. Select **MOD Administrator.**

> ![](./media/image49.png)

24. Select **Manage roles**.

> ![](./media/image50.png)

25. Select the **Bot author** role and then click on the **Save**
    button.

> ![](./media/image51.png)

26. Select **Save** again to confirm the selection.

> ![](./media/image52.png)

27. Close the window.

> ![](./media/image53.png)

**Summary**: In this lab, you acquired Power Apps trial license and
created a team in Microsoft Teams. You also created a security group and
assigned a Bot author role to MOD Administrator.
