## Toward better API security 1pm - st Laurent 1 / Tomasz Kowalczyk

“All behaviour of your system will be used by somebody”

**Introduction:**

The importance of security in system design cannot be overstated, as all behaviors of a system are susceptible to exploitation. Despite contractual agreements, security vulnerabilities remain a critical concern, emphasizing the need for robust security measures.

**Basics of Security:**

- Understanding the basics of authentication, authorization, and permissions is paramount.
- Familiarity with common vulnerabilities, as listed by OWASP, is essential for proactive risk mitigation.

**API Design Best Practices:**

- **Resource Probing:**
  - Avoid resource probing by refraining from providing specific error messages that could reveal sensitive information.
  - Limit the amount of information returned by APIs to prevent data exposure (e.g., Twitter's approach of returning generic error messages).

- **Resource Enumeration:**
  - Mitigate resource enumeration vulnerabilities by using UUIDs or non-sequential identifiers instead of predictable numeric IDs.
  - Example vulnerabilities, such as those experienced by Cisco Web and Zoom, highlight the importance of securing endpoints to prevent data leakage.

- **Timing Attacks:**
  - Guard against timing attacks by ensuring consistent response times, regardless of the validity of user input.
  - Algorithms should execute operations until completion to avoid revealing information about data validity based on response times.

- **Side Channels:**
  - Prevent side-channel attacks by minimizing the exposure of sensitive data and employing diverse data representation methods.
  - Use tokens for sensitive information and consider implementing two-factor authentication (2FA) for added security.

- **Unbounded Collection:**
  - Address unbounded collection vulnerabilities by limiting the amount of data exposed through endpoints.
  - Implement strict data creation controls to prevent unauthorized data creation and consider segmenting data into separate endpoints for enhanced security.

- **Monitoring Communication:**
  - Monitor all communication channels to detect and respond to potential security threats promptly.
  - Detailed monitoring helps identify suspicious activities and allows for timely intervention to mitigate risks effectively.

**Conclusion:**

Security considerations are paramount in API design to protect against various vulnerabilities and safeguard sensitive data. By adhering to best practices and remaining vigilant in monitoring and addressing potential security threats, developers can create robust and resilient systems that prioritize the security and privacy of users' data.

## Slides:

- # [Official slides](https://github.com/confooca/2024/tree/main)