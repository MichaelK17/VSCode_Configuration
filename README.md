# VSCode_Configuration
## How to configure java files and junit tests to VSCode

To get VS Code working correctly for your Java project (especially for testing), we addressed these configuration issues:

Java Extensions: Installed the "Extension Pack for Java" (published by Microsoft). This pack includes essential tools like the Java language server, debugger, and, importantly, the "Test Runner for Java".
Source/Test Path Configuration: Ensured VS Code correctly identified src/main as the folder for main source code and src/test as the folder for test code. This involved using VS Code's Java project configuration tools (like the "Java Projects" view or editing the .classpath file) to explicitly mark src/test as the test source root.
JUnit Library: Added the JUnit 5 JAR file to the project's "Referenced Libraries" so VS Code could resolve the import org.junit... statements and understand the test annotations (@Test, etc.). This was done using the Java extension's classpath configuration features.
Extension Updates: Ensured the Java extensions (specifically the Red Hat language support extension, part of the pack) were up-to-date, as this ultimately resolved the issue where the Testing view wasn't recognizing the Java tests.

