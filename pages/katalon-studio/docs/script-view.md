---
title: "Script View" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/script-view.html 
redirect_from: "/display/KD/Script+View" 
description: 
---
In addition to the [Manual view](https://docs.katalon.com/display/KD/Test+Case+Manual+View), Katalon Studio allows expert users to programmatically write automation test in the Script view of test cases. Users with Groovy/Java background can easily modify the test script as needed.

Given a sample test case with the steps as below:

*   _Open the browser_
*   _Navigate to a website_
*   _Click on certain control_
*   _Validate if a control exists on the page_
*   _Close the browser_

Follow these steps to automate the above test scenario in **Script view**:

1.  Select **File > New > Test Case** from the main menu. The **New Test Case** dialog will be displayed. Provide the name for the new test case, then click **OK**.  
    ![](../../images/katalon-studio/docs/script-view/image2017-2-15 9_59_10.png)  
      
    
2.  Once a new test case is created, you can switch to the **Script view** using the corresponding tab at the footer of the test case editor and observe how test steps of the **Manual view** are translated into a Groovy script in **Script view**.  
    ![](../../images/katalon-studio/docs/script-view/image2017-6-30 19_24_19.png)  
      
    
3.  To use a built-in **WebUI** keyword, enter the following syntax into the editor. 
    
    ```groovy
    WebUI.
    ```
    
      
    The **Content Assist** function will be invoked after users enter the **dot** character. **Content Assist** provides users with a context-sensitive suggestion for code completion. Therefore, all the built-in keywords for WebUI testing will be displayed as below:  
    ![](../../images/katalon-studio/docs/script-view/image2017-6-30 19_25_5.png)  
      
    
4.  Select the **[Open Browser](https://docs.katalon.com/display/KD/%5BWebUI%5D+Open+Browser)** keyword. This keyword will open a browser and navigate to the specified URL if provided. Selected keywords will have their description displayed along for reference.  
    ![](../../images/katalon-studio/docs/script-view/image2017-6-30 19_28_19.png)  
      
    
5.  Enter the **[Navigate To Url](https://docs.katalon.com/display/KD/%5BWebUI%5D+Navigate+to+Url)** keyword. This keyword will navigate to a specified URL. For now, enter the URL of Katalon Studio ([katalon.com](http://katalon.com)) as an input parameter.  
    ![](../../images/katalon-studio/docs/script-view/image2017-6-30 19_29_21.png)  
      
    
6.  Enter the **[Click](https://docs.katalon.com/display/KD/%5BWebUI%5D+Click)** keyword. This keyword represents the click action on a given object. You need to specify an object for this action.    
    ![](../../images/katalon-studio/docs/script-view/image2017-6-30 19_29_41.png)  
      
    
7.  Use the following syntax to refer to an object in **Object Repository** (alternatively, you can drag and drop the object to test case editor to generate the syntax):
    
    ```groovy
    findTestObject('{Object ID}')
    ```
    
    Where **Object ID** is the ID of that object in Katalon Studio.
    
    > You can find object ID from its Properties dialog. For example:
    > 
    > ![](../../images/katalon-studio/docs/script-view/image2017-2-15 13_18_7.png)
    
8.  Enter the **[Verify Element Present](https://docs.katalon.com/display/KD/%5BWebUI%5D+Verify+Element+Present)** keyword. This keyword validates if a certain object is displayed on the executing browser. Similar to the previous step, you need to specify the object to be used with this keyword.  
    ![](../../images/katalon-studio/docs/script-view/image2017-2-15 13_26_9.png)  
      
    
9.  Add the **[Close Browser](https://docs.katalon.com/display/KD/%5BWebUI%5D+Close+Browser)** keyword and save your test case.  
    ![](../../images/katalon-studio/docs/script-view/image2017-2-15 13_27_9.png)  
      
    The following API docs may prove useful when working in Script view:
    
    <table><thead><tr><th><div class="tablesorter-header-inner">Class</div></th><th><div class="tablesorter-header-inner">Description</div></th></tr></thead><tbody><tr><td><strong><a class="external-link" href="http://api-docs.katalon.com/studio/v4.6.0.2/api/com/kms/katalon/core/keyword/BuiltinKeywords.html" rel="nofollow">Builtin Keywords</a></strong></td><td>List of common built-in keywords</td></tr><tr><td><strong><a class="external-link" href="http://api-docs.katalon.com/studio/v4.6.0.2/api/com/kms/katalon/core/webui/keyword/WebUiBuiltInKeywords.html" rel="nofollow">WebUI Builtin Keywords</a></strong></td><td>List of Web UI built-in keywords</td></tr><tr><td><strong><a class="external-link" href="http://api-docs.katalon.com/studio/v4.6.0.2/api/com/kms/katalon/core/webservice/keyword/WSBuiltInKeywords.html" rel="nofollow">Web Service Builtin Keywords</a></strong></td><td>List of Web Service built-in keywords</td></tr><tr><td><strong><a class="external-link" href="http://api-docs.katalon.com/studio/v4.6.0.2/api/com/kms/katalon/core/mobile/keyword/MobileBuiltInKeywords.html" rel="nofollow">Mobile Builtin Keywords</a></strong></td><td>List of Mobile built-in keywords</td></tr></tbody></table>
    
      
      
    
10.  Click on **Run** in the main toolbar to execute the test case.   
    ![](../../images/katalon-studio/docs/script-view/image2017-8-11 10_56_26.png)  
      
    Katalon Studio should be able to execute all the steps of the sample test case.