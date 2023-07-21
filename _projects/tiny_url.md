---
layout: project
title: Tiny URL
subtitle: Java Redis MongoDB
---

In version 2 of the project, significant improvements have been made by introducing the Snowflake algorithm to generate unique 64-bit IDs for short URLs. To enhance readability and compatibility, the project has transitioned from base-64 to base-58 encoding, excluding certain characters that may cause confusion. This results in a more efficient and user-friendly URL shortening system.

Pros of version 2 include its simplicity, lightweight design, and integration with Redis for efficient storage and retrieval. The randomized short URLs generated by the Snowflake algorithm ensure uniqueness and reduce collision risks. The implementation also allows flexibility with dependency injection, accommodating various Redis configurations or alternative storage solutions.

However, version 2 has some areas for improvement. Customization options for short URL length or format are lacking, limiting its adaptability to diverse requirements. Error handling and rate limiting mechanisms need to be enhanced for better robustness. Additionally, scaling concerns should be addressed, considering strategies for handling high volumes of concurrent requests, and introducing database persistence for data durability.

Version 3 aims to address these improvements and introduces several new features. Users will have the ability to customize URLs and benefit from URL validation. MongoDB will serve as the primary database, with Redis acting as a cache to enhance performance. The UI/UX will undergo improvements to enhance user experience, and QR codes will be generated for short URLs. Redis will also be utilized as a rate limiter, ensuring fair usage and security. User accounts and authentication will be implemented, allowing personalized URL management and tracking statistics.

Through version 3, the project strives to deliver a more feature-rich and reliable URL shortening service, catering to diverse user needs while prioritizing scalability, security, and user experience.

<a href="https://github.com/oliverXS/url-shortener" target="_blank">More details about this project.</a>

##### Some diagrams for this project

**Version1.** <br/>
{%
	include image_with_caption.html
	url="/assets/projects/tiny_url/one.png"
	width="100%"
%}
**Version2.** <br/>
{%
	include image_with_caption.html
	url="/assets/projects/tiny_url/two.png"
	width="100%"
%}
**Version3.** <br/>
{%
	include image_with_caption.html
	url="/assets/projects/tiny_url/three.png"
	width="100%"
%}