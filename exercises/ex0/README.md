# Scenario Overview
<p align="justify">In this exercise, you will get an overview of the overall transformation scenario and the system landscape used throughout this hands-on session. You will also review the key preparation steps that have already been completed to set up the environment for the upcoming exercises.</p><br>

## Customer Situation
<p align="justify">In this hands-on session, you will work with the fictional company <b>CONSAREA Inc.</b>, a global manufacturer and distributor of premium pencils. CONSAREA is currently running on <b>SAP ERP 6.0 EhP8</b> and has decided to transition to <b>SAP S/4HANA 2023 FPS04</b> in the <b>Private Cloud Environment</b>.</p> 
<p align="justify">Like many real-world enterprises, CONSAREA aims to modernize its IT landscape while keeping the transition lean and cost-efficient.</p><br> 

## DT264 at a Glance
<p align="justify">This hands-on session consists of <b>two main parts</b> that together illustrate a complete, data-driven transition journey from <b>SAP ERP</b> to <b>SAP S/4HANA 2023 FPS04</b> in the <b>Private Cloud Environment</b>.</p>

<p align="justify">In the <b>first part</b>, you will use the <b>Find Transformation Approach</b> app to determine the most suitable transformation scenario for the company. As a result of this assessment, <b>Selective Data Transition</b> will be identified as the best-fit approach for CONSAREA.</p>

<p align="justify">In the <b>second part</b>, you will perform a <b>first sandbox run</b> of a data-driven Selective Data Transition. Building on the pre-assessed and preconfigured environment, you will see how data-driven tools guide each stage of the process — from creating the digital blueprint to <b>scoping</b>, <b>modeling</b>, and <b>executing</b> the transition to <b>SAP Cloud ERP Private</b>.</p>

<p align="justify">Below you find an overview of all exercises and their corresponding project phases.</p>

![](/exercises/ex0/images/Screenshot-02.png)<br><br><br>


## Prepared Landscape
<p align="justify">Following the identification of Selective Data Transition as the most suitable scenario, a dedicated system landscape was prepared upfront to support the hands-on exercises.</p>

<p align="justify">To enable <b>Lean SDT</b> with <b>SAP Business Transformation Center</b> (BTC), a <b>shell copy</b> of the source SAP ECC system is required. This shell contains only the <b>customizing and technical repository</b>, forming the foundation for a lean and controlled transition. By excluding application data such as master or transactional records, the shell provides a clean configuration baseline for the new SAP S/4HANA system.</p>

<p align="justify">Based on this requirement, the following setup steps were performed to prepare the target environment. A copy of the source system was created using <b>Software Provisioning Manager</b> (SWPM) with the Shell Copy [1] option. Once the shell system was available, the client designated for <b>SAP Business Transformation Center</b> was copied using a <b>remote client copy</b> [2] with a customizing-only profile. Finally, the prepared shell system was <b>moved and converted in a single step</b> to <b>SAP S/4HANA 2023 FPS04</b> using the <b>Database Migration Option with System Move to SAP S/4HANA</b> (DMOVE2S4) [3] approach, executed via <b>RISE with SAP System Transition Workbench</b>.</p>

<p align="justify">This process transfers the prepared shell directly to the Private Cloud Environment and performs the technical conversion in one integrated step — resulting in a clean, preconfigured target system.</p>

![](/exercises/ex0/images/Screenshot-01.png)<br>

<p align="justify">To complete the setup, the configuration of <b>Business Transformation Center</b> was orchestrated using <b>Cloud Integration Automation Service</b> (CIAS), ensuring that all required components and connections are ready for use.</p><br>

## Landscape Overview
<p align="justify">The following landscape illustrates the end-to-end setup used in this hands-on session:</p>

![](/exercises/ex0/images/Screenshot-03.png)<br><br><br>

## Further Links

<p align="justify">If you would like to explore more about the concepts and tools used in this hands-on session, refer to the following resources:</p>

> **💡 TIP**: To open the links in a new tab, **right-click** and choose **Open Link in New Tab**.

- [SAP Help Portal: Transformation Guidance](https://help.sap.com/docs/btc/application-help/get-transformation-guidance)
- [SAP Help Portal: SAP Business Transformation Center](https://help.sap.com/docs/btc)
- [Blog: Creating the Shell System for SAP Business Transformation Center: A Practical Approach](https://community.sap.com/t5/technology-blog-posts-by-sap/creating-the-shell-system-for-sap-business-transformation-center-a/ba-p/14109065)
- [SAP Help Portal: Shell Copy Option of Software Provisioning Manager 1.0](https://help.sap.com/docs/SOFTWARE_PROVISIONING_MGR_10/159a36e76fe84e54a703f846b08ae1f6/9b25e19477dc47dc9522691f127a84d4.html?language=en-US)
- [SAP Help Portal: RISE with SAP System Transition Workbench](https://help.sap.com/docs/rise-system-transition/workbench/about-rise-with-sap-system-transition-workbench?version=SHIP)
- [SAP Help Portal: Cloud Integration Automation Service (CIAS)](https://help.sap.com/docs/cloud-integration-automation)
- [SAP Help Portal: Data Transition Validation (DTV)](https://help.sap.com/docs/ABAP_PLATFORM_NEW/9d6aa238582042678952ab3b4aa5cc71/0d8c47a6cb2440a58e804f6e0e4877d4.html)
- [SAP Community: Data Transition and Transformation](https://pages.community.sap.com/topics/data-transition-transformation)

<br>

## Summary

<p align="justify">You have now reviewed the overall transformation scenario, explored the CONSAREA system landscape, and understood the key preparation steps that enable the upcoming exercises. The environment is fully set up and ready for the next phase of your journey.</p>

Continue to - [Exercise 1 - Build the Foundation: Upload UDP & MRC File](../ex1/README.md)
