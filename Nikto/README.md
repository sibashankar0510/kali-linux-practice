# Nikto Web Server Scanner

A practical learning guide to Nikto, a web server security scanner, using Kali Linux.

## 1. Introduction

Nikto is an open-source web server scanner written in Perl. It helps security learners and administrators identify potential issues in web servers.

It checks for known problems, outdated server software, potentially dangerous files, and common server misconfigurations.

## 2. Objectives

- Understand the basics of Nikto.
- Learn useful Linux and Nikto commands.
- Understand web server scanning.
- Learn how to interpret scan results.
- Practice responsible and authorized security testing.

## 3. Lab Environment

- Operating System: Kali Linux
- Tool: Nikto
- Category: Web Security
- Purpose: Educational and defensive security testing
- Target: Local system or authorized practice lab

## 4. Installation and Verification

### Check Nikto Version

```bash
nikto -Version
```

Displays the installed Nikto version.

### Display Help

```bash
nikto -Help
```

Displays the available command-line options.

### View the Manual

```bash
man nikto
```

Opens the manual page if it is available.

Press `q` to exit the manual.

## 5. Useful Linux Commands

### Locate the Nikto Executable

```bash
which nikto
```

Displays the executable path if Nikto is available in the system's PATH.

### Check Package Information

```bash
apt show nikto
```

Displays information about the Nikto package.

### Check Installation Status

```bash
dpkg -s nikto
```

Shows the package installation status and other details.

### List Installed Package Files

```bash
dpkg -L nikto
```

Lists files associated with the installed Nikto package.

### Check for a Running Nikto Process

```bash
ps aux | grep '[n]ikto'
```

Searches for a running process whose command matches Nikto.

## 6. How Nikto Works

Nikto performs checks against a web server and compares its responses with known checks in its testing database.

The general process is:

1. Connect to the specified web server.
2. Send requests associated with configured checks.
3. Examine the server responses.
4. Report potential security issues.
5. Allow an administrator or security tester to review the findings.

A reported finding does not necessarily mean that a confirmed vulnerability exists.

## 7. Understanding Scan Results

Depending on the scan, Nikto may report:

- HTTP response codes.
- Web server software information.
- Missing or unusual HTTP security headers.
- Potentially exposed files.
- Outdated software indicators.
- Possible security misconfigurations.

Results should be reviewed carefully. Some findings may be false positives or require further verification.

## 8. Important Concepts

### Web Server

A web server receives HTTP or HTTPS requests and sends responses to clients.

### HTTP Headers

HTTP headers carry information about requests and responses. Some response headers can help improve browser-side security.

### Security Misconfiguration

A security misconfiguration occurs when a system is configured in a way that may increase security risks.

### False Positive

A false positive is a reported issue that turns out not to be a real vulnerability.

## 9. Practical Screenshots

Screenshots from my Kali Linux practice can be added below.

### Version Check

Save the screenshot as `nikto-version.png` and upload it to this directory.

![Nikto Version Check](nikto-version.png)

### Help Output

Save the screenshot as `nikto-help.png` and upload it to this directory.

![Nikto Help Output](nikto-help.png)

**Note:** These image links will display correctly after the corresponding screenshots have been uploaded with the exact filenames.

## 10. What I Learned

- Introduction to the Nikto web server scanner.
- Checking tool versions and available options.
- Exploring Linux package information.
- Understanding web server scanning.
- Learning about HTTP responses and security headers.
- Interpreting potential security findings.
- Understanding the limitations of automated scanners.
- Practicing responsible security testing.

## 11. Safety and Authorization

All security testing must be performed only on systems that I own or have explicit permission to test.

I use local environments and authorized training labs for learning.

Sensitive information, credentials, session tokens, and private scan data should not be published in a public repository.

## 12. References

- [Nikto on Kali Linux](https://www.kali.org/tools/nikto/)
- [Official Nikto GitHub Repository](https://github.com/sullo/nikto)

---

**Disclaimer:** This repository documents educational learning and authorized defensive security practice.
