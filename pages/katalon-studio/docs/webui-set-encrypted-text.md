---
title: "[WebUI] Set Encrypted Text" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/webui-set-encrypted-text.html 
redirect_from: "/display/KD/%5BWebUI%5D+Set+Encrypted+Text" 
description: 
---
Description
-----------

Set encrypted text into an input field. It also clears the previous value of the input field. To encrypt raw text, go to **Help > Encrypt Text**.

_Manual mode_

The pop-up dialog has been shown when calling keyword “**Set Encrypted Text**”. Input raw text and select insert.

**_Script Mode_**

Go to **Help > Encrypt Text**, input raw text to encrypt. Next, copy and paste encrypted text into the test scripts.

 Parameters
-----------

<table><thead><tr><th><div class="tablesorter-header-inner">Param</div></th><th><div class="tablesorter-header-inner">Param Type</div></th><th><div class="tablesorter-header-inner">Mandatory</div></th><th><div class="tablesorter-header-inner">Description</div></th></tr></thead><tbody><tr><td><span>to&nbsp;</span></td><td><span>TestObject</span></td><td><span>Required</span></td><td><span>Represent a web element.</span></td></tr><tr><td><span>text</span></td><td><span>String</span></td><td><span><span>Required</span></span></td><td><span><span><span>The encrypted text.</span></span></span></td></tr><tr><td><span><span>flowControl</span></span></td><td><span><span>FailureHandling</span></span></td><td><span>Optional</span></td><td><span>Spec</span><span>ify </span><a href="https://docs.katalon.com/x/qAAM" rel="nofollow">failure handling</a><span> schema to determine whether the execution should be allowed to continue or stop.</span></td></tr></tbody></table>

Example
-------

Set the encrypted text to txt_Password of a login form.

```groovy
'Open browser and navigate to AUT'
WebUI.openBrowser('http://demoaut.katalon.com/profile.php#login')

'Input username'
WebUI.setText(findTestObject('Page_Login/txt_UserName'), 'John Doe')

'Input password'
WebUI.setEncryptedText(findTestObject('Page_Login/txt_Password'), 'g3/DOGG74jC3Flrr3yH+3D/yKbOqqUNM')

'Click on "Login" button'
WebUI.click(findTestObject('Page_Login/btn_Login'))

'Close browser'
WebUI.closeBrowser()
```