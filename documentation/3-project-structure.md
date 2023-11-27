# Project Structure

## Overview
A Robot Framework project consist of requires below list:

1. An Editor
    1. IDEs - Pycharm, VS Code, Eclipse, Sublime text
    2. RIDE (explicitly created for Robot Framework's scripting but not recommended as it doesn't have the advanced and mature capabilities that of IDEs)
    3. Notepad
2. Robot Framework Script Formats
    1. Space Separated (2-4 spaces, or tabs, etc.)
    2. Pipe Delimited (using pipe character **“|”** as separator)
3. Keyword-Driven (type plain English keywords to invoke pre-written logic that might be other keywords or even Python script that lives in pre-written libraries)
4. Natural Language (Business Domain - meaning that the test steps will reflect capabilities that our system under test can perform)


- The test script is going to hold your test cases. and your test cases are going to talk to an app keyword file.
- The app keyword file is going to hold high level chunky keywords that you create, and those keywords will represent various capabilities your system under test can perform. The keywords in the keyword file are then going to talk to page object files.
- The page object files are going to be containers that encapsulate the locators and more granular keywords that are specific to different pages of your system under test. Also, the page object keywords are going to then talk to the various libraries.
- The various libraries are going to be downloaded and the selenium web drivers are binary files that we've installed and those are the bridge between the Selenium library and the browser.

## File Organization
- **/ProjectBase** <-- main project file
  - /Tests 
    - Product_Home.robot <-- homepage tests
    - Product_Login.robot <-- landing page tests
  - **/Resources**
    - common.robot (Suit Setup, Open Browser, etc.)
    - /ProductOne
      - ProductApp.robot <-- app keyword files (app capabilities)
      - /PO
        - Home.robot <-- home page-specific locators and keywords
        - Login-robot <-- login page-specific locators and keywords
        - TopNav.robot <-- login page-specific locators and keywords
  - **/Libraries** <-- custom libraries written with Python
  - **/Result** <-- result logs from each run
    - /ProductOne
    - /ProductTwo ... 

