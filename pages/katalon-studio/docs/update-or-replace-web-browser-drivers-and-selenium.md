---
title: "Update or Replace Web Browser Drivers and Selenium" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/update-or-replace-web-browser-drivers-and-selenium.html 
redirect_from: "/display/KD/Update+or+Replace+Web+Browser+Drivers+and+Selenium" 
description: 
---
For manually replacing and updating other versions of WebDrivers and Selenium, please refer to this [guide](https://docs.katalon.com/x/1xtO). 

> Katalon Studio team strongly suggest users **NOT** to manually replace or update any WebDrivers. Any changes in drivers may cause runtime bugs for Katalon Studio application.

<table><thead><tr><th>Katalon Studio V5.1.0</th><th>How to Replace&nbsp;</th></tr></thead><tbody><tr><td>&nbsp;</td><td><strong>Windows</strong></td><td><strong>MAC OSX</strong></td></tr><tr><td>Selenium <a class="external-link" href="https://raw.githubusercontent.com/SeleniumHQ/selenium/master/java/CHANGELOG" rel="nofollow">3.7.1</a></td><td><ul><li><strong>Download </strong>the desired Selenium version <a class="external-link" href="http://selenium-release.storage.googleapis.com/index.html" rel="nofollow">here</a> (<span>Select </span><strong>only</strong><span> Selenium 3.0+ and higher version than 3.7.1)</span></li><li><span><strong>Delete</strong> existing selenium-server-standalone-3.x.jar</span><span><br></span></li><li><span><strong>Copy</strong> preferred <strong>driver</strong> into this folder</span><br>&lt;Katalon Studio folder&gt;\configuration\resources\lib</li></ul></td><td><p>&nbsp;</p><ul><li>&nbsp;/Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/lib</li></ul></td></tr><tr><td>Chromedriver <a class="external-link" href="https://chromedriver.storage.googleapis.com/2.33/notes.txt" rel="nofollow">2.33</a></td><td><div class="content-wrapper"><ul><li><strong>Download </strong>preferred Chromedriver <a class="external-link" href="https://sites.google.com/a/chromium.org/chromedriver/downloads" rel="nofollow">here</a></li><li><strong>Copy</strong> downloaded Chromedriver and <strong>paste</strong> into Katalon Studio folder</li></ul><div class="confluence-information-macro confluence-information-macro-information conf-macro output-block" data-hasbody="true" data-macro-name="info"><blockquote class="important"><span class="aui-icon aui-icon-small aui-iconfont-info confluence-information-macro-icon"></span><div class="confluence-information-macro-body"><p>You can use 32-bit Windows Chromedriver for both 32-bit and 64-bit Windows.</p></div></blockquote></div><ul><li><ul><li>&lt;Katalon Studiofolder&gt;\configuration\resources\drivers\chromedriver_win32</li><li>&lt;Katalon Studiofolder&gt;\configuration\resources\drivers\chromedriver_win64</li></ul></li></ul></div></td><td><p>&nbsp;</p><ul><li>/Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/drivers/chromedriver_mac</li></ul></td></tr><tr><td>Firefox (Gecko Driver) <a class="external-link" href="https://github.com/mozilla/geckodriver/releases/tag/v0.19.0" rel="nofollow">0.19</a></td><td><ul><li><strong>Download </strong>preferred Gecko Driver <a class="external-link" href="https://github.com/mozilla/geckodriver/releases" rel="nofollow">here</a><span><strong><br></strong></span></li><li><span><strong>Copy</strong><span> downloaded Gecko driver and </span><strong>paste</strong><span> into Katalon Studio folder</span></span><ul><li><span>&lt;Katalon Studio folder&gt;\configuration\resources\drivers\firefox_win32</span></li><li>&lt;Katalon Studio folder&gt;\configuration\resources\drivers\firefox_win64</li></ul></li></ul></td><td><p>&nbsp;</p><ul><li>/Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/drivers/firefox_mac</li></ul></td></tr><tr><td>IEDriverServer <a class="external-link" href="https://raw.githubusercontent.com/SeleniumHQ/selenium/master/cpp/iedriverserver/CHANGELOG" rel="nofollow">3.6.0</a></td><td><ul><li>Download preferred IEDriver <a class="external-link" href="http://selenium-release.storage.googleapis.com/index.html" rel="nofollow">here</a></li><li><strong>Copy</strong><span> downloaded IEDriverServer and </span><strong>paste</strong><span> into Katalon Studio folder</span></li><li>&lt;Katalon Studio folder&gt;\configuration\resources\drivers\iedriver_win32</li><li>&lt;Katalon Studio folder&gt;\configuration\resources\drivers\iedriver_win64</li></ul></td><td>&nbsp;</td></tr></tbody></table>