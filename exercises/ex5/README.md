# Exercise 5 - Build the Model: Create Transformation Model & Version
<p align="justify">In this exercise, you will create the transformation model and its version, the technical foundation that defines how your scoped data will be processed during execution in the upcoming cycle. The transformation model translates the scope defined in the digital blueprint into technical definitions and rules that fully describe the transformation initiative.</p><br>

## Steps:
Follow these steps to complete the exercise:<br>
1.  Within your confirmed blueprint, choose **Create Transformation Model**.<br><br>
    ![](/exercises/ex5/images/Screenshot-01.png)<br>

2.  The **Manage Transformation Models** application opens, with your blueprint already preselected.<br>
3.  Enter **TRF_MDL_DT264_XX** (replace *XX* with your seat number, for example **TRF_MDL_DT264_01**) as **Title** and choose **Create**.<br><br>
    ![](/exercises/ex5/images/Screenshot-02.png)<br>

4.  After a few seconds, the **Transformation Model** is successfully created.<br><br>
    In this view, you can see that the transformation model combines all **transformation objects**, **relations**, **filters**, and **rules** into one consistent technical definition for your transformation initiative.<br><br>
    In addition to the scoped objects defined in your **Digital Blueprint**, extra elements are automatically added to ensure consistency — including semantically related or logically grouped objects, baseline components required for technical stability, and custom objects identified through the **System Scan**.<br><br>
    ![](/exercises/ex5/images/Screenshot-03.png)<br>

5.  Choose **Transformation Objects** [1] and search for **FI Document** [2]. Then scroll down and click the **Name** of the **FI Document** [3] transformation object to navigate into it.<br><br>
    ![](/exercises/ex5/images/Screenshot-04.png)<br>

6.  The details of the **FI Document** appear. Choose **Filters**.<br><br>
    You can see that the transformation filters applied to this object are displayed - there are filters for **Org** and **Time Slice** on several tables and fields.<br><br>
    ![](/exercises/ex5/images/Screenshot-05.png)<br>

7.  Use the **Back** button to return to the transformation model overview.<br><br>
    Choose **Transformation Filters** tab [1] and then open the **Company Code Filter** [2] with the ID EccCompanyCodeFilter.<br><br>
    ![](/exercises/ex5/images/Screenshot-06.png)<br>

8.  The filter details open, showing that the value is set to company code **2000** — as scoped in your blueprint.<br><br>
    ![](/exercises/ex5/images/Screenshot-07.png)<br>

9.  Next, open the **Fiscal Year Greater Than or Equal To Filter** with the ID EccFiscalYearGreaterEquals.<br><br>
    The filter value is set to **2021**, following the Time Slice definition.<br><br>
    ![](/exercises/ex5/images/Screenshot-08.png)<br>

10. Use the **Back** button to return to the transformation model overview. Then, choose **Create Version**.<br><br>
    ![](/exercises/ex5/images/Screenshot-09.png)<br>

11. The **Transformation Model Version** application opens, with your transformation model already preselected.<br>
12. Enter **MDL_V1** as **Title** and choose **Create**.<br><br>
    ![](/exercises/ex5/images/Screenshot-10.png)<br>

13. After a few seconds, the **Transformation Model Version** is successfully created.<br><br>
    It represents a **snapshot** of your **transformation model** and serves as the **technical basis** for executing the **data transformation**.<br><br>
    It contains the same **objects**, **relations**, **filters**, and **rules** as defined in the model, ensuring that each transformation run is performed **consistently** and can be **traced back** to its exact configuration.<br><br>
    ![](/exercises/ex5/images/Screenshot-11.png)<br>

14. **Congratulations!** You have successfully completed this exercise.<br><br><br>

## Optional: Test Your Knowledge
Run this optional [quiz](https://quiz-app-gk8jvkhz.cfapps.eu10-005.hana.ondemand.com/dt264/quiz/7v6kfj3m) to test your understanding. If you prefer to skip it, continue with the next exercise.<br>

> **💡 TIP**: To open this link in a new tab, **right-click** and choose **Open Link in New Tab**.
<br>

## Summary
<p align="justify">You have now built a transformation model and version that capture all scoped and related objects, preparing the setup for executing the transformation in the next exercise.</p>

Continue to - [Exercise 6 - Initialize Cycle: Create Cycle & Run Prevalidation](../ex6/README.md)