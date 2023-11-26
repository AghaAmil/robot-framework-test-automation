# Project Files and Script Layers
- The test script is going to hold your test cases.
- The app keyword file is going to hold high level chunky keywords that you create, and those keywords will represent various capabilities your system under test can perform,
- The page object files are going to be containers that encapsulate the locators and keywords that are specific to different pages of your system.
- of course, the various libraries are going to be downloaded
- The selenium web drivers are binary files that we've installed and those are the bridge between the Selenium library and the browser.

So from a folder structure standpoint, our test script is going to go under a test directory while the app keyword file and all your page objects are going to go into a resource folder. And of course in the installation section you might recall that we placed our selenium web drivers into a C bin directory. 
