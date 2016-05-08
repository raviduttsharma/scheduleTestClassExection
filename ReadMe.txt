Schedule your test classes to run daily

Many of the projects have a common problem of test coverage when the time for production deployment comes. Generally the development and maintenence of test classes do not go hand in hand with development and maintenence of apex classes. And when the time of deployment comes, you find the your code coverage is below 75%. Usually developers makes changes to code but forgets to make the required changes in test classes. To avoid such scenarios, you can schedule your test classes to run daily and send out the status email to developers so that the test classes are fixed whenever code changes are done.

How to make this work :
You can download all the classes and copy in in your Salesforce org. Schedule the class named "TestClassScheduler" to run daily or weekly as per your requirement. Before scheduling, change the email address in sendEmail method present in TestClassUtils class.