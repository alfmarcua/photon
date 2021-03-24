Submit a new issue only if you are sure it is a missing feature or a bug. Otherwise please discuss the topic in the [mailing list](https://lists.openstreetmap.org/listinfo/photon) first. 

## We love pull requests. Here's a quick guide:

1. [Fork the repo](https://help.github.com/articles/fork-a-repo) and create a branch for your new feature or bug fix.

2. Run the tests. We only take pull requests with passing tests: `mvn clean test`

3. Add at least one test for your change. Only refactoring and documentation changes
require no new tests. Also make sure you submit a change specific to exactly one issue. If you have ideas for multiple 
changes please create separate pull requests.

4. Make the test(s) pass.

5. Push to your fork and [submit a pull request](https://help.github.com/articles/using-pull-requests). A button should
appear on your fork its github page afterwards.

## Code formatting

We use IntelliJ defaults and a very similar configuration for NetBeans defined in the root pom.xml. For eclipse there is this [configuration](https://github.com/graphhopper/graphhopper/files/481920/GraphHopper.Formatter.zip). Also for other IDEs 
it should be simple to match:

 * Java indent is 4 spaces
 * Line width is 100 characters
 * The rest is left to Java coding standards but disable "auto-format on save" to prevent unnecessary format changes. 
 * Currently we do not care about import section that much, avoid changing it
 * Unix line endings (should be handled via git)

And in case we didn't emphasize it enough: we love tests!

## Installation

photon requires java, at least version 8.

In order to develop with an IDE, you need to install [lombok](https://projectlombok.org/). For example, for eclipse:

1. Download [lombok.jar](https://projectlombok.org/download)
2. Execute `java -jar lombok.jar` to start lombok installer
3. Specify eclipse location path and click "Install/Update"
4. Check that `-javaagent` has been added to the ini file of eclipse specifying the path of `lombok.jar`.
