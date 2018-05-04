# onewebsite

## Team
Varnit Tewari

## Prerequisites
-Java 8
-Maven

## Git Commit Format
Commits should not be past tense. Please use git command structure like tenses

eg. create new file, add changes, remove file

## How to run it
Clone the repository and go to the root directory.
Execute mvn compile exec:java
Open in your browser http://localhost:4567/

## How to test it
The Maven build script provides hooks for run unit tests and generate code coverage reports in HTML.

## To run tests on all tiers together do this:

Execute mvn clean test jacoco:report
Open in your browser the file at PROJECT_HOME/target/site/jacoco/index.html

## To run tests on each tier in isolation do this:

Execute mvn clean exec:exec@tests-and-coverage

## To view the Model tier tests open in your browser the file at PROJECT_HOME/target/site/jacoco/model/index.html
## To view the Application tier tests open in your browser the file at PROJECT_HOME/target/site/jacoco/appl/index.html
## To view the UI tier tests open in your browser the file at PROJECT_HOME/target/site/jacoco/ui/index.html

## How to generate the Design documentation PDF
Execute mvn exec:exec@docs
The generated PDF will be in PROJECT_HOME/target/ directory

## How to archive the project
Execute mvn exec:exec@zip
The generated zipfile will be in ``PROJECT_HOME/target/` directory

License
MIT License

See LICENSE for details.
