# **Lab 4 - Add an agent to a model-driven app and supervise it with Agent feed (preview)**

**Objective**: In this lab, you will learn to create an AI-powered claim
management solution by using Copilot to design a business plan, generate
a model-driven app, and configure an autonomous agent to review
reimbursement claims. You will also learn how to supervise and monitor
agent actions using the Agent feed in Power Apps.

## **Exercise 1: Create a plan**

1.  Sign in to Power Apps at **https://make.powerapps.com/** with your
    Office 365 tenant credentials.

2.  Ensure that you are in your developer environment - **Dev One**. If
    not, click on the environment selector and select **Dev One**.

     ![](./media/image1.png)

3.  From the left navigation pane, select **Plans**.

     ![](./media/image2.png)

4.  Select **Create a plan**.

     ![](./media/image3.png)

5.  Enter the given prompt in the text box and then select **Generate**.


     **Prompt**: +++I need to manage reimbursement claims in a simple way. Employees can submit reimbursement claims for eligible personal travel expenses incurred in line with company policies.+++
      ```
     Requirements:

    - A single app for managing reimbursement claims.
    
    - Employees submit personal travel reimbursement claims.
    
    - A manager or reviewer can view submitted claims and approve or reject
      them based on company travel reimbursement guidelines.

     An AI agent should automatically review submitted travel claims and provide a recommendation (approve or reject) according to the guidelines
      
     ```
        
  ![](./media/image4.png)

5.  Copilot opens the plan and analyzes your business scenario based on
    the description.

     ![](./media/image5.png)

6.  When a plan starts, the **Requirements Agent** identifies user needs
    based on your description. Review the user roles and needs.
    Select **"Looks good "** to move to the next step and generate a
    data model.

     ![](./media/image6.png)

7.  The processing agent has generated a set of processes. Here, the
    processing agent has generated the **Travel Reimbursement Claim
    Submission and Review** process. In your case, the process name can
    differ. Select **Looks good** to proceed to the next step and
    generate data tables.

     ![](./media/image7.png)

8.  Next, the **Data Agent** suggests tables to store your business
    data.

     ![](./media/image8.png)

9. Select **Show details** to view the data in a diagram and edit it.
    It opens the data workspace.

     ![](./media/image9.png)

10. You can see all the tables in the data workspace. 

     ![](./media/image10.png)

11. Remove all other tables except the **Reimbursement Claim** table. To remove a table, click on the **(…) View options** and then select **Remove**.

     ![](./media/image11.png)

12. Select **Remove**.

     ![](./media/image12.png)
    
     ![](./media/image13.png)

13. Select the **Reimbursement Claim** table, then select **View data** from the top bar.

     ![](./media/image14.png)

14. You can see the data stored in your table.

     ![](./media/image15.png)

15. Check if you have the **Status** column in the **Reimbursement Claim** table.

     ![](./media/image16.png)

16. If you don’t see the **Status** column in the **Reimbursement
    Claim** table, then enter the below prompt to add it to the table.

     **Prompt**: +++Add column for Status+++

17. To add one more column to the table, enter the given prompt and
    select the send icon.

     **Prompt**: +++Add column for Expense Category+++
    
     ![](./media/image17.png)

18. Check that Copilot has generated the column.

     ![](./media/image18.png)

19. Click on the drop-down menu of the **Status** column and select
    **Edit** column.

     ![](./media/image19.png)

20. Remove all other options. To do this, select the **ellipsis (…)** next to the option you want to remove (for example, **Under Review**), and then select **Remove**.

     ![](./media/image20.png)

21. In the **Default choice** field, select **Submitted** from the drop-down.

     ![](./media/image21.png)

22. The table with sample data is ready. Click **<-** **Back**.

     ![](./media/image22.png)

23. Select **Looks good** to continue.

     ![](./media/image23.png)

24. The **Solution Agent** analyzes the plan and proposes technologies
    tailored to solve your business problem.

     ![](./media/image24.png)

25. Check if the Solution agent has generated a Model-driven app? If
    not, then select **Edit**.

     ![](./media/image25.png)

26. Enter the given prompt in the text box. Click **send**.

     **Prompt:** +++Create a Claim Management Hub Model-driven app.+++
    
     ![](./media/image26.png)

27. The solution agent has generated the Model-driven app. Select **Keep**.

     ![](./media/image27.png)

28. Select **Looks good** to accept the technologies.

     ![](./media/image28.png)

29. Select the **Save** icon to save the solution.

     ![](./media/image29.png)

