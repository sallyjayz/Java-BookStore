Installation
Before starting, make sure you install JDK and Maven. Follow the installation videos above if you need help.

Running Your App
To run your app, first open up a terminal window and cd into your project directory. Then type the following command to install and run your project on a Tomcat server:

mvn clean install tomcat7:run
Once that is running the terminal should display something similar to the following:

INFO: Starting Servlet Engine: Apache Tomcat/7.0.47
May 21, 2018 10:22:35 PM org.apache.coyote.AbstractProtocol start
INFO: Starting ProtocolHandler ["http-bio-8080"]
Previewing Your Work
In order to see your changes in a browser, make sure Tomcat is still running in your terminal, and visit http://localhost:8080/books/list in a browser to see the app running.

Running Tests
To run tests, run the following command: (Note: terminate the run process above first, with ctrl c, since the tests run on the same port)

mvn -P integration verify
Running that command should show you the failing tests. This is good! We'll be fixing these tests once we jump into the build step. As you move through the modules, you can run module-specific tests that are shown above the tasks in each module.