---
layout: page
title: "Reading Pencil: Privacy Policy"
description: "Reading Pencil's privacy policy: nothing you read leaves your computer."
permalink: /reading-pencil/privacy/
---

# Reading Pencil: Privacy Policy

_Last updated: 10 October 2026_

Reading Pencil is a browser extension that draws a small pencil under the line
you are reading. This policy says exactly what it does with your data. The
short version: **nothing you read leaves your computer.**

## What Reading Pencil collects

Nothing is collected, sent or shared. Reading Pencil has no analytics, no
crash reporting, no advertising, no accounts and no servers. It makes one
kind of network request only: when you start the pencil on a PDF, or open one
from "Where you left off", it downloads that PDF from its own address, to show
it in a page of its own (see "PDFs" below). That request goes only to the
website the PDF comes from.

## What it stores on your device

Reading Pencil keeps a small amount of information in your browser's own
extension storage (`chrome.storage.local`), on your computer only:

- **Your settings:** your reading pace, Pencil or Line, which hand, colour,
  highlight strength, and whether to keep to the article.
- **Where you left off:** for each long page you have started reading with
  the pencil (at most 50; the oldest are removed first):
  - the page's address (for a PDF, the PDF's address; and, if the site
    changed its address while you read, up to three other addresses of the
    same article), with tracking
    parameters (such as `utm_source`) and parameters that carry secrets
    (such as tokens, passwords, signatures, session IDs or email
    addresses) removed; very long addresses are not kept at all;
  - the first 80 characters of the paragraph you were on, used only to find
    that paragraph again when you come back;
  - how far into that paragraph you were, and when.
- **Whether you have seen the short how-to hint** (a count, so it stops after
  a few times).

Nothing is stored for pages you read in an Incognito window.

This information is never transmitted anywhere, and websites cannot read it
from the extension's storage. It is used only to draw the pencil and to put
it back where you left off. While the pencil is drawn on a page, that page's
own scripts can see it there (its position and colour, and the "continue"
card when one is shown), as they can see anything else on their page.

## PDFs

Chrome's own PDF viewer lets no extension in, so when you start the pencil on
a PDF, Reading Pencil opens it in a page of its own, inside the extension. To
do that, it downloads the PDF from its own address (the one your browser
opened, or the one kept in "Where you left off"), with your browser's cookies
for that website, as your browser itself would (so a PDF you had to sign in
for still opens). The PDF is shown and read on your computer. It is not
stored, and it is not sent anywhere else. A PDF you choose from your computer
is read from that file and never leaves it. PDFs are not opened from Incognito
windows.

## How to remove it

- Open the toolbar popup → **Where you left off** to forget one page or all of
  them.
- Uninstalling Reading Pencil removes everything it stored.

## Permissions, and why

- **Read and change data on websites** (content script and host access for
  `http` and `https` pages): when you start the pencil on a page, to find the
  text of the article and draw the pencil over it; and when you start it on a
  PDF, to download that PDF from its own address and show it in Reading
  Pencil's page. Page content is read in your browser to measure lines; it is
  never stored (apart from the 80-character excerpt above) or sent anywhere.
- **storage:** to keep your settings and places on your device.
- **activeTab** and **scripting:** to place the pencil on a tab where it
  isn't running yet, when you ask for it there; and once, when the extension
  is installed, updated or switched back on, to give the web pages already
  open its script, so that "Start reading here" works in them without a
  reload. Until you start the pencil, that script only notes where you
  right-click, and, when you open the toolbar popup, counts the lines it
  could read there. Nothing leaves your browser.
- **contextMenus:** the "Start reading here" item in the right-click menu.

## Children

Reading Pencil collects no data from anyone, including children.

## Changes

If this policy ever changes, the new version will be published here with a
new date. Reading Pencil will never begin collecting or transmitting data
without a new version of the extension and of this policy.

## Contact

Questions: message [@threatner_ on X](https://x.com/threatner_).
