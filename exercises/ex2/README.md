# Exercise 2 - Analyze Transition Options: Find Transition Approach
<p align="justify">In this exercise, you will analyze your system data and determine the most suitable transition path to <b>SAP S/4HANA Cloud, private edition</b> using the <b>Find Transformation Approach</b> app in <b>SAP Cloud ALM</b>. Based on your uploaded analysis files, you will create a transformation approach project, complete the scenario fit assessment, and initialize a transformation project to kick off the implementation phase.</p>

This exercise consists of the following sub-exercises:
- [Exercise 2.1 - Create Transformation Approach](#exercise-21---create-transformation-approach)
- [Exercise 2.2 - Run Scenario Fit Assessment](#exercise-22---run-scenario-fit-assessment)
- [Exercise 2.3 - Review Transformation Project Tasks](#exercise-23---review-transformation-project-tasks)

<br>

## Exercise 2.1 - Create Transformation Approach
<p align="justify">In this sub-exercise, you will set up the transformation approach project and explore system insights based on your uploaded analysis files. This lays the groundwork for identifying the most suitable transition path in the next step.</p>

### Steps:
Follow these steps to complete the exercise:<br>
1.  Open [SAP Cloud ALM](https://calm-consarea-sdt.eu10-004.alm.cloud.sap) and log in with the user **DEMOXX** (replace *XX* with your seat number, for example **DEMO01**).<br>

    > **💡 TIP**: To open this link in a new tab, **right-click** and choose **Open Link in New Tab**.

2.  Navigate to **Transformation** [1] &gt; **Find Transformation Approach** [2].<br><br>
    ![](/exercises/ex2/images/Screenshot-1-01.png)<br>

3.  In the **Find Transformation Approach** application, choose **Create**.<br><br>
    ![](/exercises/ex2/images/Screenshot-1-02.png)<br>

4.  Enter **APPROACH_DT264_US_XX** (replace *XX* with your seat number, for example **APPROACH_DT264_US_01**) as the **Name**.<br><br>
    ![](/exercises/ex2/images/Screenshot-1-03.png)<br>

5.  Open the **Products / SKUs** [1] tab and select **SAP ECC** as **Source Product** [2] and **SAP S/4HANA Cloud Private Edition (RISE with SAP)** as **Target Product** [3].<br><br>
    ![](/exercises/ex2/images/Screenshot-1-04.png)<br>

6.  Open the **Analysis** tab and select the **MRC** and **UDP** files created in the previous exercise. Then choose **Create**.<br><br>
    ![](/exercises/ex2/images/Screenshot-1-05.png)<br>

7.  The project details appear, visualizing the first **system metrics** such as **Lifespan**, **Size** and **Extensibility**.<br><br>
    ![](/exercises/ex2/images/Screenshot-1-06.png)<br>

8.  Let’s dive deeper into the **System Insights** section to explore key information derived from your uploaded analysis files.<br><br>
    The **Key Metrics** area provides an overview of your system’s overall **lifespan**, **data footprint**, and **extensibility** indicators.<br><br>
    Under **Data Highlights**, you can review insights such as the **Top Company Codes**, **Top Application Components**, the **Number of Technical Modifications**, and the **Number of Technical Custom Extensions**.
    These insights help you understand the complexity and scope of your source system before determining the most suitable transformation approach in the next sub-exercise.<br><br>
    ![](/exercises/ex2/images/Screenshot-1-07.png)<br>

9.  **Congratulations!** You have successfully completed this sub-exercise.<br><br><br>


## Exercise 2.2 - Run Scenario Fit Assessment
<p align="justify">After creating your transformation approach project in the previous exercise, you will now complete the <b>Scenario Fit Assessment</b>. By answering a short, system-tailored questionnaire, you’ll receive a recommendation for the most suitable transition scenario and directly create your transformation project to start with the implementation.</p>

### Steps:
Follow these steps to complete the exercise:<br>
1.  Within your transformation approach project, open the **Scenario Fit Assessment** tab [1] and choose **Start Questionnaire**.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-01.png)<br>

2.  The questionnaire opens, consisting of eight questions. Open the details of the first question.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-02.png)<br>

3.  For **Choose the appropriate option**, select **No complex transformation requirements anticipated (Low effort)** and choose **Apply**.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-03.png)<br>

4.  Repeat Steps 2 and 3 to answer the other questions.<br>
    - Question 2 (Planned Rollout Strategy): Select **Full system (Low effort)**
    - Question 3 (Business System Downtime): Select **Less than 48 hours (Medium effort)**
    - Question 4 (Re-Engineering & Change Management): Select **Medium demand to change (Moderate effort)**
    - Question 5 (Data Scope): Select **Only active and relevant data incl. history (Low effort)**
    - Question 6 (Transformation Requirements): Select **Medium (Moderate effort)**
    - Question 7 (Company Codes): Select **Yes, it is**
    - Question 8 (Customer Tables): Select **Yes, it is**

5.  Choose **Save**.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-04.png)<br>

