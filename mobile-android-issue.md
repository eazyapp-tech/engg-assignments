# RentOk Android Issue Assignment

## Issue Summary

We have identified a critical issue related to changing the app icon and name dynamically in the RentOk Manager Android application. This issue causes the package name to change to the activity alias, leading to failures in activity calls.

### Error Message

Changing enabled activity-alias from default to net.eazypg.eazypgtenant.xyz
android.content.ActivityNotFoundException: Unable to find explicit activity class {net.eazypg.eazypgtenant/com.cashfree.pg.core.api.ui.CFCoreUPIPaymentActivity}; have you declared this activity in your AndroidManifest.xml?

### Steps to Reproduce

1. Change the app icon and name based on the logged-in user.
2. Observe the change in the package name to the activity alias.
3. Attempt to perform an action using the Cashfree SDK, resulting in the mentioned error.

## Problem Analysis

The issue arises from dynamic changes in the app icon and name, leading to a modification in the package name to the activity alias. This alteration conflicts with the expectations of the Cashfree SDK, resulting in the inability to find the required activity (`CFCoreUPIPaymentActivity`), consequently causing the `ActivityNotFoundException`.

### Code Reference

You can refer to the specific code causing the issue in the following file:
[IconChanger.java](https://github.com/eazyapp-tech/flutter_dynamic_icon/blob/98c993638fd8bb1a111a0adaad0dfc7d6767de0e/android/src/main/java/io/github/tastelessjolt/flutterdynamicicon/IconChanger.java#L63)

If needed, you can also use the example app provided in this repository for reference: [flutter_dynamic_icon](https://github.com/eazyapp-tech/flutter_dynamic_icon)

## Additional Notes

This issue primarily stems from the dynamic alteration of the package name conflicting with the Cashfree SDK's expectations. By carefully managing the package name change process and ensuring proper activity declaration, this issue can likely be mitigated effectively.

## Submission Guidelines

- Create a new repository on GitHub or GitLab to host your project.
- Complete the technical task following the requirements outlined above.
- Provide clear instructions on how to build and run the application.
- Share the repository link with us for evaluation.

Feel free to use any third-party libraries or frameworks you find appropriate to accomplish the task. Focus on demonstrating your ability to develop a robust and efficient Android application that effectively handles data-heavy operations and delivers an exceptional user experience. Good luck!

---
