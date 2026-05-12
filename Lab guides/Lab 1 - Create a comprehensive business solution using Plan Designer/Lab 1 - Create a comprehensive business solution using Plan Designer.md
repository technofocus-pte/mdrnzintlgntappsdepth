# **Lab 1: Create a comprehensive business solution using Plan Designer**

**Objective**: In this lab, you will use Copilot in Power Apps to design
and implement a real estate solution. You will create a structured plan
that defines business requirements, processes, data tables, and
technology components, and then generate a canvas app that surfaces and
manages real estate showings.

**Note:** This lab includes steps to create a plan, which is a
Copilot‑first development tool. Your results may be similar but not
identical, as Copilot’s outputs can vary. In that case, use this lab as
a reference or guideline. For example, if this lab works with a step
called “Showing table”, but your generated plan does not include that
exact item, look for a similar step or equivalent action.

## **Exercise 1: Create a plan**

1.  Sign in to Power Apps at +++https://make.powerapps.com/+++ with your
    Office 365 tenant credentials.

2.  Ensure that you are in your developer environment - **Dev One**. If
    not, click on the environment selector and select **Dev One**.

     ![](./media/image1.png)

3.  From the left navigation pane, select **Plans**.

     ![](./media/image2.png)

4.  Select **Create a plan**.

     ![](./media/image3.png)

5.  Enter the given prompt in the text box and then select **Generate**.

     **Prompt**: +++Create a plan to manage real estate showings+++
    
     ![](./media/image4.png)

6.  Copilot opens the plan and analyzes your business scenario based on
    the description.

     ![](./media/image5.png)

7.  From the top-right corner of the screen, select the **drop-down**
    menu (View all) of the agents list to view the presence status of
    all collaborators, including plan agents.

     ![](./media/image6.png)

8.  When a plan starts, the **Requirements Agent** identifies user needs
    based on your description. Review the user roles and needs.
    Select **"Looks good "** to move to the next step and generate a
    data model.

     ![](./media/image7.png)

9.  The processing agent has generated a set of processes. Here, the
    processing agent has generated the **Schedule and Manage Property
    Showings** and Review and **Improve Property Based on Showing
    Feedback** processes. In your case, the process name can differ.

     ![](./media/image8.png)

10. Select **Looks good** to proceed to the next step and generate data
    tables.

     ![](./media/image9.png)

11. Next, the **Data Agent** suggests tables to store your business
    data.

     ![](./media/image10.png)

12. Select **Edit** and use Copilot to describe what you want to change
    or add.

     ![](./media/image11.png)

13. Select **Show details** to view the data in a diagram and edit it.
    It opens the data workspace.

     ![](./media/image12.png)

14. You can see all the tables in the data workspace. 

     ![](./media/image13.png)

15. Select the **Showing** table (here select Property Showing), then
    select **View data** from the top bar.

     ![](./media/image14.png)

16. You can see the data stored in your table.

     ![](./media/image15.png)

17. Check if you have the **Status** column in the **Showing** table
    (here, Property Showing table).

     ![](./media/image16.png)

18. If you have the Status column in the Showing table, but it has the
    choices listed as – Scheduled, completed, or cancelled, then use the
    given prompt to change the options. Select the **Submit** icon.

     **Prompt**: +++Update the Status column to use the following choices: Pending, Completed, Confirmed, and Cancelled.+++
    
     ![](./media/image17.png)

19. You can see that the choices are now updated.

     ![](./media/image18.png)

20. If you don’t have a Status column, then use the given prompt to
    create it.

     **Prompt**: +++Add a column named Status of type Choice with the options Pending, Completed, Confirmed, and Cancelled.+++

21. Select **Back**.

> ![](./media/image19.png)

22. When you're ready to generate the technology proposal,
    select **Looks good** to continue.

     ![](./media/image20.png)

23. The **Solution Agent** analyzes the plan and proposes technologies
    tailored to solve your business problem.

     ![](./media/image21.png)

