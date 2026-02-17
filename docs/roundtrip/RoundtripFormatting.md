---
tags:
    - roundtrip
---

# Roundtrip Spreadsheets, Formats, and Tools

!!! Roles "User roles" 
    TBD

The Roundtrip tools make use of CSV spreadsheets for import and export. Here are some things to keep in mind when working with CSV spreadsheets, in contrast to other formats, such as XLS.

## File formats and character encoding:

- All spreadsheets must use CSV (comma-separated values) spreadsheets.
    - CSV is a non-proprietary spreadsheet format that can be opened by all spreadsheet tools. 
    - While it does not support things like cell highlighting and text styling, it is very reliable, portable, and accessible.
- All spreadsheets must use Unicode UTF-8 character encoding.
    - UTF-8 is the most commonly used character encoding system used online.
    - Most non-English keyboards are developed to use UTF-8 encoding to ensure that their characters are accurately and reliably displayed across operating systems and web browsers.
- Certain exports will generate ZIP archives for download.
    - ZIP archives compress files and folder directories to reduce their size and facilitate transfer of larger files.
    - All operating systems have built-in tools to create and open ZIP archives – they are often found under “compress” actions.
        - ![Compress or uncompress files and folders on Mac](https://support.apple.com/en-ca/guide/mac-help/mchlp2528/mac)
        - ![Zip and unzip files (Windows)](https://support.microsoft.com/en-us/windows/zip-and-unzip-files-8d28fa72-f2f9-712f-67df-f80cf89fd4e5)
    - Third-party ZIP tools can be used, but are  not required.

## Spreadsheet tools:

In general, any spreadsheet tool that supports the above file format and character encodings requirements should work fine. We have some recommendations based on our testing and experiences:

**Google Sheets**
- Good for online/collaborative work.
- Works on all operating systems and browsers.
- Supports CSV export.
- Defaults to UTF-8 encoding.
- Free, but requires a Google account to use, and in certain cases using a service like this may not be appropriate, especially if sensitive information is being entered.

**LibreOffice and OpenOffice**
- Good for offline/local work.
- Work on all operating systems.
- Supports saving as CSV.
- Supports UTF-8 encoding.
- Free to download.

**Microsoft Excel**
- Microsoft Excel is NOT recommended.
- Defaults to XLS, not as easy to use CSV.
- Defaults to a proprietary encoding, and does not reliably support UTF-8 encoding.
- Note that on Windows, sometimes it will work well enough, but on macOS, these issues cannot be reliably avoided.
- At this time, we have not thoroughly tested any of Microsoft’s online services (eg: Office 365) and are not sure how they address these issues.

**Numbers**
- Not yet tested.