# Exercise 7 - Execute Blueprint: Review Reference Cycle
<p align="justify">In this exercise, you will explore the <b>execution phases</b> of your cycle, which manage the <b>end-to-end data transformation</b> between the source and target system — from generating runtime objects to completing postprocessing activities. Due to time constraints, these runtime-intensive phases will be reviewed using a pre-executed <b>reference cycle</b>, during which you will also observe how the <b>DTV</b> (Data Transition Validation) project is automatically created and transferred without performing any manual configuration steps.</p>

This exercise consists of the following sub-exercises:
- [Exercise 7.1 – Review Cycle Preparation](#exercise-71--review-cycle-preparation)
- [Exercise 7.2 - Review Run & Postprocess Cycles](#exercise-72---review-run--postprocess-cycles)

<br>

## Exercise 7.1 – Review Cycle Preparation
<p align="justify">In this sub-exercise, you will review the <b>Cycle Preparation</b> phase of the cycle. During this phase, the system generates runtime objects for transformation and postprocessing — and automatically creates a DTV project in the source system if the DTV tool was enabled.</p><br><br>

> **⚠️ CAUTION**: In this exercise, you will switch to the **reference implementation** cycle. Make sure to follow the instructions carefully to avoid inconsistencies in the process.

<br>

### Steps:
Follow these steps to complete the exercise:<br>
1.  Within your cycle, open **Manage Cycles** [1] context menu and select the **Transformation** [2] application.<br><br>
    ![](/exercises/ex7/images/Screenshot-1-01.png)<br>

2.  The **Transformation** overview is displayed. Choose **Manage Cycles**.<br><br>
    ![](/exercises/ex7/images/Screenshot-1-02.png)<br>

3.  In the **Manage Cycles** application, enter **CYCLE_REFERENCE_IMPL** in the search field [1] and press **Enter**. Then open the corresponding cycle [2].<br><br>
    ![](/exercises/ex7/images/Screenshot-1-03.png)<br>

4.  The **Reference Implementation Cycle** appears. Navigate to **2. Cycle Preparation**.<br><br>
    ![](/exercises/ex7/images/Screenshot-1-04.png)<br>

5.  Choose **Preparation Log** to display the execution details.<br><br>
    ![](/exercises/ex7/images/Screenshot-1-05.png)<br>

6.  The **Cycle Logs** applications opens. Enter **DTV** into the search field [1] and press **Enter**.<br><br>
    As you can see, two log entries confirm that the **DTV project** was created and configured successfully [2].<br><br>
    Through this automation, much of the technical setup is handled by the system, allowing you to focus on configuring only the **DTV reports** relevant for the business data validation.<br><br>
    ![](/exercises/ex7/images/Screenshot-1-06.png)<br>

7.  **Congratulations!** You have successfully completed this sub-exercise.<br><br><br>


## Exercise 7.2 - Review Run & Postprocess Cycles
<p align="justify">After reviewing the cycle preparation, you will now explore the Run and Postprocess phases of the reference implementation. These phases demonstrate how the data transformation is executed and how the DTV (Data Transition Validation) project is automatically transferred to the target system for subsequent validation.</p>

### Steps:
Follow these steps to complete the exercise:<br>
1.  Within the reference cycle, open the **3. Run Cycles** tab.<br><br>
    ![](/exercises/ex7/images/Screenshot-2-01.png)<br>

2.  Choose **Go to Run Cycles**.<br><br>
    ![](/exercises/ex7/images/Screenshot-2-02.png)<br>

3.  Enter **FI Document** into the search field [1] and press **Enter**.<br><br>
    You can see how the data transformation, for example for **financial documents**, was executed during runtime.<br><br>
    ![](/exercises/ex7/images/Screenshot-2-03.png)<br>

4.  Use the **Back** button to return to the cycle overview.<br>
5.  Open the **4. Postprocess Cycles** tab.<br><br>
    ![](/exercises/ex7/images/Screenshot-2-04.png)<br>

6.  Choose **Go to Postprocess Cycles**.<br><br>
    In the postprocessing phase, the migrated data is converted to match the release and data structures of the target system using the ABAP upgrade mechanism. This ensures that the transferred data and configuration are fully compatible with SAP S/4HANA.<br><br>
    ![](/exercises/ex7/images/Screenshot-2-05.png)<br>

7.  Enter **DTV** into the search field [1] and press **Enter**.<br><br>
    The program **BDTS_DTV_TABLE_TRANSFER** is executed in this phase. It transfers the DTV project and related configuration tables from the source system to the target system and automatically extends the setup to include the new SAP S/4HANA environment.<br><br>
    ![](/exercises/ex7/images/Screenshot-2-06.png)<br>

8.  Use the **Back** button to return to the cycle overview.<br>
9.  **Congratulations!** You have successfully completed this sub-exercise.<br><br><br> 

## Optional: Test Your Knowledge
Run this optional [quiz](https://quiz-app-gk8jvkhz.cfapps.eu10-005.hana.ondemand.com/dt264/quiz/yl9up3e5) to test your understanding. If you prefer to skip it, continue with the next exercise.<br>

> **💡 TIP**: To open this link in a new tab, **right-click** and choose **Open Link in New Tab**.
<br>

## Summary
<p align="justify">You have now completed the execution phase of your lean selective data transition. By reviewing the reference cycle, you explored how <b>SAP Business Transformation Center</b> manages the automated transformation flow — from preparing runtime objects to transferring and validating data in the target system.</p>
<p align="justify">🎉 <b>Congratulations</b> — This concludes the hands-on session <b>How to Start Transitioning to SAP Cloud ERP Private</b>, where you successfully completed a guided transition to <b>SAP Cloud ERP Private</b> using <b>SAP Business Transformation Center (BTC)</b>.</p>