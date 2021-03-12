Concepts Included:

- Shared state across cucumber step definitions
- Page Object pattern
- Common web page interaction methods(Browser Utils)
- Common api interaction methods(Rest Services)
- Externalised test configuration(qa.properties, dev.properties, demo.properties)
- Commonly used test utility classes(Utilities package)

Tools:
- Java
- Maven
- Cucumber
- Selenium Webdriver -> UI 
- JUnit -> Assertion Lib
- REST Assured -> API


Required Installations:
- Java 13
- Maven 4.0
- Chrome and Chrome driver (UI tests use Chrome by default, can be changed in config)

Reporting:
- Reports are written into /target directory after a successful run.
- Tests result in a HTML report for each feature in cucumber-html-reports/overview-features.html.
- In the case of test failures, a screen-shot of the UI at the point of failure is embedded into the report.

Usage:
- In order to run the test please use terminal command:

mvn clean verify -Dcucumber.options="--tags @smoke_test" -Dbrowser=chrome -Denv=QA

- Please provide test tag for desired scenario, browser and environment.


WIP:
- Parallel test runs
- DB connection
- Jenkins integration
