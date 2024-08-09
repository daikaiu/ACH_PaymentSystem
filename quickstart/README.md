# Square Java SDK Quickstart

This quickstart sample creates a Square client instance with your Square access token and then lists the locations in your account.
The sample is based on the [Java SDK Quickstart guide](https://developer.squareup.com/docs/sdks/java/quick-start).

## Setup

[Install Java Guide](https://www.java.com/en/download/help/download_options.html) - If you don't have java already installed on your machine.

[Maven Install Guide](https://maven.apache.org/install.html)
**note**: Gradle is also supported but the quickstart here demonstrates using Maven. 

## Quickstart instructions

1. Change into the `quickstart` directory

1. Copy the example config file in `src/main/resources`, and place your `Square Access Token` inside of the new file.

    ```
    $ cp src/main/resources/config.properties.example src/main/resources/config.properties
    ```

1. Replace `PLACE_VERSION_HERE` with the latest SDK version from [here](https://developer.squareup.com/docs/sdks/java)

1. Compile the program
    ```
    $ mvn package -DskipTests
    ```

1. Execute the code
    ```
    $ mvn exec:java -Dexec.mainClass="com.square.examples.Quickstart"
    ```

1. In your console, you should see output similar to this:
    ```
    Location(s) for this account:
    LGJ1WWJ8PSV8Z: Default Test Account, 1600 Pennsylvania Ave NW, Washington
    ```

## Resources

[Square Java SDK Guide](https://developer.squareup.com/docs/sdks/java/using-java-sdk) - details on how to use / configure the Square client.

[Maven Repository for Square](https://mvnrepository.com/artifact/com.squareup/square) - Where the package files are hosted

[Java SDK Source Code](https://github.com/square/square-java-sdk) - Github repo with sdk source code