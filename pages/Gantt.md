---
layout: default
title: Gantt Chart
nav_order: 5
---

# Comment Anywhere Gantt Chart

The following chart describes the implementation timeline for Comment Anywhere for Spring of 2023.

The project will be turned in on April 21st, 2023 and we will present on April 28th, 2023.


![gantt chart timeline for comment anywhere]({{site.url}}/assets/images/Gantt_Chart.png)
[Download the Comment Anywhere Gantt chart pdf]({{site.url}}/assets/pdfs/Gantt_Chart.pdf)

## Gantt Chart tasks, detailed explanations :

1. Set up the Git repository, readme, and directory structure.

2. Create the necessary compilation files, such as the docker file, makefile, package.json, tsconfig.json, manifest.json, and webpack.config.js.
 - the docker file(s) configure how docker containers are constructed and deployed.
 - the [makefile](https://makefiletutorial.com/#makefile-syntax) configures compilation, deployment, and test commands.
 - [package.json](https://docs.npmjs.com/cli/v7/configuring-npm/package-json) configures typescript, webpack, and other npm extensions needed for transpiling the front end.
 - [webpack.config.js](https://webpack.js.org/configuration/) webpack.config.js configures how the source typescript files are 'packed' into javascript files.
 - [manifest.json](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json) manifest.json configures the extension to work with browsers.

3. Stub some basic functions for the back end to ensure basic running of Server and Database and cross-module communication.

4. Implement one full message chain to ensure that the Front End can indeed communicate with the back end.
 - More information about message chains can be found in the [design document]({{site.url}}/pages/design.html).

5. Stub all the Go functions for the back end. No actual code is written, only the signatures across the board. It’s refined until no errors are appearing. Copy the information from the design document into comments on the code.

6. Stub all functions for the front end in the same way. (Can be simultaneous to back end)

7. Write the methods, simultaneously writing a parallel testMethod. Unit test each message and integration test each message chain until it 
is working properly.

    1. The database.generated.Queries class will need to be completed by writing sqlc code and unit tests before most other back end classes and methods can be properly tested.

    2. Account creation and management will need to precede the implementation of certain other features.

8.  Deploy the back end on the cloud, acceptance test, and release the extension as a downloadable from a statically hosted github page.

9.  Submit the extension to the Mozilla and Chrome marketplaces for review.
 - This will occur after the end of the semester. Acceptance into the marketplaces is not an enumerated specification. If acceptance does not occur, we will ultimately self-host and deploy only on our static page.

10.  Restyle the frontend.
 - This is a continuous, interative process that will continue as we develop in an effort to make the extension as user-friendly and attractive as possible.