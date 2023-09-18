# Split the chat phrases
The following is a Kata, an exercise in coding, refactoring and test-first.

The goal is to solve the exercise in your own best way, showing us how you approch problems and your workflow. We may give more value to how you reached the solution with respect to the solution itself.

## Before you start
* Try not to read ahead.
* Do one task at a time. The trick is to learn to work incrementally.
* Commit your code on GitHub or any other SCM repository you prefer.
* Release your work under an OSI-approved open-source license of your choice.
* Disable Copylot and don't watch others solutions while trying to solve this kata, you'll make it harder for us to asses your skills.

## Description

The goal is to build different Docker images and run containers to implement a HTTP web service.

## The Kata

### Step 1 (Docker web service)
Create a Docker image that implements a WEB server able to expose static HTML files. The HTML files will be opened through a browser after a container based on this image stars. The HTML pages will be included in the Docker image.
Run a Docker container based on this image.


### Step 2 (Multiple Docker web services)
Modify the previous image so that the HTML contents are loaded at run time. Run two containers that use the same image but that expose two different index.html pages


### Step 3 (HTTP proxy)
Create a Docker image that implements a HTTP proxy server. Run a container based as on this image so that it will be possible to navigate on different HTTP pages, related to the two different containers started at step 2, changing the browser URL.

### Step 4 [Extra] (HTTPs support)
Modify the image implemented at step 3 so that the proxy server will be reachable through HTTPs protocol.


### Step 5 (Load balancing and HA)
Run different containers based on previous images with following requirements:
 * Run two containers that serve the same HTML pages
 * The HTML pages are reachable through a browser using a specific URL
 * Even if one of the containers is stopped, the HTTP pages will be reachable anyway.
 * If both containers are stopped then, when trying to access HTML pages via the browser, a custom error will be displayed


**IMPORTANT:** Provide a README for all step with instructions on how to build tun and test the environment.

**CODE SUBMISSION:** Add the code to your own Github account and send us the link.
