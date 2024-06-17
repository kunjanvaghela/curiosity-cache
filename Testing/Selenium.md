
# Basics:

Why Selenium:
1.        Free and open source
2.        Large user base and helping communities
3.        Cross browser compatibility
4.        Platform compatibility
5.        Multiple programming language support

Selenium Components:
1.        Selenium IDE (Integrated Development Environment)
2.        Selenium RC (Remote Control)  Selenium 1
3.        Selenium WebDriver)  Selenium 2 & 3
4.        Selenium Grid

Architecture:

|     |                                                                                                                                                              |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------- | --- | --- | --------------------------------------------------------------------------------------------------------------------------- | --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | --- | -------------------------------------------------------------------------------------------------------------------------------------------------- | --- | --- | --- | -------------------------------------------------------------------------------------------------------------------------------------------- | --- | --- | --- | --- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
|     |                                                                                                                                                              |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
|     | ![Text Box: Test Script](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image001.png)             |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     | ![Text Box: Webdriver API](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image002.png) |     |     |     | ![Text Box: Browser](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image003.png) |     |     |     |     |                                                                                                                                                    |
|     |                                                                                                                                                              | ![](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image004.png) |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
|     |                                                                                                                                                              |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
|     |                                                                                                                                                              |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
|     | ![Text Box: Selenium Client Library](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image005.png) |                                                                                                                             |     |     |                                                                                                                             |     | ![Text Box: JSON Wire Protocol over HTTP](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image006.png) |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     | ![Text Box: Real Browsers](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image007.png) |
|     |                                                                                                                                                              | ![](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image008.png) |     |     | ![](file:////Users/kunjanvaghela/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image009.png) |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
|     |                                                                                                                                                              |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
|     |                                                                                                                                                              |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
|     |                                                                                                                                                              |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |
|     |                                                                                                                                                              |                                                                                                                             |     |     |                                                                                                                             |     |                                                                                                                                                                   |     |                                                                                                                                                    |     |     |     |                                                                                                                                              |     |     |     |     |                                                                                                                                                    |

 

Browser Supported:
Chrome, IE/Edge, Firefox, Safari

Languages Supported:
Python, Ruby, Java, Javascript, C

Process to write automation test cases:
1.        Decide what to automate  The functionalities which can be automated
2.        Outline test scenarios:
		a. Input and Output for each scenario
		b. Determine the values/passing condition
3.        Find all the elements/locators needed for the test

Assert vs Verify
-              Assert:                  Execution stops if assert condition fails.
-              Verify:                    No halt in the test execution even though verify condition fails.
Note: No built-in features for verification in Selenium Webdriver


Soft Assert vs Hard Assert
-              Soft Assert:      collects error during execution, shows error in the end.
-              Hard Assert:    throws an AssertException immediately when an assert statement fails

  

# Selenium Webdriver

- Browser Automation Framework that accepts commands and sends them back to the webserver.
- Implemented through browser specific driver.
- Controls browser by directly communicating with it
- Supports: Java, C#, PHP, Python, Ruby, Perl

Geckodriver: Not for <2.53 Firefox version

Is FirefoxDriver a class or an interface?
A.       It is a class which implements the WebDriver interface  using **Dynamic Polymorphism**.

What is the super interface of the WebDriver?
A.       SearchContext

Explain: ‘Webdriver driver = new FirefoxDriver()’
A.       WebDriver is an interface and we are creating an object reference of type WebDriver instantiating an object of FirefoxDriver class.

Different Exceptions you have faced in Selenium WebDriver:
-              WebDriverException
-              TimeoutException
-              NoAlertPresentException
-              NoSuchWindowException
-              NoSuchElementException
-              TimeoutException
-              StaleElementRefereneException
-              IllegalStateException

To give username password on a popup window:
A.       Pass username and password with the URL. Example:
http://username:password@url
e.g.: [http://admin:admin123@abs.com](http://admin:admin123@abs.com)
Static Wait:       thread.sleep()


Types of Dynamic Wait in Selenium WebDriver
1.        Implicit Waits
		a. Wait for a certain amount of time before it throws an exception.
		b. Default setting: 0
2.        Explicit Waits
		a. Syntax: WebDriver Wait
3.        Fluent Waits
4.        PageLoadTimeOut

Waiting Strategies:
1)        Implicit waits – built-in way to automatically wait for elements. An implicit wait value can be set either with the timeouts capability in the browser options, or with a driver method. Global setting that applies to every element location call for the entire session.
2)        Explicit waits –



Locators:

class name       Locates elements whose class name contains the search value (compound class names are not permitted)

css selector     Locates elements matching a CSS selector

id                               Locates elements whose ID attribute matches the search value

name                     Locates elements whose NAME attribute matches the search value

link text                Locates anchor elements whose visible text matches the search value

partial link text                Locates anchor elements whose visible text contains the search value. If multiple elements are matching, only the first one will be selected.

tag name            Locates elements whose tag name matches the search value

xpath                      Locates elements matching an XPath expression

  

# Selenium Grid:

-              Tool used to run tests on different machines against different browsers in parallel.
-              Used to distribute the test execution on multiple platforms and environments concurrently.

Components -
1.        Hub:
	a. Central Server
	b. Where tests are executed
	c. One hub for grid instance  can be Linux/Windows/Mac
