---
title: "[Mobile] Wait For Element Has Attribute" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/mobile-wait-for-element-has-attribute.html 
redirect_from: "/display/KD/%5BMobile%5D+Wait+For+Element+Has+Attribute" 
description: 
---
Description
-----------

Wait until the given mobile element has an attribute with the specified name.

Parameters
----------

<table><thead><tr><th>Param</th><th>Param Type</th><th>Mandatory</th><th>Description</th></tr></thead><tbody><tr><td><span>to</span></td><td>TestObject</td><td>Required</td><td><p><span>Represent a mobile element.</span></p></td></tr><tr><td><span>attributeName</span></td><td>String</td><td>Required</td><td><span>The name of the attribute to wait for.</span></td></tr><tr><td>timeout</td><td>int</td><td>Required</td><td><span>System will wait at most timeout (seconds) to return a result</span></td></tr><tr><td><span>flowControl</span></td><td>FailureHandling</td><td>Optional</td><td><span>Spec</span><span>ify </span><a href="https://docs.katalon.com/x/qAAM" rel="nofollow">failure handling</a><span> schema to determine whether the execution should be allowed to continue or stop.</span></td></tr></tbody></table>

Returns
-------

<table><thead><tr><th>Param Type</th><th>Description</th></tr></thead><tbody><tr><td>boolean</td><td><ul><li><strong>true:</strong> the element has the attribute with the specified name.</li><li><strong>false: </strong>the element doesn't have the attribute with the specified name.</li></ul></td></tr></tbody></table>

Example
-------

You want to wait for 'App' button has 'class' attribute.

```groovy
import static com.kms.katalon.core.testcase.TestCaseFactory.findTestCase
import static com.kms.katalon.core.testdata.TestDataFactory.findTestData
import static com.kms.katalon.core.testobject.ObjectRepository.findTestObject
import internal.GlobalVariable as GlobalVariable
import com.kms.katalon.core.configuration.RunConfiguration as RunConfiguration
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as Mobile
import com.kms.katalon.core.util.internal.PathUtil as PathUtil
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUI
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WS
import static com.kms.katalon.core.checkpoint.CheckpointFactory.findCheckpoint
import com.kms.katalon.core.model.FailureHandling as FailureHandling
import com.kms.katalon.core.testcase.TestCase as TestCase
import com.kms.katalon.core.testdata.TestData as TestData
import com.kms.katalon.core.testobject.TestObject as TestObject
import com.kms.katalon.core.checkpoint.Checkpoint as Checkpoint

'Start application on current selected android\'s device'
Mobile.startApplication(GlobalVariable.G_AndroidApp, false)

'Wait until app control has class atribute'
Mobile.waitForElementHasAttribute(findTestObject(findTestObject('Object Repository/Application/android.widget.TextView - App')), 'class', 20)

'Close application on current selected android\'s device'
Mobile.closeApplication()
```

###### Wait until the given web element has an attribute with the specific name

###### Parameters:  

*   to - TestObject (required): represent a mobile element
    
*   attributeName - String (required): the name of the attribute to verify
    
*   timeOut - int (required): \- system will wait at most timeout (seconds) to return result
    
*   flowControl - FailureHandling (optional): specify failure handling schema to determine whether the execution should be allowed to continue or stop. More details is in this page: [Failure Handling](/display/KD/Failure+Handling)

#### Returns

**true** if element has the attribute with the specific name; otherwise, **false**

#### Example: You want to wait until the button has an attribute with name = 'class'

Manual: 

** ![](../../images/katalon-studio/docs/mobile-wait-for-element-has-attribute/image2016-8-15 19_2_59.png)**

Script:

```groovy
Mobile.waitForElementHasAttribute(findTestObject('SampleApp.apk/android.widget.Button - Button0'), 'class', 10)
```