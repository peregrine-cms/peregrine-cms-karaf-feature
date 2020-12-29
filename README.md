# Peregrine CMS Karaf Feature

This project is a feature definition for Peregrine CMS.

## Install Apache Karaf

See [Apache Karaf Quickstart](https://karaf.apache.org/manual/latest/quick-start.html).

## Install Apache Sling Feature

See [Running Apache Sling on Apache Karaf](Running Apache Sling on Apache Karaf)

## Install Peregrine Feature

NOTE: Since Peregrine is not yet available on a public Maven respository, you will need to build Peregrine l
ocally so that Karaf can pull the build artifacts from your local .m2 repository.

1. Build this project.

        $ mvn clean install

2. Log into the Karaf shell add the Peregrine repository, then install Peregrine as a feature.

        karaf@root()> feature:repo-add mvn:com.peregrine-cms/peregrine-feature/1.0-SNAPSHOT/xml/features
        karaf@root()> feature:install peregrine
