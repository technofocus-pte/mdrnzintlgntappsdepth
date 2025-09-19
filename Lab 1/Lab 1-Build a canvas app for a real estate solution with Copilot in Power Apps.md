# **Lab 1: Build a canvas app for a real estate solution with Copilot in Power Apps** #

**Estimated duration**: 15 min

## **Objective**: 
In this lab, you will learn to create a custom canvas app
in Power Apps through conversation with Copilot. You will learn how
Copilot generates tables, how to customize tables with the help of
Copilot and how to share an app with the user. ## 

**Note:** Copilot in Power Apps can generate different app layouts,
forms, and data connections apps.

## **Exercise 1: Build a canvas app and share with the user**

**Task 1: Create an app with Copilot**

**Note:** In this lab, your results for data might vary from those shown
in the screenshots and images. The reason is because Power Apps uses AI
to generate data for the lab and the data changes daily.

1.  Sign into the Power
    Apps +++[*https://make.powerapps.com/+++ using*](https://make.powerapps.com/+++%C2%A0using) your
    Office 365 tenant credentials.

2.  Select **Environment** **selector** to change it to developer
    environment – Dev One.

> ![](./media/image1.png)

3.  Select **Dev One** environment.

![](./media/image2.png)

4.  

> ![](./media/image3.png)

5.  From the left navigation pane, select **Apps** and then
    select **Start with Copilot**.

> ![](./media/image4.png)

6.  Enter the following prompt to search for an AI-generated table:

> +++**Build an app to manage real estate showings**+++
>
> Select the **Generate** button.
>
> ![](./media/image5.png)

7.  If you come across any pop-up, close it.

8.  Copilot creates one or more Dataverse tables with data that includes
    typical real estate tasks.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image6.png)

9.  To see more information, click on three dots of
    the **Showing** table and select **View data**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image7.png)

10. You can now see the columns on the **Showing** table.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image8.png)
>
> Your next steps are to modify and add to the already generated table.

11. Check if **Feedback** column is present in the **Showing** table. If
    yes then go to the next step, if no then select
    the **Showing** table, enter the below prompt in the copilot pane
    and click on the **Send** button.

> +++**Add the Feedback column**+++
>
> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image9.png)

12. Now click on the **Showing table** and then in the text box, in the
    lower part of the Copilot pane to the right of the screen, enter the
    following text and select the **Send** button.

> +++**Rename Feedback column as Details** **in Showing Table**+++
>
> This will rename Feedback column as Details in the showings table.
>
> ![](./media/image11.png)

13. Now click on the **Showing table** and then in the text box, in the
    lower part of the Copilot pane to the right of the screen, enter the
    following text:

> +++**In showing table add a new column as client full name**+++
>
> This will add a column in the showings table. Select
> the **Send** button.
>
> ![](./media/image12.png)

14. Select **Save and open app**.

> ![](./media/image13.png)

15. Again, select **Save and open app** on **Done working?** pane.

> ![A screenshot of a computer Description automatically
> generated](./media/image14.png)

16. When the app first loads, a dialog might appear stating “**Welcome
    to Power Apps Studio”**. If so, select the **Skip** button.

> ![](./media/image15.png)

17. The app that has been built for you should show in **Edit** mode.

> ![](./media/image16.png)

18. For a better view, close the Copliot pane.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image17.png)

19. Select the **Data** icon from the left navigation bar. Copilot has
    created a **Dataverse** table that's now displaying in
    the **Environments** section.

> ![](./media/image18.png)
>
> **Note**: Currently, Copilot is only supported for Dataverse. You
> can't use any other data access point at this time.

20. Select the **Tree view** from the left navigation bar. You can see
    the **Welcome screen** is opened in the canvas and other remaining
    screens are listed under the Tree view on left side.

> ![](./media/image19.png)

21. Click on **Showings screen** in the **Tree view** and you can see
    the screen is now opened.

> ![](./media/image20.png)

22. From the upper part of your screen, select the **Save** button to
    save the new app that you created.

> ![](./media/image21.png)

23. Give the app name as +++**Real Estate Showings**+++ and
    select **Save**.

> ![A purple rectangle with a red rectangle AI-generated content may be
> incorrect.](./media/image22.png)

**Task 2: Test the app**

1.  Select the **Play** button from the upper part of the screen to test
    the app.

> ![](./media/image23.png)

2.  In the left pane, select the **+New** button.

> ![](./media/image24.png)

3.  Fill in the fields with the following information and then select
    the check mark in the upper-right corner of the screen.

> **Showing:** +++Showing 6+++
>
> **Showing Date:** Enter any future date
>
> **Time:** 09:00
>
> **Agent Name:** Select any from the suggestions.
>
> **Details:** +++Spacious+++
>
> **Property:** Select any from the suggestions. ![A screenshot of a
> computer AI-generated content may be incorrect.](./media/image25.png)

4.  To close the test window, select cross mark at the top right corner
    of the screen.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image26.png)

5.  You will be navigated to the editing window. Select **Ok** on the
    ‘**Did you know**’ pop-up window.

> ![A white background with black text Description automatically
> generated](./media/image27.png)

6.  To publish the app, select **Publish** button on from the top right
    of the screen.

> ![](./media/image28.png)

7.  Select **Publish this version**.

> ![](./media/image29.png)

8.  Select **\<- Back** to go back on the home page.

> ![](./media/image30.png)

9.  Select **Leave**.

> ![](./media/image31.png)

**Task 3: Share the app with user**

1.  Select **Apps** from left navigation pane, select **Real Estate
    Showings** app and then select **Share** from above horizontal
    palette.

> ![](./media/image32.png)

2.  Type +++Brooke+++ and then select **Brooke Gray** from the
    suggestions.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image33.png)

3.  Select **Share**.

> ![](./media/image34.png)

4.  Select **Copy link**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image35.png)

5.  Open the link in the new tab and sign in with Brooke Gray’s email
    ID. Open a new browser, paste the above link and sign in with
    Brooke's credentials and then you can see the app.

> **Note**: Open the Outlook account of the Brooke Gray with Login id
> - [*+++brookeg@LODSA7xxxxx.onmicrosoft.com*](mailto:+++brookeg@LODSA7xxxxx.onmicrosoft.com)+++
> (**change the domain name** in login id) and Password –
> +++Pa$$w0rd@124+++.
>
> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image36.png)

6.  Select **Showings** screen.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image37.png)

**Summary**: In this lab, you learnt how to create a custom canvas app
using copilot, how to customize and share the app with the user.