30. Keep the selection as is under the **Select an existing solution**
    option and then select **Save**.

     ![](./media/image30.png)

31. Do not navigate from the current window.

## **Exercise 2: Create a Model-driven app**

### **Task 1: Create a Model-driven app**

1.  Under the **Technology** section, hover over the Model-driven app
    (here, the name of the Canvas app is Claim Management Hub) and then
    select the **+ icon** to create the app.

     ![](./media/image31.png)

2.  The Model-driven app is created. Select the **Save and publish**
    icon.

     ![](./media/image32.png)

3.  Go back to the Plan designer. Hover over the Agent (here, the name
    of the Agent is Travel Claim Reviewer) and then select the **+
    icon** to create the agent.

     ![](./media/image33.png)

4.  You will be navigated to the Copilot Studio. Select **Skip**.

     ![](./media/image34.png)

5.  You can see that the agent has been set up. The **Reimbursement
    Claim** table has been added as a knowledge source.

     ![](./media/image35.png)

6.  Select **Edit** in the **Instructions** section.

     ![](./media/image36.png)

7.  Replace the existing instructions with the ones provided below.
    Select **Save**.

     ```
     You are responsible for reviewing employee reimbursement claims and
     assigning an approval status of Approved or Rejected.
    
     Approve the claim if the amount is less than $1,300 and the expense is
     for eligible categories such as hotels or taxis (excluding fines).
     Reject the claim if the amount is $1,300 or more.
     ```   
    
      ![](./media/image37.png)

8.  Go to the **Tools** section and select **Add tool**.

     ![](./media/image38.png)

9.  Select **Microsoft Dataverse**.

     ![](./media/image39.png)

10. Select **Update a row in selected environment**.

     ![](./media/image40.png)

11. The connection will be created. Select **Add and configure**.

     ![](./media/image41.png)

12. Hjkjl just for reference

     ![](./media/image42.png)

13. Enter +++Review the claim+++ as the agent name.

     ![](./media/image43.png)

14. Enter the given description:

     +++Review the claim based on company guidelines.+++
    
     ![](./media/image44.png)

15. Expand the **Additional details** option.

     ![](./media/image45.png)
    
     ![](./media/image46.png)

16. In the **Credentials to use** field, select **Maker-provided
    credentials** from the drop-down menu.

     ![](./media/image47.png)

17. Close the **Test pane** for a better view.

     ![](./media/image48.png)

18. In the **Input** section, for the **Environment** field, select
    **Custom value** from the drop-down list.

     ![](./media/image49.png)

19. From the **Choose an environment** drop-down list, select
    **Current**.

     ![](./media/image50.png)

20. In the Table name field, select **Custom value** from the drop-down
    list.

     ![](./media/image51.png)

21. Click in the **Choose a table** field and select **Reimbursement
    Claims** from the list.

     ![](./media/image52.png)

22. Select **+Add input** to add one more input field and then add **Status**.

     ![](./media/image53.png)

23. For the **Status** field, select **Customize**.

     ![](./media/image54.png)

24. In the **Description** field, enter the following description and 
    then select **Save**. You need to change the value number
    **137690002** to the appropriate **option value** for the
    **Approved** and **Rejected** options in your **Status** column.

     +++If approved put+++ < Enter Value number for Approved >, +++if rejected put+++ < Enter Value number for Rejected >
    
     ![](./media/image55.png)

25. From the top bar, select the **Overview** tab.

     ![](./media/image56.png)

26. In the **Instructions** section, select **Edit**.

     ![](./media/image57.png)

