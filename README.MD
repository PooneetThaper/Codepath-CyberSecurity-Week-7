# Project 7 - WordPress Pentesting

Time spent: **5** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Cross-Site Scripting (XSS) Vulnerability
  - [x] Summary: Cross-Site Scripting (XSS) Vulnerability
    - Vulnerability types: Cross-Site Scripting (XSS) Vulnerability with embedding
    - Tested in version: 4.2
    - Fixed in version: 4.2.3
  - [x] GIF Walkthrough:
  - [x] Steps to recreate:
    - Create new post
    - Paste '''[embed src='https://youtube.com/embed/123\x3csvg onload=alert(123)\x3e'][/embed]'''
    - The onload is executed and an alert comes up
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
2. (Required) User Enumeration
  - [x] Summary: User Enumeration to get valid user
    - Vulnerability types: User Enumeration
    - Tested in version: 4.2
    - Fixed in version:
  - [x] GIF Walkthrough:
  - [x] Steps to recreate:
    - Guess usernames with random password until website tells you that the password is wrong
    - Guess passwords for that user until password is successful

3. (Required) Cross-Site Scripting (XSS) Vulnerability
  - [x] Summary: Cross-Site Scripting via Media File Metadata
    - Vulnerability types: Cross-Site Scripting (XSS) Vulnerability
    - Tested in version: 4.2
    - Fixed in version:
  - [x] GIF Walkthrough:
  - [x] Steps to recreate:
    - Upload a new image as Media
    - Edit the data of the media with a script
    - View the attachment page

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

## License

    Copyright [2018] [Pooneet Thaper]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
