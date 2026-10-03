# Build-a-Java-App-with-Gradle-through-GitHub-Actions
Build a Java App with Gradle, then build a Docker image after it passes through GitHub Actions and push it to a Docker repository on Docker Hub.


# Challenges met during the Project
1- Many of the dependencies were deprecated (like OpenJDK), and I had to update them manually to a newer version or replace them entirely (Eclipse Temurin), as they are no longer in use.
I took the Gradle Java app from an old repo; hence the required update because GitHub will, most of the time, flag a failure.

2- Some of the placeholders in the code needed to be reconfigured, and this alone created some failures during the testing phase.

3- At one point, I had to stop the running action because the daemon hung for 14min and had to restart the action. I have also applied a timeout of 10 minutes instead to not wait for too long.