27. After the existing instruction, enter **Use /** and select **Review
    the claim** tool from the suggestions.

     ![](./media/image58.png)

28. Select **Save**.

     ![](./media/image59.png)

### **Task 2: Add a trigger**

1.  In the **Triggers** section, select **Add trigger**.

     ![](./media/image60.png)

2.  Select **Turn it on** in the **Add trigger** window.

     ![](./media/image61.png)

3.  Select **When a row is added, modified or deleted** trigger and then
    select **Next**.

     ![](./media/image62.png)

4.  Select **Continue**.

     ![](./media/image63.png)

5.  Ensure that the app connections are created, and then select
    **Next**.

     ![](./media/image64.png)

6.  For the **When a row is added, modified or deleted** trigger, enter
    the following details, then select **Create trigger**.

     **Change type**: Added
    
     **Table name**: Reimbursement Claims
    
     **Scope**: Organization
    
     **Additional instructions to the agent when it's invoked by this
     trigger**: Keep the existing selection
    
     ![](./media/image65.png)

7.  Select **Close**.

     ![](./media/image66.png)

8.  To test the trigger, select the recently created trigger from the
    **Triggers** section.

     ![](./media/image67.png)

9.  Select the **Sends a prompt to the specified copilot for
    processing** step.

     ![](./media/image68.png)
    
     ![](./media/image69.png)

10. In the message field, remove the existing message and enter the
    given message.

     +++Row ID:+++ Select Reimbursement Claims from the Dynamic content
    
     +++Claim Title:+++ Select Claim Title from the Dynamic content
    
     +++Claim Amount:+++ Select Claim Amount from the Dynamic content
    
     ![](./media/image70.png)

11. Select **Save**.

     ![](./media/image71.png)

12. Go back to the Copilot Studio and select **Publish**.

     ![](./media/image72.png)

13. Select **Publish**.

     ![](./media/image73.png)

### **Task 3: Test the trigger**

1.  To test the trigger, create a claim in the Model-driven app. Go to
    the Power Apps portal where the **Claim Management Hub** app is
    open. Select **+New**.

     ![](./media/image74.png)

2.  Enter the following details.

     **Claim Title**: Trip
    
     **Submission Date**: Any future date
    
     **Travel Start Date**: Any future date
    
     **Travel End Date**: Any future date
    
     **Total Amount**: 1250
    
     **Expense Category**: Hotel
    
     ![](./media/image75.png)

3.  Select **More commands** and then select **Save and Close**.

     ![](./media/image76.png)

4.  Select **Test trigger**.

     ![](./media/image77.png)

5.  Select **Start testing**.

     ![](./media/image78.png)

6.  You can see the agent’s response.

     ![](./media/image79.png)

7.  From the top menu bar, select the **Activity** tab.

     ![](./media/image80.png)

8.  See the **Complete** status.

     ![](./media/image81.png)

9.  Select **Publish**.

     ![](./media/image82.png)

## **Exercise 3: Agent feed in Power Apps**

### **Task 1: Use the Power Apps MCP server in the agent** 

1.  In the Model-driven app, select **Agents** from the left navigation
    pane.

     ![](./media/image83.png)

2.  Select more options next to Travel Claim Reviewer and then select
    **+ Add to feed**.

     ![](./media/image84.png)

3.  Open the **Travel Claim Reviewer** agent.

     ![](./media/image85.png)

4.  In the **Tools** section, select the **+ Add tool**.

     ![](./media/image86.png)

5.  Select the **Power Apps MCP server**.

     ![](./media/image87.png)

6.  Click the **Not connected** drop-down and select **Create new
    connection**.

     ![](./media/image88.png)

7.  Select **Azure AD** and select **Create**.

     ![](./media/image89.png)

8.  Select the **Mod Admin** account.

     ![](./media/image90.png)

9.  Select **Add and configure**.

     ![](./media/image91.png)

10. Go to the Power Apps portal. Select the **Claim Management Hub** app
    and then select the **Play** icon.

     ![](./media/image92.png)

11. Agent feed should appear in the left navigation pane.

     ![](./media/image93.png)

### **Task 2: Supervise agents in model-driven apps with agent feed (preview)**

1.  On the Copilot Studio, open the **Test** pane (if not), enter
    +++Review claim+++, and select the **send** icon.

     ![](./media/image94.png)

2.  Observe the agent’s response. Note that the agent uses the **Power
    Apps MCP Server** tool.

     ![](./media/image95.png)

3.  Navigate to the **Claim Management Hub** app window that we opened
    in a new window. Select **+New** to add a new claim.

     ![](./media/image96.png)

4.  Enter the following details and select **Save & Close**.

     **Claim Title**: Travel

     **Owner**: MOD Administrator

     **Submission Date**: Enter any future date

     **Total Amount**: 1200

     **Expense Category**: Hotel


     ![](./media/image97.png)

6.  In the left pane, under the Agent feed section, select the
    **Completed** tab, and you can see the output.

     ![](./media/image98.png)

7.  Create one more claim and save it.

     **Claim title**: Test
    
     ![](./media/image99.png)

8.  Refresh the page and check under the Needs attention tab, you can
    see the new entry regarding the **Test** claim.

     ![](./media/image96.png)
    
     **Summary**: In this lab, you learnt to use Copilot to build a
     model-driven app with an AI agent that reviews employee reimbursement
     claims. You learnt to configure the agent to evaluate claims based on
     business rules, trigger it using Dataverse events, and monitor its
     actions through the Agent feed in Power Apps, enabling supervised
     AI-driven decision-making.
