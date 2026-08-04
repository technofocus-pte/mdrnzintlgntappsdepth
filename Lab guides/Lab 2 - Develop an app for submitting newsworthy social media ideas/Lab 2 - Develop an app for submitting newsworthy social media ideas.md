---
lab:
  title: Lab 2 - Develop an app for submitting newsworthy social media ideas
  description: +++Make an app to have employees submit newsworthy social media ideas to the marketing department+++
  duration: 112 minutes
  level: 100
  islab: true
---

# **Lab 2 - Develop an app for submitting newsworthy social media ideas**

**Objective**: In this lab, you will learn to use Copilot to create a
Power Apps canvas app that enables employees to submit newsworthy social
media ideas. You will learn how to generate an app from a
natural-language prompt, customize Dataverse tables and fields, and
configure a form to collect and manage idea submissions.

## **Exercise 1 - Create a canvas app with AI capabilities**

### **Task 1 - Create a canvas app with Copilot**

In this task, you describe the app's purpose to Copilot. Based on your
input, Copilot generates a draft application.

**Note**: This exercise includes steps to use Copilot to create an app
with you. Keep in mind that as Copilot matures, your results might be
similar but not identical. Prompt outcomes can vary. Try alternate
prompts to get the desired outcomes. Certain product features may have
moved to different locations, and behaviors may have changed due to
continuous product evolution. Use your best judgment in such instances.
This exercise shows you the general concepts to follow as you build your
own apps with an agent.

1.  Sign in to Power Apps at +++https://make.powerapps.com/+++ with your
    Office 365 tenant credentials.

2.  Ensure that you are in your developer environment - **Dev One**. If
    not, click on the environment selector and select **Dev One**.

     ![](./media/image1.png)

3.  Select **Apps** from the left navigation pane.

     ![](./media/image2.png)

4.  On the **+ New app** screen, select **Start with Copilot**.

     ![](./media/image3.png)

5.  Enter the following text in the text box and then select the
    **Generate** button:

     +++Make an app to have employees submit newsworthy social media ideas to the marketing department+++

     ![](./media/image4.png)

6.  Copilot shows you a preview of the tables and relationships it
    creates, including relevant sample data. Review the tables to ensure
    they include the expected information, such as appropriate column
    names, correct data types, and meaningful relationships between
    tables.

     ![](./media/image5.png)

7.  Select the **Employee Social Media Idea** table and then select
    **View data**.

     ![](./media/image6.png)

8.  If a **Status** column isn’t created, enter the given prompt in the
    Copilot pane and select the **send** button.

     +++Add a Status column in the Employee Social Media Idea table+++

     ![](./media/image7.png)

9.  Check whether the **Status** was created.

     ![](./media/image8.png)

10. Check whether **Status** was created as a dropdown or text field.
    Select the dropdown next to the **Status** column header, then
    select **Edit column**. You can also identify the column type by its
    icon.

     ![](./media/image9.png)

     ![](./media/image10.png)

11. If **Status** is a text column, enter +++Convert the status column to Choice datatype+++ to convert it to a choice column.

12. Select **Cancel** to close the **Column properties** screen.

     ![](./media/image11.png)

13. Enter the given prompt and then select the **send** button.

     +++Add three new Choice data type columns named Social Content Type, Level of Effort, and Impact+++
    
     ![](./media/image12.png)

14. Check that all the 3 columns are created and have a **Choice** data type.

     ![](./media/image13.png)

15. Close the **Copilot** pane.

     ![](./media/image14.png)

16. Select **Save and open app**.

     ![](./media/image15.png)

17. In the ‘**Done working**’ pop-up, select **Save and open app**.

     ![](./media/image16.png)

18. Select **Skip** in the **Welcome to Power Apps Studio** pop-up window.

     ![](./media/image17.png)

19. You can see the **Welcome** screen of the app.

     ![](./media/image18.png)

20. Close the **Copilot** pane.

     ![](./media/image19.png)

21. Select the **Data** tab from the left navigation pane.

     ![](./media/image20.png)

22. From the **Employee Social Media Ideas** table, select **More actions** > **Edit data**.

     ![](./media/image21.png)

23. Select **New column**.

     ![](./media/image22.png)

24. Enter +++Content URL+++ for **Display name**, choose **Single line of
    text** as the **Data type**, select **URL** for **Format**, and select **Save**.

     ![](./media/image23.png)

25. Select **Close**.

     ![](./media/image24.png)

26. Refresh the data source by selecting the ellipsis next to the source and choosing **Refresh**.

     ![](./media/image25.png)

27. Select the **Tree view**.

     ![](./media/image26.png)

28. Select the **Employee Social Media Ideas** screen from the **Tree view**.

     ![](./media/image27.png)

29. Select **Form 2**. Use the given path - **Employee Social Media Ideas** screen > **ScreenContainer2** > **BodyContainer2** > **RightContainer2** > **MainContainer2** > **Form2**.

     ![](./media/image28.png)

30. Open the **Properties** pane by selecting the **Properties icon**
    from the horizontal bar.

     ![](./media/image29.png)

31. Add the new column to the form: select **Form2** (if not selected),
    in the **Properties** pane, select **9 selected** (number may vary)
    next to **Fields**.

     ![](./media/image30.png)

32. Select **Add field**.

     ![](./media/image31.png)

33. Choose **Content URL**, then select **Add**.

     ![](./media/image32.png)

34. Close the **Fields** pane.

     ![](./media/image33.png)

35. The **Content URL** field should now appear.

     ![](./media/image34.png)

36. Select **Save**.

     ![](./media/image35.png)

37. Enter +++Newsworthy Social Media Ideas+++ as the name of the app. Select the **Save** button to save your application.

     ![](./media/image36.png)

### **Task 2 - Test the application**

1.  Select the **play** button.

     ![](./media/image37.png)

2.  Select **+New**.

     ![](./media/image38.png)

3.  Fill out the form using the information given below.

     **Marketing Department:** Content
    
     **Idea Description:** Video that will compare our old products to the new.
    
     **Impact:** Moderate
    
     **Level of Effort:** Medium
    
     **Social Content Type:** Video
    
     **Status:** Pending
    
     **Idea Title:** Instagram video
    
     **Content URL:** www.bing.com
    
     ![](./media/image39.png)

4.  Select **Save** (check mark). The new item should be displayed.

     ![](./media/image40.png)

5.  Close the preview and the app designer when finished.

     ![](./media/image41.png)

6.  Select **Ok** in the ‘**Did you know**’ pop-up window.

     ![](./media/image42.png)

7.  Select **Back** from the left corner of the portal.

     ![](./media/image43.png)

8.  Select **Leave**.

     ![](./media/image44.png)

9.  Select **Tables** from the left navigation pane.

     ![](./media/image45.png)

10. Scroll down and click on the **Employee Social Media Ideas** table.

     ![](./media/image46.png)

11. You can see the new entry added while testing the app.

     ![](./media/image47.png)

 **Summary:** In this lab, you learnt how Copilot can accelerate canvas
 app development in Power Apps through natural language interaction.
 You built an app for submitting social media ideas by generating the
 app structure and underlying Dataverse tables using Copilot, enhancing
 the data model with additional choice and URL columns, and customizing
 the app form.
