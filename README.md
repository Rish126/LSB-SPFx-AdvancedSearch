# SearchDoc 1.3.6

## Summary

SPFx (v1.16.1) web part that queries multiple document libraries in the current SharePoint web based on specific metadata fields. Dynamically builds a CAML query based on filter selections as seen in thefollowing screenshot.

![screenshot](./SearcDoc%201.2%20Sreenshot.png)

## Used SharePoint Framework Version

![version](https://img.shields.io/badge/version-1.16.1-green.svg)

## Applies to

- [SharePoint Framework](https://aka.ms/spfx)
- [Microsoft 365 tenant](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)

> Get your own free development tenant by subscribing to [Microsoft 365 developer program](http://aka.ms/o365devprogram)

## Prerequisites

> Any special pre-requisites?

## Solution

| Solution      | Author(s)                                               |
| ------------- | ------------------------------------------------------- |
| SearchDoc-1.3 | Patrick Gaul, NTT Data Services (Sierra Systems Group)  |

## Version history

| Version | Date             | Comments                  |
| ------- | ---------------- | ------------------------- |
| 1.3.6   | June 15, 2023    | Field Changes             |
| 1.3.0   | March 16, 2023   | Updgraded SPFx to 1.16.1  |
| 1.2.0   | March 10, 2023   | Deployed to Production    |

## Disclaimer

**THIS CODE IS PROVIDED _AS IS_ WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

---

## Minimal Path to Awesome

- Clone this repository
- Ensure that you are at the solution folder
- in the command-line run:
  - **npm install**
  - **gulp serve**

> Include any additional steps as needed.

## Features

Created for the Legal Services Branch of the British Columbia Government. This web part ynamically builds CAML queries for each of an array of SharePoint Document Libraries that use a custom content type (LSB KB Document) that can be found at https://bcgov.sharepoint.com/sites/AG-LSBKB/_layouts/15/SiteAdmin.aspx#/contentTypes. It determines the libraries based on the entries in the "Libraries" list found at https://bcgov.sharepoint.com/sites/AG-LSBKB/Lists/Libraries.

This web part has the following features:

- Allows the selection of two "Areas of Law" and related "Topics of Law", with further metadata selections which further restrict search results.
- The available selections of "Topic of Law" are dynamically adjusted to those available under "Area of Law".
- The "Keyword Search" box can include a series of keywords separated by spaces (any of which will be included in the results), or a single phrase enclosed in quotes. Both the document name and description will be searched for occurrences.
- The interface adapts itself to the site's current colout theme.

## References

- [Getting started with SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)
- [Microsoft 365 Patterns and Practices](https://aka.ms/m365pnp) - Guidance, tooling, samples and open-source controls for your Microsoft 365 development
