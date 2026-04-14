# Haxor World AIO Changelog

## v3.0.1
> Release Date: April 15, 2026

Thank you for using Haxor World AIO. This update focuses on expanding the availability of core security tools to all users and introduces a new checker utility.

### New Features
- Added a new **WHM Checker** tool to quickly and efficiently validate WHM credentials at scale.

### UI Improvements
- Unified the **Execution Logs** panel design across scanner pages for a more consistent monitoring experience.
- Improved the **Statistics** tab so live metrics such as **Execution Logs**, **Total Processed**, and **Session Time** are only active when a task is actually running.
- Refined empty states and task status presentation to make inactive sessions clearer and easier to read.

### Bug Fixes
- [FIXED] Resolved a task state race condition where completed tasks could remain stuck behind a **Stop** action and could not be deleted immediately.
- [FIXED] Improved stop-task handling for cases where a task had already finished before the stop request was processed.
- [FIXED] Corrected live statistics behavior that previously continued showing execution data even when no task was running.

### Optimizations
- Improved task log rendering behavior for better readability and more stable real-time updates.
- Refined active task selection logic so the statistics panel always prioritizes the correct running session.
- Unlocked the **Vulnerability Scanner** feature globally. It is now accessible for **Free** and **Pro** users (previously restricted to the Premium tier).

### Important Notes
> Live statistics are now session-aware and will remain inactive until at least one task is actively running.

---

## v3.0.0
> Release Date: April 05, 2026

Thank you for using Haxor World AIO. In this update, we focused on adding new tools and improving stability so that workflows run optimally. Here are the full details:

### New Features
- Added a comprehensive Vulnerability Scanner for mass-detecting and reporting CVEs, equipped with targeted and aggressive payload delivery modes.
- Added a new Update Logs popup feature synchronized directly with GitHub.
- Integrated a new Shodan API scanning logic with aggressive multi-threading (up to x200 limits).
- Revamped the UI system on the CMS Scanner and Vulnerability Scanner pages with the standardized Task Queue component.

### Bug Fixes
- [FIXED] Fixed queue state updates that were delayed when a task was recently deleted or cleared.
- [FIXED] Implemented a better progress bar synchronization when iterating through a massive amount of target domains.

### Optimizations
- Theme mode can now be quickly toggled through the Action Search Panel (Press: Ctrl + F).
- Target file readings are now 30% more memory-efficient when uploading large payload blocks.

### Important Notes
> Please ensure that your target lists do not contain trailing white spaces or empty lines (\n) to prevent execution failures during bulk scanning.
