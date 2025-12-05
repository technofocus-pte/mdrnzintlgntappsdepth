# **Lab 2: Create a canvas app from an image and add Copilot control (Preview)**

**Estimated duration**: 20 min

## **Objective**: ##
In this lab, you will learn how to create an app from a
visual design and connect it to data through a few simple, guided steps.
You will learn to customize the app and learn how to add a Copilot
control to a canvas app.    

**Note:** Copilot in Power Apps can generate different app layouts,
forms, and data connections apps.

## **Exercise 1: Create a canvas app from an image**

### **Task 1: Create an app**

1.  Sign in with your Office 365 tenant credentials to Power Apps using
    <https://make.powerapps.com/>.

2.  Ensure that you are in **Dev** **One** environment.

    ![](./media/image1.png)

3.  Select **+ Create** from the left-pane and then select **Start with
    a page design**.

    ![](./media/image2.png)

4.  Select **Image** **or Figma file**.

    ![](./media/image3.png)

5.  Ensure that **Start from an image** is selected. Review the examples
    of recommended images and tips. Once you’re done, select
    the **Next** button.

    ![](./media/image4.png)

6.  Enter a name for the app – **Membership Form**. Select **Start with
    sample image**. Select **Membership form image**. Select **Phone**
    format and then select **Next**.

    ![](./media/image5.png)

    **Note:** If you're using your own image, the image file extension
    must be .jpg or .png, and the file size must be less than 4MB. Also,
    the image must contain a clearly legible one-page form with a light
    background color. For the best results, edit your image so that it has
    a white background and high contrast.

7.  Your image will be automatically tagged based on the components that
    were identified. For example, in the following sample image, the box
    that says “Enter your first name” was identified as a **Text
    input** control. After you've reviewed the tags and ensured that
    each component is correctly tagged, select **Next**.

    **Note:** You can draw a new tag by selecting and dragging to select
    the region that encompasses the component. Then, choose the type of
    component that you want to associate the new tag with.

    To make edits to an existing tag or to delete it, select the tag. You
    can then assign a different component for that tag, or adjust the
    dimensions of the tag by dragging the corners to change the size. If
    you'd like to remove the tag, select **Delete tag**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image6.png)

    **Tip:** Select the **Guidance** tab on the right-side of the screen
    to learn more about the different types of components and how to
    accurately tag each one.

8.  The next step is to set up data. For the best experience,
    select ***Connect to a Dataverse table*** and select **Next**.
    You'll be guided in the next stage to either select an existing
    Dataverse table you have and map the fields in the image to the
    columns in that table or create a new table in Dataverse and add
    columns based on the form fields in your image, and your app will
    contain a form component that is connected to your Dataverse table.

    **Note:** The option to Connect to a Dataverse table will be disabled
    if you don't have Dataverse in your environment. If you don't want to
    connect to Dataverse, select **Skip this for now**. If you choose this
    option and select **Create**, your app will be created as-is, which
    means that the components you tagged in the previous step will be
    generated directly. They won't be placed into a form component, and
    your app won't be connected to data.
    
    ![](./media/image7.png)

9.  From the drop-down menu of the **Table name** field, choose **Create
    new table** and then select **Next**.

    ![](./media/image8.png)
    
    **Note:** Each tag corresponds to a data column based on the form
    fields that were identified in your image. You can edit the table and
    column details. Select a tag to modify the column properties, such
    as **Display Name**, **Name**, and **Data type**. To remove an
    existing column, select the tag and then select **Delete column**.

10. Select **Next**, you'll be able to review the table and column
    structure.

    **Note:** Select **Table properties** on the right-side of the screen
    to view and edit the properties for your new table.

    ![](./media/image10.png)

11. Once you've completed the review, select **Create app** to create
    the app.

    ![](./media/image11.png)
    
    **Note:** The app creation might take few minutes.

12. Once the app is created, your new app will open in Power Apps Studio
    so you can continue building and customizing your app.

13. As you have chosen to create a new table in Dataverse, your form
    will be automatically connected to your new table. To check that,
    click on the **Form1** under the **Tree view** and observe that
    under the **Properties** pane, **Membership Form** is selected as a
    **Data source**.

    ![](./media/image12.png)

14. Select **Save** icon to save the app.

    ![A screenshot of a computer Description automatically generated](./media/image13.png)

### **Task 2: Customize the app**

1.  Select **App** from the **Tree view**.

![A screenshot of a computer AI-generated content may be incorrect.](./media/image14.png)

2.  Select **Formulas** from the property selector.

![A screenshot of a computer AI-generated content may be incorrect.](./media/image15.png)

3.  Write the given formulas to store background color of text label and
    the button color into the variables.

    *BGColor = RGBA(0, 120, 212, 1);*

    *ButtonColor = RGBA(0, 120, 212, 1);*

    ![](./media/image16.png)

4.  From the **Tree view**, select **Textlabel8** under the **Screen1**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image17.png)

5.  In the Property selector, select the **Fill** property of Text
    label, delete the existing color value and enter the value –
    **BGColor**. Note that, BGColor contains the color value.

    ![](./media/image18.png)

