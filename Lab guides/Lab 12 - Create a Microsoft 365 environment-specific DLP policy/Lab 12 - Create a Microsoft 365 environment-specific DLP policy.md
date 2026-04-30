# **Lab 12 - Create a Microsoft 365 environment-specific Data Loss Prevention policy**

**Exercise 1: Control user access to environments: security groups and
licenses**

**Task 1: Create Microsoft 365 Users**

1.  Navigate to the Microsoft 365 admin center using
    +++[*https://admin.microsoft.com+++*](https://admin.microsoft.com+++/)

2.  From the left navigation, select **Users** \> **Active users** page,
    and click **Add a user**.

> ![](./media/image1.png)

3.  On the Set up the basics pane, enter the given details.

> **First name**: Brooke
>
> **Last name**: Gray
>
> **Display name**: Brooke Gray
>
> **Username**: brookeg
>
> ![](./media/image2.png)

4.  To reset the password for all the user, uncheck all check boxes and
    enter password as: +++Pa$$w0rd@124+++ and then click on **Next**.

> ![](./media/image3.png)

5.  On the **Assign product licenses** pane, select all the license
    check boxes and click **Next**.

> ![](./media/image4.png)

6.  On the **Optional settings** pane, select **Next**.

> ![](./media/image5.png)

7.  On the **Review and finish** pane, click **Finish adding**.

> ![](./media/image6.png)

8.  Select **Close**.

> ![](./media/image7.png)

**Task 2: Create a security group and add members to the security
group**

1.  Open a new tab in the same browser and navigate to the **Microsoft
    365 admin
    center** using [**https://admin.microsoft.com**](urn:gd:lg:a:send-vm-keys).
    Sign in with your Office 365 tenant credentials.

2.  Select **Teams & groups** \> **Active teams & groups**.

> ![](./media/image8.png)

3.  Select the **Security group** tab and then select **+Add a security
    group**.

> ![](./media/image9.png)

4.  Add the group Name: +++[**PPS-security**+++
    and** Description:**](urn:gd:lg:a:send-vm-keys) +++Power Platform
    security group+++ and then click **Next**.

> ![](./media/image10.png)

5.  Click on the **Create group** button.

> ![](./media/image11.png)

6.  Click on the **Close** button to close the window.

> ![](./media/image12.png)

7.  Select the **PPS-security** group you created.

> ![](./media/image13.png)

8.  Select the **Members** tab and then click on **View all and the
    managed members** hyperlink.

> ![](./media/image14.png)

9.  Click on **+ Add members**.

> ![](./media/image15.png)

10. Select the users (For example, here, Brooke) to add to the security
    group and then select **Add(1).**

> ![](./media/image16.png)

11. **Close** the ‘Members’ pane to return to the **Groups** list.

> ![](./media/image17.png)

12. You have completed this task. Please do not close the tab and
    proceed with the next task.

**Task 3: Associate a security group with a Dataverse environment**

1.  Open a new tab and navigate to the Power Platform admin center
    using [**https://admin.powerplatform.microsoft.com**](urn:gd:lg:a:send-vm-keys) and
    if required, sign in with your Office 365 tenant credentials. 

2.  In the navigation pane, select **Manage \>** **Environments**, and
    then select **+New**.

> ![](./media/image18.png)

3.  On the New environment window, enter the following information.

**Type**: Trial

> **Region**: United States – Default
>
> **Name:** Test
>
> ![](./media/image19.png)

4.  Expand the **Change default settings** option and toggle the **Add a
    Dataverse data store** button to **Yes**. Select **Next**.

> ![](./media/image20.png)

5.  Keep the **Language** as **English (United States)**, **Currency**
    as **USD** and then click on **+** **Select**.

> ![](./media/image21.png)

6.  Under the **Restricted access**, select **PPS-Security** and then
    select **Done**.

> ![](./media/image22.png)

7.  You can see under the Security group, the **PPS-security** group is
    added and then select **Save**.

> ![](./media/image23.png)

**Exercise 2: Configure DLP to block Power Platform connectors in the
Power Platform admin center**

**Task 1: Create a policy**

1.  Navigate to Power Platform admin center
    using [**https://admin.powerplatform.microsoft.com**](urn:gd:lg:a:send-vm-keys) and
    if required, sign in with your Office 365 tenant credentials. 

2.  From the left navigation pane, select **Security**.
    Under **Security**, select **Data and privacy,** then select the
    **Data policy** tile.

> ![](./media/image24.png)

3.  To create a new policy, select **+New policy**.

> ![](./media/image25.png)

4.  Enter the name of the policy **-** +++**PP-Connector Policy**+++ and
    click **Next**.

> ![](./media/image26.png)

1.  Search for **Dataverse**, select **Microsoft Dataverse**, and
    click **Move to Business**.  Choose carefully, you may have to
    expand the Name column to differentiate between connectors in your
    search results.

> ![](./media/image27.png)

2.  Search for **SharePoint**, select **SharePoint,** and click **Move
    to Business**.

> ![](./media/image28.png)

3.  Search for **Outlook**, select **Office 365 Outlook,** and
    click **Move to Business**.

> ![](./media/image29.png)

4.  Select the **Business** tab and you should now have three connectors
    moved to Business. Click **Next**.

> ![](./media/image30.png)

5.  Do not add any connectors and click **Next**.

> ![](./media/image31.png)

6.  On the **Define Scope**, select **Add multiple environments** and
    then click **Next.**

> ![](./media/image32.png)

7.  Select your **Test** trial environment and then select **+Add to
    policy**.

> ![](./media/image33.png)

8.  Select **Added to policy** tab and then click **Next**.

> ![](./media/image34.png)

9.  **Review** the policy and then select **Create policy**.

> ![](./media/image35.png)

10. Your **Policy** has been created.

> ![](./media/image36.png)

### **Task 2: Create a flow to get the weather**

1.  Switch back to the **Power Apps maker
    portal** [**https://make.powerapps.com**](urn:gd:lg:a:send-vm-keys) tab
    and make sure you have signed in with your Office 365 tenant
    credentials. 

2.  Select the trial environment – **Test** from the environment
    selector.

> ![](./media/image37.png)

3.  Select **Flows** from the left. Click **+ New** **flow** and
    select **Instant cloud flow.**

> ![](./media/image38.png)

4.  Provide a **Flow name** of **Weather flow**, select **Manually
    trigger a flow** as your trigger, and then select
    the **Create** button.

> ![](./media/image39.png)

5.  Click **+ New step**.

> ![](./media/image40.png)

6.  Search for **MSN** in the **Search connectors and actions** text
    box. Select the **Get forecast for today** action.

> ![](./media/image41.png)

7.  Provide your **Location - Denver**, select **Units - Imperial**, and
    click **+ New step**.

> ![](./media/image42.png)

8.  Search for **send email** and select **Send an email (V2) Office 365
    Outlook**.

> ![](./media/image43.png)

9.  Provide your email for **To** and enter **Today's
    Weather** for **Subject**.

10. Click on the Body enter +++**Today’s weather for:**+++ and
    select **Location** from the Dynamic content pane.

> ![](./media/image44.png)

11. Hit the **\[ENTER\]** key, enter +++**Temperature:**+++ and
    select **Temperature** from the Dynamic content pane.

12. Hit the **\[ENTER\]** key, enter +++**Conditions:**+++ and
    select **Conditions** from the Dynamic content pane.

13. You may add other values to the email.

> ![](./media/image45.png)

14. Select the **Save** button to save the flow. The DLP enforcement job
    will run.

> ![](./media/image46.png)

15. You should get an error as a result of violating your DLP policy
    that you created. As a result, your flow will be disabled, and it
    can't be enabled while it conflicts with any DLP policies. In this
    specific example, it's disabled because you have included an **MSN
    Weather** connector in a flow that also contains an **Office 365
    Outlook** connector. If you want this flow to run, you can either
    add the **MSN Weather** connector to the **Business data only** data
    group in your Office 365 DLP policy that you previously created, or
    you can remove the **Office 365 Outlook** connector from
    the **Business data only** data group.

> ![](./media/image47.png)
