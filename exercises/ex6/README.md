# Exercise 6 - Initialize Cycle: Create Cycle & Run Prevalidation
<p align="justify">In this exercise, you will create a cycle based on your transformation model version. It represents the execution layer of your data transformation, connecting the source and target systems and defining when and how data is processed.</p><br>

## Steps:
Follow these steps to complete the exercise:<br>
1.  Within your model version, choose **Create Cycle**.<br><br>
    ![](/exercises/ex6/images/Screenshot-01.png)<br>

2.  The **Manage Cycles** application opens with your **Transformation Model** and **Transformation Model Version** preselected.<br>
3.  Maintain the following details in the **Cycle Attributes** and **System Connection** sections, then choose Create:<br>
    - **Name**: **CYCLE_DT264_US_XX** (replace *XX* with your exercise number, for example **CYCLE_DT264_US_01**)
    - **Type**: **Test**
    - **Retention Date**: for example **Dec 31, 2025**
    - **Use DTV Tool**: **Yes**
    - **Source System**: **SRC.300**
    - **Target System**: **TGT.300**

    <br>

    ![](/exercises/ex6/images/Screenshot-02.png)<br>

4.  After a few seconds, the **Cycle** is successfully created and appears in status **New**.<br><br>
    It serves as the **execution layer** of your transformation model version, connecting the source and target systems. Each cycle follows **four structured phases** that guide the end-to-end data transformation.<br><br>
    ![](/exercises/ex6/images/Screenshot-03.png)<br>

5.  Next, begin with the **first phase** of the cycle — **Prevalidation**. Choose **1. Cycle Prevalidation** to open the corresponding section.<br><br>
    ![](/exercises/ex6/images/Screenshot-04.png)<br>

6.  The **Cycle Prevalidation** section opens.<br><br>
    The **Prevalidation** phase ensures that your cycle is technically ready to proceed with data preparation and transformation. During this phase, additional **data transformation–specific checks** are performed to verify system consistency and readiness.<br><br>
    These automated validations analyze both the **source** and **target systems**, identifying potential configuration or connectivity issues early in the process. You can monitor the current **Prevalidation Status** [1] and review detailed results in the **Prevalidation Logs** [2], which summarize all executed checks and their outcomes.<br><br>
    ![](/exercises/ex6/images/Screenshot-05.png)<br>
    
6.  Choose **Run Prevalidation** to start the analysis.<br><br>
    ![](/exercises/ex6/images/Screenshot-06.png)<br>

7.  The prevalidation process is initiated, and system checks begin.<br><br>
    After a few minutes, the checks are completed. Use the **Refresh** button on top of the screen to update the status — the individual checks will change to **Done** once successfully finished.<br><br>
    ![](/exercises/ex6/images/Screenshot-07.png)<br>
8.  The cycle is now validated and ready for the subsequent transformation phases.<br>
9.  **Congratulations!** You have successfully completed this exercise.<br><br><br>

## Optional: Test Your Knowledge
Run this optional [quiz](https://quiz-app-gk8jvkhz.cfapps.eu10-005.hana.ondemand.com/dt264a/quiz/qoqc53td) to test your understanding. If you prefer to skip it, continue with the next exercise.<br>

> **💡 TIP**: To open this link in a new tab, **right-click** and choose **Open Link in New Tab**.
<br>

## Summary
<p align="justify">You have now created and validated a cycle based on your transformation model version. This completes the setup phase and prepares the foundation for exploring the following steps in the data transformation workflow.</p>

Continue to - [Exercise 7 - Execute Blueprint: Review Reference Cycle](../ex7/README.md)