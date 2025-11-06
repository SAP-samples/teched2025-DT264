# Exercise 1 - Build the Foundation: Upload UDP & MRC File
<p align="justify">In this exercise, you will extract two key analysis files from the source SAP ERP 6.0 system – the <b>Usage and Data Profiling</b> (UDP) file and the <b>Maintenance Readiness Check</b> (MRC) file – and upload them to SAP Cloud ALM.</p>
<p align="justify">These files serve as the technical and functional input for the <b>Find Transformation Approach</b> application, providing the basis to analyze your current system setup and determine the optimal transition path to SAP Cloud ERP Private.</p><br>

## Steps:
Follow these steps to complete the exercise:<br>
1.  Log on to the **SRC** system in SAP GUI, client **300**, using the user **DEMOXX** (replace *XX* with your seat number, for example **DEMO01**), and open transaction **SE38** (ABAP Editor).<br>
2.  In the **Program** field, enter **RC_UDP_START_DMR2** [1] and choose **Execute** (F8) [2].<br><br>
    ![](/exercises/ex1/images/Screenshot-01.png)<br>

3.  Choose **Download DRM2 Analysis Data** and save the ZIP file to your local disk.<br><br>
    ![](/exercises/ex1/images/Screenshot-02.png)<br>

4.  Still in transaction **SE38**, run the program **RS_SAVE_LAST_MRC_RES_LOCALLY** [1] and choose **Execute** (F8) [2].<br><br>
    ![](/exercises/ex1/images/Screenshot-03.png)<br>

5.  Specify a **file path** [1] and choose **Execute** [2] to download the **Maintenance Readiness Check (MRC)** JSON file to your local disk.<br><br>
    ![](/exercises/ex1/images/Screenshot-04.png)<br>

6.  Switch to [SAP Cloud ALM](https://calm-consarea-sdt.eu10-004.alm.cloud.sap) and log in with the user **DEMOXX** (replace *XX* with your seat number, for example **DEMO01**).<br>

    > **💡 TIP**: To open this link in a new tab, **right-click** and choose **Open Link in New Tab**.

7.  Navigate to **Transformation** [1] &gt; **Manage Analysis File** [2].<br><br>
    ![](/exercises/ex1/images/Screenshot-05.png)<br>

8.  In the **Manage Analysis File** application, choose **Create**.<br><br>
    ![](/exercises/ex1/images/Screenshot-06.png)<br>

9.  Enter **UDP_DT264_XX** (replace *XX* with your seat number, for example **UDP_DT264_01**) as the **Name**, and keep the default **Analysis Type**.<br><br>
    ![](/exercises/ex1/images/Screenshot-07.png)<br>

10. Upload the ZIP file you downloaded in Step 3 and choose **Create**.<br><br>
    ![](/exercises/ex1/images/Screenshot-08.png)<br>

11. Verify that the analysis file has been successfully uploaded.<br><br>
    ![](/exercises/ex1/images/Screenshot-09.png)<br>

12. Repeat Steps 8 to 11 to upload the **MRC file**:
    - Enter **MRC_DT264_XX** (replace *XX* with your seat number, for example **MRC_DT264_01**) as the Name.
    - Change the **Analysis Type** to **SAP ERP Maintenance Readiness Check** (MRC).
    - Upload the **MRC JSON file**, confirm the disclaimer, and choose **Create**.
    - Verify that the file has been successfully uploaded.

    <br>

    ![](/exercises/ex1/images/Screenshot-10.png)<br>    

13. **Congratulations!** You have successfully completed this exercise.<br><br><br>


## Optional: Test Your Knowledge
Run this optional [quiz](https://quiz-app-gk8jvkhz.cfapps.eu10-005.hana.ondemand.com/dt264/quiz/sok9kkyb) to test your understanding. If you prefer to skip it, continue with the next exercise.<br>

> **💡 TIP**: To open this link in a new tab, **right-click** and choose **Open Link in New Tab**.
<br>

## Summary
<p align="justify">You have now extracted the <b>Usage and Data Profiling</b> (UDP) and <b>Maintenance Readiness Check</b> (MRC) analysis files from the source SAP ERP 6.0 system and uploaded them to the <b>Manage Analysis File</b> app in <b>SAP Cloud ALM</b>. This builds the foundation for analyzing your current system setup and determining the optimal transition path in the next exercise.</p>


Continue to - [Exercise 2 - Analyze Transition Options: Find Transition Approach](../ex2/README.md)