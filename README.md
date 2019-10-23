# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) WordPress 4.2 - Unauthenticated Stored Cross-Site Scripting (XSS)
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [x] GIF Walkthrough: 
	<img src='xss.gif'>

  - [x] Steps to recreate: <br>
	-Add a normal comment and wait for it to be approved. <br>
	-Once approved paste the payload in the reply to that comment. <br>
	-Wait for an admin to view that comment for the xss to do it's job. <br>
  - [x] Affected source code:
    - [Link](https://core.trac.wordpress.org/browser/tags/4.2/src/wp-comments-post.php)

2. (Required) WordPress 4.7.0-4.7.1 - Unauthenticated Page/Post Content Modification via REST API
  - [x] Summary: 
    - Vulnerability types: Privilege Escalation
    - Tested in version: 4.7
    - Fixed in version: 4.7.2
  - [x] GIF Walkthrough: 
	<img src='pe.gif'>
  - [x] Steps to recreate:
	-Locate a website running wordpress 4.7
	-get and exploit from exploit db and run it against the website to see the posts
	-make a file with the desired content in it
	-run the exploit as shown in the gif to replace the content of the post with your content 
  - [x] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/4.7/src/wp-includes/rest-api/endpoints/class-wp-rest-posts-controller.php)
    - [Exploit Link] (https://www.exploit-db.com/exploits/41223)

1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
