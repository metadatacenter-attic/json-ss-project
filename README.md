## Mapping Master Build Project

This project contains a Maven POM that builds JSON-SS-related components.
Currently it builds the [core JSON-SS](https://github.com/metadatacenter/json-ss.git) project 
and the [JSON-SS Itegration Tests](https://github.com/metadatacenter/json-ss-integration-tests.git) project.

#### Prerequisites

To run the build process in this project, you must have the following items installed:

+ A tool for checking out a [Git](http://git-scm.com/) repository.
+ Apache's [Maven](http://maven.apache.org/index.html).

#### Building

Create a suitable local directory and then clone the Mapping Master-related projects as follows:

    git clone https://github.com/metadatacenter/json-ss.git
    git clone https://github.com/metadatacenter/json-ss-integration-tests.git
    git clone https://github.com/metadatacenter/json-ss-project.git

Change into the JSON-SS project directory:

    cd json-ss-project

And then build everything with Maven:

    mvn clean install

The JSON-SS integration tests can take quite a while to run. You can skip them as follows:

    mvn -DskipTests=true clean install

Documentation for JSON-SS can be found [here](https://github.com/metadatacenter/json-ss/wiki).