2.        Node:
a.        Registered on a Hub

b.        Where tests are run

c.        Can be any platform

d.        Many nodes in a grid instance

Benefits:

1.        Parallel Testing: Allows tests to be run concurrently

2.        Multi-browser and multi-platform testing

3.        Smart routing between hubs and nodes

4.        Manages multiple connections

Pros:

1.        Scaling –

a.        Distribute tests on several machines

b.        Can run tests in parallel

2.        Central Management

a.        Run tests against large number of browsers and platforms (OSs).

3.        Smart –

a.        Finds specified nodes quickly and easily

b.        Routes test scripts to the correct node

Cones:

1.        Maintainability –

a.        Required to keep the hub and nodes running smoothly

b.        For better maintaining:

                                                                                             i.         Enable warning and logs for easy debugging

                                                                                          ii.         Creating scripts to manage grid for common behavior like starting and stopping.

2.        Performance –

a.        Tests can start to degrade in performance over time due to for ex, stale browsers.

b.        For better performance:

                                                                                             i.         Explicitly kill browser after tests

                                                                                          ii.         Restart nodes periodically

                                                                                       iii.         Restart server

  

Page Object Model

1.        A class for each page in the app

2.        Each page has:

a.        Selectors/Locators

b.        Methods

3.        Goals:

a.        Separation of test and code

b.        More maintainable test code

  

Important Methods/Functions:

1.        .sendKeys():     Input text in textbox.

2.        .click():                 To click on the element

3.        .clear():                To clear the element

4.        .getText():           to get text of any element

5.        .getAttribute(<attributename>):         to get value of the attribute

6.        By.linkText(‘’).click():                    To click on a hyperlink

7.        By.partialLinkText(‘’).click():  To click on a hyperlink

8.        driver.findElement(By.id(<formName>).submit()): To submit a form

9.        driver.findElement(By.xpath(<xpath>)).sendKeys(Keys.ENTER): To click enter

10.  driver.getCurrentUrl():                Get the current URL.

11.  driver.manage().window().maximize():            Maximize window.

Without using sendKeys(), how to input into an element: using JavascriptExecutor

Navigate back and forth in a browser using Selenium WebDriver:

1.        driver.navigate().forward():     to navigate to the next web page.

2.        driver.navigate().back():            to navigate to the previous web page.

3.        driver.navigate().refresh():      to refresh the current web page  risky as whole DOM is loaded again. Prone to StaleElementException.

4.        driver.navigate().to(<url>):      to launch a web browser window & navigate to specified URL.

Different ways to open web pages:

1.        driver.get(<url>):            Opens & waits till page gets loaded.

2.        Driver.navigate.get()/to():         Opens but does not wait till the whole page gets loaded.

Different ways to refresh a webpage:

1.        driver.navigate().refresh()

2.        driver.get(<url>)

3.        driver.navigate().to(<URL>)

4.        sendKeys(Keys.F5)  on any textbox on the webpage

Difference between:

1.        driver.getWindowHandle()  returns handle of the current page (a unique identifier).

2.        driver.getWindowHandles()  returns a set of handles of all the pages available.

Difference between:

1.        driver.close()               closes current WebDriver instance

2.        driver.quit()                   close all the opened WebDriver instances

Difference between:

1.        driver.findElement()     returns a single WebElement (found first) based on the locator, NoSuchElementException triggered if no element found.

2.        driver.findElements()  returns a list of WebElements, returns a list of 0 elements if no element found.

Check if an element is displayed on the web page?

1.        isDisplayed()

2.        isSelected()      only for list object (radio buttons, drop downs, and checkboxes).

3.        isEnabled()        returns False if not selected.

**How to select a value in dropdown?**

A.       By using a Select class. Example:

WebElement mySelectElement = driver.getElement(By.name(“dropdown”));

Select dropdown = new Select(mySelectElement);

dropdown.selectByVisibleText(<text>)

dropdown.selectByIndex(<index>)

dropdown.selectByValue(<Value>)

How to capture screenshot using Selenium WebDriver?

A.       By using ‘TakeScreenshot’ interface

How to mouse hover on a web element using WebDriver?

A.       By using **Actions** class.

Handling different windows:

1.        driver.current_window_handle  To get the ID of the original window

2.        driver.switch_to.new_window('tab')

3.        driver.switch_to.new_window('window')

4.        driver.switch_to.window(original_window)  Switches to the specified window

Reading Excel

1.        openpyxl.load_workbook(<path>)

2.        pandas.read_excel(<path>)

Automating Captchas using Selenium?

A.       Not possible, maybe through 3rd party APIs.

What cant we automate using Selenium:

1.        Captcha solving

2.        Windows OS based pop-ups (not file upload)

3.        Mobile application based

Uploading file:

A.       For input type ‘file’, directly send file path using .sendKeys(<path>)

RightClick:        ActionChains(driver).context_click(<element>).perform()

  

Challenges faced using Selenium

1.        Changing requirements

2.        No way to deal with captcha

3.        Difficult to identify dynamic objects, locator shifting

4.        Cant support non-web based

5.        Dealing with AJAX components

a.        After page is loaded

b.        When particular check-box is selected triggering another component/element load. For example state list load on country select.

6.        Cross-browser testing issues Code must be compatible with all the browsers