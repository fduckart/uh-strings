A Java String utility class.


##### Build Tool
First, you need to download and install maven (version 3.2.3+).

Be sure to set up a M2_REPO environment variable.

##### Java
You'll need a Java JDK to build and run the project (version 1.8).

The files for the project are kept in a code repository,
available from here:

https://github.com/fduckart/uh-strings

##### Building
Install the necessary project dependencies:

    $ mvn install

To build a jar file for use:

    $ mvn clean package

You should have a jar file in the target directory.

##### Running Unit Tests
The project includes Unit Tests for various parts of the system.
For this project, Unit Tests are defined as those tests that will
rely on only the local development computer.
A development build of the application will run the Unit Tests.
The test build of the application is configured to run both the
Unit Tests and the System Tests (which may require network access).
The production build does not run any tests. 

You can also run specific Unit Tests using the appropriate command
line arguments.

To run the Unit Tests with a standard build:

    $ mvn clean test

To run a test class:

    $ mvn clean test -Dtest=StringsTest

To run a single method in a test class:

    $ mvn clean test -Dtest=StringsTest#trunctate
