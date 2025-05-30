# Project SECURITY: Advanced Web Application Firewall (WAF)

**Project SECURITY** is a powerful web application firewall (WAF) designed to protect PHP-based websites, including custom scripts, popular shopping carts, and CMS applications. It utilizes intelligent algorithms to detect known hacker attacks and identify new, unknown threats using advanced code and pattern recognition. Additionally, it offers automated responses to mitigate these attacks.This is a powerful website security application that will protect your website from hackers, attacks, and other threats. It will protect your website from SQLi attacks (SQL injections), XSS vulnerabilities, proxy visitors, VPN visitors, TOR visitors, spam, and many other types of threats.

## Key Features

- **Automated Threat Detection:** Detects both known and unknown threats by analyzing code and traffic patterns.
- **Powerful Admin Panel:** Comprehensive control over your website's security with real-time logs, customizable settings, and instant access to security tools.
- **Block Unwanted Traffic:** Block malicious visitors based on IP address, countries, IP ranges, ISPs, browsers, operating systems, and sources.
- **Minimal System Resources:** Optimized for speed and minimal resource consumption while providing maximum protection.
- **Cross-Platform Protection:** Suitable for all PHP-based websites, including custom scripts, shopping carts, and CMS applications (e.g., WordPress, Joomla, etc.).
- **Customizable Alerts:** Receive instant notifications when potential threats are detected or actions are taken.

## Installation

### Requirements:
- PHP 7.0 or higher
- A web server (Apache, Nginx, etc.)
- MySQL or SQLite (for storing logs, settings, etc.)

### Steps to Install:

1. **Download or Clone the Repository:**

   ```bash
   git clone https://github.com/mscbuilde/Website-Security.git
   ```

2. **Upload to Your Server:**
  
Upload the files to your web server directory where you want to install the firewall.

4. **Configure the Firewall:**
 
Navigate to the config/ directory and update the config.php file to suit your server environment.

5. **Setup Database (Optional but Recommended):**
 
If you wish to store logs, create a database and import the provided SQL schema located in database/schema.sql. Update the config.php file to reflect the database connection settings.

6. **Activate the Firewall:**
   
To enable the firewall on your website, include the firewall script at the top of your website's main index.php or equivalent entry point:
```bash
require_once('path/to/project-security/firewall.php');
```

6. **Access the Admin Panel:**
 
Navigate to http://yourdomain.com/admin and log in using the default admin credentials (which you should change immediately after installation). The default credentials are:

- Username: admin

- Password: password123

## Admin Panel Overview

The admin panel is designed to be user-friendly and feature-rich. Here's a quick rundown of the features available:

**Dashboard:**

View a real-time overview of attacks, blocked traffic, and security status.

**Logs:**

Access detailed logs of all detected and blocked attacks. Logs can be filtered by attack type, date, source IP, and more.

**Blocking:**

- IP Blocking: Block individual IP addresses or entire IP ranges.

- Country Blocking: Prevent traffic from specific countries.

- ISP Blocking: Block traffic from specific Internet Service Providers.

- Browser/OS Blocking: Block visitors using certain browsers or operating systems.

**Settings:**

Customize various settings such as:

- Attack Sensitivity: Control how aggressive the detection algorithm is.

- Alert Settings: Configure notifications for new threats and security updates.

- Action Settings: Set automatic responses for different attack types (e.g., block, challenge CAPTCHA, etc.).

**Security Features**

- Code & Pattern Recognition: Utilizes advanced algorithms to analyze and recognize attack patterns in real-time.

- Automated Response System: Once a threat is detected, the system can automatically block it, log the event, and notify the administrator.

- Brute Force Protection: Prevents multiple failed login attempts and protects against password-guessing attacks.

- SQL Injection & XSS Protection: Detects and blocks common web vulnerabilities like SQL injections and cross-site scripting (XSS).

- Session Management: Detects and prevents session hijacking and fixation attacks.

  **Contribution**
  
- We welcome contributions! If you would like to contribute to Project SECURITY, feel free to fork the repository and submit a pull request.

- Before submitting changes, please ensure that:

- You write clear commit messages.

- You test your changes thoroughly.

- You follow the coding standards used in the repository.

**License**

Project SECURITY is released under the MIT License.
 

