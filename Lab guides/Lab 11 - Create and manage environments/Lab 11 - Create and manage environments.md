# **Lab 11: Create and manage an environment using Power Platform Admin Center**

**Objective:** In this lab, you will learn how to control who can create
and manage environments, enable or disable Administration mode in the
Power Platform Admin Center, create a custom security role, and assign
it to an administrative user.

## **Exercise 1: Control environment creation in the Power Platform Admin Center**

### **Task 1: Setting an environment refresh Cadence**

You can indicate how often you would prefer an environment to receive
updates and features from certain Microsoft Power Platform services. You
have two options to choose from after creating an environment.

**Service -** Canvas app authoring

**Frequent** - Get access to the latest updates and newest features
multiple times a month

**Moderate** - Get access to updates and features at least once a month

To set refresh cadence:

1.  Browse to the Power Platform admin center
    at +++https://admin.powerplatform.microsoft.com+++ and
    sign in with your Office 365 tenant credentials. 

2.  From the left navigation pane, select **Manage** > **Environments**
    and then click on the **Dev One** environment.

     ![](./media/image1.png)

3.  Click on **Edit** in the details section.

     ![](./media/image2.png)

4.  Under **Refresh cadence**, choose the **cadence** type –
    **Frequent,** and then click on the **Save** button.

     ![](./media/image3.png)

     **Note:**
    
    - By default, environments are automatically in
      the **frequent** cadence; creating and editing canvas apps will
      receive updates once a week. When apps are published, they will
      receive the corresponding runtime version.
    
    - If you've chosen the **moderate** cadence for the environment, all
      creating and editing of canvas apps will receive updates once a month.
      When apps are published, they will receive the corresponding runtime
      version.

### **Task 2: Control who can create and manage environments in the Power Platform admin center**

1.  Select the **Gear** icon in the upper-right corner of
    the **Microsoft Power Platform** site.

     ![](./media/image4.png)

2.  Select **Power Platform settings**.

     ![](./media/image5.png)

3.  Select **Add-on capacity assignments.** 

     ![](./media/image6.png)

4.  Select **Only specific admins** and click **Save.**

     ![](./media/image7.png)

### **Task 3: Administration mode**

You can set a sandbox, production, or trial (subscription-based)
environment in administration mode so that only users with System
Administrator or System Customizer security roles will be able to sign
in to that environment. Administration mode is useful when you want to
make operational changes and not have regular users affect your work,
and not have your work affect end users (non-admins)

1.  From the left-side menu, select **Manage** > **Environments**, and
    then select your **Dev One** environment.

    ![](./media/image1.png)

2.  On the **Details** page, click on **Edit**.

     ![](./media/image2.png)

3.  Under **Administration mode**, toggle **Disabled** to **Enabled**
    and then select **Save**.

     ![](./media/image8.png)

     ![](./media/image9.png)

4.  On the **Details** page, click on **Edit**. **Disable**
    Administrative mode and **save** it.

     ![](./media/image10.png)

## **Exercise 2: Create a new custom security role**

### **Task 1 - Create a new custom security role that only has access to the "Security Role" table**

1.  Open a new tab and navigate
    to +++https://make.powerapps.com+++ If
    required, sign in with your Office 365 tenant credentials.

2.  Select your **Dev One** environment.

     ![](./media/image11.png)

3.  Select your environment and click on **Settings** \> **Advanced
    Settings**.

     ![](./media/image12.png)

4.  In the upper-right corner of the screen,
    select **Settings** > **Personalization Settings**.

     ![](./media/image13.png)

5.  In the **General** tab, scroll down to the bottom and select
    the **user information** link.

     ![](./media/image14.png)

6.  On the user information page, select the different tabs, such
    as **Summary**, **Details**, or **Administration**, to see details
    about your profile.

     ![](./media/image15.png)

7.  Go back to the **Power Platform admin center** tab. From the
    left-side menu, select **Manage** > **Environments**, and then
    select your **Dev One** environment.

     ![](./media/image1.png)

8.  Select **Settings**.

     ![](./media/image16.png)

9.  Click on **Users + permissions > Security roles.**

     ![](./media/image17.png)

10. Click on **New role.**

     ![](./media/image18.png)

11. In the **Role Name** field, enter a name for the new role -
    **Security update**. In the **Business unit** field, select the
    business unit the role belongs to. Select **Save**.

    ![](./media/image19.png)

12. Scroll down to the **Table** list and set the **Security
    Role** table privileges as follows. Click on the **Save and
    Close** button.

     **Create**: Business Unit
    
     **Read**: Organization
    
     **Write**: Business Unit
    
     **Delete**: Business Unit
    
     **Append**: Business Unit
    
     **Append** **To**: Business Unit
    
     **Assign**: Business Unit
    
     ![](./media/image20.png)

### **Task 2: Assign the new security role to an administrative user**

1.  Click on **Settings** on the top navigation pane.

     ![](./media/image21.png)

2.  Select **Users + permissions - > Users**.

     ![](./media/image22.png)

3.  Select an administrative user - **MOD Administrator** and then
    choose **Manage Security roles**.

     ![](./media/image23.png)

4.  Select the new security role – **Security update** which was created
    above, and then **Save** it.

     ![](./media/image24.png)

5.  Click on **Save** to confirm the role assignment.

     ![](./media/image25.png)

**Summary:** In this lab, you learnt how to restrict environment
creation and management to admins from the Power Platform Admin Center.
You also learnt how to create security roles, give the privileges, and
assign them to an administrative user.
