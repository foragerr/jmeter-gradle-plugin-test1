# jmeter-gradle-plugin-test1
Simple gradle project to demonstrate issue [kulya/jmeter-gradle-plugin#37](https://github.com/kulya/jmeter-gradle-plugin/issues/37)

To reproduce the issue, run `gradle jmeterRun` This executes the test plan nonDefaultLocation.jmx as specified in build.gradle
  
    jmeterTestFiles = [file("src/test/resources/nonDefaultLocation.jmx")]

running 'gradle jmeterListTestPlan' however does not list this test plan, lists DefaultLocation.jmx instead

