# Uninitialized Class Member Variables in C#

This repository demonstrates a common error in C#: failing to initialize class member variables.  Uninitialized variables can lead to unpredictable program behavior, especially when dealing with concurrency. The solution shows the correct approach, demonstrating how to initialize variables within the constructor to prevent such issues.

## Bug

The `Bug.cs` file contains a class with a member variable that is not explicitly initialized.  Depending on the context, this could result in the variable holding an unexpected default value, leading to bugs. 

## Solution

The `BugSolution.cs` file provides a corrected version. The class member variable is initialized within the constructor, ensuring it has a defined value when the object is created. This best practice makes code more robust and predictable.