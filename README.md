# data-stack

## Download Jars from Maven Central Repository
### Overview

This documentation describes how to download jar files from the Maven Central Repository using `wget` and install them into the `container/jars` folder. The `container/jars` folder is used to store external JAR files.

### Prerequisites

Before you begin, you must have the following:

- A working installation of `wget` on your local machine.
- Access to the internet to download jar files from the Maven Central Repository.

### Steps

Follow these steps to download jar files from the Maven Central Repository using `wget` and install them into the `container/jars` folder.

1. Open a terminal window on your local machine.

2. Navigate to the root directory of the project.

3. Create the `container/jars` folder if it does not already exist. You can do this by running the following command:

```shell
mkdir -p container/jars
```

4. Identify the Maven Central Repository URL for the JAR file you want to download. For example, if you want to download the `spark-sql-kafka-0-10` JAR file, you can find the URL on the [Maven Central Repository website](https://mvnrepository.com/).

5. Use the `wget` command to download the JAR file from the Maven Central Repository. Replace `<URL>` with the actual URL of the JAR file. For example:

```shell
wget -O container/jars/spark-sql-kafka-0-10_2.12-3.5.1.jar <URL>
```

6. Repeat steps 4 and 5 for each JAR file you want to download and install into the `container/jars` folder.

7. Verify that the JAR files have been downloaded and installed into the `container/jars` folder by listing the contents of the folder:

```shell
ls container/jars
```
