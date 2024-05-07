# Get Started

[Install Java Guide](https://www.java.com/en/download/help/download_options.html) - If you don't have java already installed on your machine.

[Maven Install Guide](https://maven.apache.org/install.html)
**note**: Gradle is also supported but the quickstart here demonstrates using Maven. 

[Square SDK Guide](https://developer.squareup.com/docs/sdks/java/using-java-sdk) - details on how to use / configure the Square client.

[Java Quickstart guide](https://developer.squareup.com/docs/sdks/java/quick-start) - The quickstart directory is based off of this document.


## Quickstart instructions

Change into the `quickstart` directory

Copy the example config file in `src/main/resources`, and place your `Square Access Token` inside of the new file.

```
$ cp src/main/resources/config.properties.example src/main/resources/config.properties
```

Compile the program
```
$ mvn package -DskipTests
```

Execute the code
```
$ mvn exec:java -Dexec.mainClass="com.square.examples.Quickstart"
```

You should see your `Square Sandbox Seller account's` location logged in the console.