6.  The **Scenario Selection** overview appears. It identifies **Selective Data Transition** [1] as the best-fit scenario and automatically suggests the required **SAP Tooling** [2] for this approach.<br><br>
    Open the details of the **Selective Data Transition** scenario [3].<br><br>
    ![](/exercises/ex2/images/Screenshot-2-05.png)<br>

7.  The scenario details appear, displaying both the **Scenario Overview** and the **Scenario Fit Insights**.<br><br>
    Since this scenario will be used, choose **Finalize Selection**.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-06.png)<br>

8.  On the **Finalize Transformation Approach Setup** dialog, choose **Finalize**.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-07.png)<br>

9.  The **Selective Data Transition** scenario is now automatically selected. Close the details.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-08.png)<br>

10. Choose **Create Transformation Project**.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-09.png)<br>

11. The **Transformation Project** wizard opens.<br><br>
    Enter **PROJECT_DT264_US_XX** (replace *XX* with your seat number, for example **PROJECT_DT264_US_01**) as the **Name**, and choose **Save**.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-10.png)<br>

12. The details of the **Transformation Project** appear, confirming that your project has been successfully created and is ready for implementation.<br><br>
    The **Transformation Project** provides a **standard task list** for the Selective Data Transition scenario in **SAP Cloud ALM**. It serves as the central workspace to **collect all relevant information, orchestrate activities in SAP Business Transformation Center**, and **track progress** across all implementation phases.<br><br>
    ![](/exercises/ex2/images/Screenshot-2-11.png)<br>

13. **Congratulations!** You have successfully completed this sub-exercise.<br><br><br>


## Exercise 2.3 - Review Transformation Project Tasks
<p align="justify">After finalizing the transformation approach, you will now review the automatically created <b>Transformation Project</b> and its associated task list in <b>SAP Cloud ALM</b>. This task list outlines all key setup activities required to prepare your <b>Selective Data Transition</b> project—from establishing connectivity and verifying preconditions to initializing the digital blueprint.</b>

<p align="justify">In a real implementation, you would execute these setup tasks step by step to configure the environment. However, since the system landscape for this hands-on session has already been fully prepared, you will skip these initial tasks and proceed directly to the next step: <b>Creating the Digital Blueprint</b>, which marks the start of the guided transition process.</p>

### Steps:
Follow these steps to complete the exercise:<br>
1.  Within your transformation project, choose **Go to Transformation Project Overview**.<br><br>
    ![](/exercises/ex2/images/Screenshot-3-01.png)<br>

3.  The **Project Overview** appears. Under **Project Tasks**, open the first task **Set Up and Configure SAP Business Transformation Center**.<br><br>
    ![](/exercises/ex2/images/Screenshot-3-02.png)<br>

4.  The **Tasks** application opens with the task preselected. Review the description of the activities that need to be completed within this step.<br><br>
    ![](/exercises/ex2/images/Screenshot-3-03.png)<br>

5.  Once reviewed, change the status to **Done** and return to the project management overview using the **Back** button.<br><br>
    ![](/exercises/ex2/images/Screenshot-3-04.png)<br>

6.  The task now switches from **Open** to **Done**.<br><br>
    ![](/exercises/ex2/images/Screenshot-3-05.png)<br>

7.  In **Project Tasks**, scroll down to **Create a Digital Blueprint** and choose **Summary** [1].<br><br>
    ![](/exercises/ex2/images/Screenshot-3-06.png)<br>

8.  The **Summary** view appears, providing a preview of the activities you will perform in the next exercise.<br><br>
    ![](/exercises/ex2/images/Screenshot-3-07.png)<br>

9.  **Congratulations!** You have successfully completed this sub-exercise.<br><br><br>

## Optional: Test Your Knowledge
Run this optional [quiz](https://quiz-app-gk8jvkhz.cfapps.eu10-005.hana.ondemand.com/dt264a/quiz/fr4163gk) to test your understanding. If you prefer to skip it, continue with the next exercise.<br>

> **💡 TIP**: To open this link in a new tab, **right-click** and choose **Open Link in New Tab**.
<br>

## Summary
<p align="justify">You have now analyzed your transition options and identified <b>Selective Data Transition</b> as the best-fit scenario for your move to <b>SAP Cloud ERP Private</b>. The automatically created <b>Transformation Project</b> provides the structure for all setup activities and marks the starting point for your guided implementation.</p>


Continue to - [Exercise 3 - Initialize Project: Create Digital Blueprint](../ex3/README.md)
