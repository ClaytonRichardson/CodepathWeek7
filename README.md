# Project 7 - WordPress Pentesting

Time spent: 10 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) XSS Vulnerability
  - [ ] Summary: This exploit is all about affecting the user when they view the post made by the malicious user.
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.6.1
  - [ ] GIF Walkthrough: 
![Alt Text](https://github.com/ClaytonRichardson/CodepathWeek7/blob/master/firstvuln.gif)
  - [ ] Steps to recreate: 
  1. Create a new post
  2. add malicious tags in title of new post
  3. view post to be alerted of XSS
  - [ ] Affected source code:
   
2. (Required) Stored XSS Vulnerability
  - [ ] Summary: This exploit is to store user cookie data when viewing the comment made my a malicious user.
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.3.1
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  1. Open a post made by any user
  2. proced to leave a comment consisiting of <svg onload=prompt(document.cookie)>
  3. Any user to view this comment will have their cookie data stored
  - [ ] Affected source code:
    
3. (Required) Authenticated Stored Cross-Site Scripting
  - [ ] Summary: A clickable link that leaves unknowing victims open to an XSS attack.
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  1. Make a post with the description being <ahref="[caption code=">]</a><a title="onmouseover=alert('XSS') ">link</a>
  - [ ] Affected source code:
    


## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [2018] [ClaytonRichardson]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