24. Select **Looks good** to accept the proposed technologies.

     ![](./media/image22.png)

25. Select the **Save** icon to save the solution.

     ![](./media/image23.png)

26. Keep the selection as is under the **Select an existing solution**
    option and then select **Save**.

     ![](./media/image24.png)

27. Do not navigate from the current window.

## **Exercise 2: Create a canvas app**

### **Task 1: Create a canvas app for a real estate solution**

1.  Under the **Technology** section, hover over the Canvas app (here,
    the name of the Canvas app is Showing Organizer) and then select the
    **+ icon** to create the app.

     ![](./media/image25.png)

2.  You will now navigate to the Power Apps designer. Select **Skip** on
    the **Welcome to Power Apps Studio** pop-up.

     ![](./media/image26.png)

3.  From the left navigation pane, click the **Property Showings** screen.

     ![](./media/image27.png)

4.  Expand the **Property Showings** screen.

     ![](./media/image28.png)

5.  Select the **Record gallery** from the left navigation pane. On the canvas, select the **edit** icon. **Property Showings** screen > **ScreenContainer4** > **BodyContainer4** > **SidebarContainer4** > **RecordsGallery4**.

     ![](./media/image29.png)

6.  Select **Layout** > **Title and subtitle**.

     ![](./media/image30.png)

7.  Select the recently added **Subtitle**.

     ![](./media/image31.png)

8.  In the formula bar, set the **Text** value to the given formula. Enter +++ThisItem.Status+++ and then select **ThisItem.’Status (crc5b_status)’** from the suggestions. Note that the **crc5b** value is different in your case.

     ![](./media/image32.png)

9.  You can now see that the **Text** property for the **Subtitle** is
    updated.

     ![](./media/image33.png)

10. Select **Save**.

     ![](./media/image34.png)

### **Task 2: Test the app**

1.  Make a new request for a property that shows in the app by selecting
    the **Play** button from the top bar of the screen.

     ![](./media/image35.png)

2.  Check if + New option is visible. If not, then close the testing
    window by selecting the **X** in the upper-right corner.

     ![](./media/image36.png)

3.  In the left pane, select the **+ New** button.

     ![](./media/image37.png)

4.  Select the **Properties** icon from the horizontal menu to open the
    **Properties** pane. Select **RecordsGallery4**, and then set the
    **Flexible height** toggle to **On**.

     ![](./media/image38.png)

5.  Now, select the **Play** button.

     ![](./media/image39.png)

6.  To change the app window size, expand the **Browser** option, and
    then select **Canvas size**.

     ![](./media/image40.png)

7.  Fill in the fields with the following information. Select the check
    mark in the upper-right corner of the screen.

     **Showing Title:** +++Show 7+++

     **Duration Hours:** 1
    
     **Showing DateTime:** Any future data
    
     **Status:** Confirmed (You can select any from the drop-down list)
    
     **Property:** 123 Maple St (You can choose any from the drop-down list)
    
     **Buyer:** Daniel Martinez
    
     **Agent:** John Smith (You can choose any from the drop-down list)
    
     **Client:** Jessica Lee (You can choose any from the drop-down list)
    
     ![](./media/image41.png)

8.  Select the **X** in the upper-right corner to close out of the app.

     ![](./media/image36.png)

9.  If a dialog appears saying, **Did you know?**, select **OK**.

    ![](./media/image42.png)

10. Select the **Save** button to save the new app that you created.

     ![](./media/image43.png)

11. Exit the app to return to the Power Apps home page.

 **Summary**: In this lab, you learnt to build a real estate showing
 management solution. You created a plan in the Power Apps portal,
 where Copilot analyzes a business prompt to identify user roles,
> processes, and data requirements. You learnt to review and refine the
> generated data model, including validating and updating table columns
> such as the Status choice field in the Showing table, and created a
> canvas app directly from the generated plan.