6.  Adjust the width of Membership Form **Text label** as shown in the
    image.

    ![](./media/image19.png)

7.  Select the **Text label** and change the alignment to center. If
    **Align** option is not visible, click the ellipsis (…) icon next to
    the font type selector.

    ![](./media/image20.png)

8.  Select the **Button1 (Select response)** on the canvas and move it
    to the center of the form.

    ![](./media/image21.png)

9.  To add new screen to the app, select **+New screen** from the Tree
    view. Select **Success** screen.

    ![](./media/image22.png)

10. Double click on the **Success message** and change it to “**Your
    response submitted successfully**”.

    ![](./media/image23.png)

11. To add Text label, select **+Insert \> Text label**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image24.png)

12. Move the **Text label** below the success message and change the
    **Text** property of the label to "**If you need more information,
    kindly click on below Copilot button**".

    ![](./media/image25.png)

13. Change the **Font** of the label to **Segoe UI**, **Font size –
    21**, **center alignment** and resize the label as shown in the
    image below.

    ![](./media/image26.png)

14. Select **+Insert \> Button**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image27.png)

15. Move the button below the text label. Double click on the button and
    change the **Text property** of it to “**Copilot**”.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image28.png)

16. To add one more screen to the app, select **+New screen \> Blank**.

    ![](./media/image29.png)

17. To add navigation path to each screen, select **Screen1** from the
    Tree view.

    ![](./media/image30.png)

18. Select **Submit response button** on Screen1. Add following formula
    to the existing formula of OnSelect property of the button.

    **Note**: Ensure that, the existing formula is ended with semicolon
    (;).
    
    *Navigate(Screen2);*
    
    ![](./media/image31.png)

19. Now, select **Screen2**.

    ![](./media/image32.png)

20. Select **Copilot button** and change its **OnSelect** property to
    the given formula.

    *Navigate(Screen3);*
    
    ![](./media/image33.png)

21. Select the **Fill** property of the button and replace it with the
    **ButtonColor**.

    **Note:** ButtonColor is the Named variable which contains color
    value.
    
    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image34.png)

22. Save the app.

    ![](./media/image35.png)

## **Exercise 2: Add Copilot control to a canvas app (preview)**

### **Task 1: Add the Copilot control to your canvas app**

1.  Select **App** from the **Tree view**.

    ![A screenshot of a computer Description automatically generated](./media/image36.png)

2.  On the command bar, select **Settings**. If the Settings is not
    visible, select **ellipsis** (…)

    ![](./media/image37.png)

3.  Select **Updates**. Select he **Preview** tab, set the toggle
    for **Copilot component** to **On**.

    ![](./media/image38.png)

4.  Now select **Screen3** in the Tree view. On the app authoring menu,
    select **Insert**. Select **Copilot (preview)** to add this control.

    ![](./media/image39.png)

5.  When the Copilot control is added, from the
    control **Properties** tab, select **Data source (Items)** and
    choose a Dataverse table – **Membership Forms** for your data
    source. Currently, the Copilot control can only answer questions for
    smaller datasets.

    ![](./media/image40.png)
    
    ![](./media/image41.png)

6.  Click on **Views** drop down and select **Active Membership Forms**.

    ![](./media/image42.png)

7.  Select **Edit** in front of the Fields control from the
    **Properties** pane.

    ![](./media/image43.png)

8.  To remove **Created On** column, select (…) next to **Created On**
    and then select **Remove**.

    ![](./media/image44.png)

9.  Add all the fields present in the app. Select **Add fields**, select
    **Email Address**, **Membership Date**, **Membership Type**,
    **Street Address** and **Phone Number** and then select **Add**.

    ![](./media/image45.png)

10. Move the Copilot control to the center of the screen.

    ![](./media/image46.png)

11. Select **+Insert \> Button**.

    ![](./media/image47.png)

12. Move the button as shown in the belove image.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image48.png)

13. Doble click on the Button control and change its **Text** property
    to **Done**. Move the Button below the Copilot control.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image49.png)

14. Now select the **OnSelect** property of the Button from property
    selector and change it to the given formula.

    Navigate(Screen1);
    
    ![](./media/image50.png)

15. Save the app.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image51.png)

16. Select **Test** icon to test the app.

    ![](./media/image52.png)

17. Fill up the Membership form and select Submit response. You will be
    navigated to **Success** screen.

    ![](./media/image53.png)

18. Select **Copilot** button.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image54.png)

19. Ask more questions. For example – What is the Membership type of
    Sara?

    **Note:** To have better experience, add more responses to the data.
    
    ![](./media/image55.png)

20. Select **Done**.

    ![A screenshot of a chat AI-generated content may be incorrect.](./media/image56.png)

**Summary**: In this lab, you learnt how to create a canvas app from an
image, how it gets connected to your data stored in the Dataverse and
how to customize the app. You also learnt how to add Copilot control to
a canvas app which lets app users get insights about the data in your
app through natural language conversations with an AI-powered copilot.


