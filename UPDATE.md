# Haxor World AIO Update v3.0.0
> Release Date: April 05, 2026

Thank you for using Haxor World AIO. In this update, we focused on adding new tools and improving stability so that workflows run optimally. Here are the full details:

## New Features
- Added a comprehensive Vulnerability Scanner for mass-detecting CVEs, equipped with targeted and aggressive payload delivery modes.
- Added a new Update Logs popup feature synchronized directly with GitHub.
- Integrated a new Shodan API scanning logic with aggressive multi-threading (up to x200 limits).
- Revamped the UI system on the CMS Scanner and Vulnerability Scanner pages with the standardized Task Queue component.

## Bug Fixes
- [FIXED] Fixed queue state updates that were delayed when a task was recently deleted or cleared.
- [FIXED] Implemented a better progress bar synchronization when iterating through a massive amount of target domains.

## Optimizations
- Theme mode can now be quickly toggled through the Action Search Panel (Press: Ctrl + F).
- Target file readings are now 30% more memory-efficient when uploading large payload blocks.

### Important Notes
> Please ensure that your target lists do not contain trailing white spaces or empty lines (\n) to prevent execution failures during bulk scanning.
