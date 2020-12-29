# Peregrine Karaf Feature

## Installation

1. Build this project.

        $ mvn clean install

2. Log into Karaf and run:

        feature:repo-add mvn:com.peregrine-cms/peregrine-feature/1.0-SNAPSHOT/xml/features
        feature:install peregrine
