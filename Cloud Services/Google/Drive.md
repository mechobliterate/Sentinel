# Google Drive Privacy Settings

<div align="center">
  <img src="../../images/cloud-services/google/drive-logo.svg" alt="Google Drive Logo" width="120" height="120">
</div>

## Overview

Google Drive is Google's cloud storage service integrated with Google Docs, Sheets, Slides, and other productivity apps. Google scans all files for features, spam detection, and (unless disabled) personalization across Google services.

**Key Privacy Concerns:**
- Files scanned by Google (docs, images, videos)
- Content used for ad personalization if smart features enabled
- Sharing defaults may expose files unintentionally
- No end-to-end encryption (Google can access files)
- Integration with Gmail means email attachments auto-saved
- Third-party apps may have access
- File activity tracked and used for suggestions

---

## Quick Settings Checklist

### Essential Settings
- [ ] Disable "Smart features" in Drive and Docs
- [ ] Review sharing permissions on all files
- [ ] Check "Shared with me" for unexpected access
- [ ] Disable "Show suggestions" and "Priority"
- [ ] Review third-party app connections
- [ ] Enable 2-Factor Authentication on Google Account
- [ ] Set up offline access carefully (caches files locally)

### Best Practices
- [ ] Use specific sharing (emails) instead of "Anyone with link"
- [ ] Set expiration dates on shared links
- [ ] Regularly audit who has access to files
- [ ] Don't store highly sensitive documents (use encrypted alternatives)
- [ ] Download backups of important files periodically

---

## Critical Privacy Settings

### 1. Disable Smart Features (MOST IMPORTANT)

**Path:** Drive Settings > General

❌ **Uncheck:** "Use Drive for desktop offline access"  
❌ **Uncheck:** "Suggestions"  
❌ **Uncheck:** "Activity dashboard"

**Path:** Google Docs/Sheets Settings

❌ **Uncheck:** "Show suggested files, links, and people"  
❌ **Uncheck:** "Smart Compose"

### 2. Review File Sharing

**Check all files:**
1. Go to drive.google.com
2. Search: `is:shared`
3. Review each shared file/folder
4. Remove unnecessary sharing

**Sharing best practices:**
- Use "Specific people" instead of "Anyone with link"
- Use "Viewer" or "Commenter" instead of "Editor" when possible
- Set expiration dates on temporary shares
- Regularly audit shared files

### 3. Manage Third-Party App Access

**Path:** myaccount.google.com > Security > Third-party apps with account access

**Remove apps that:**
- You don't recognize
- You no longer use
- Have Drive access but don't need it

**Apps to watch:**
- PDF editors
- Photo editors
- Productivity tools
- Backup services

### 4. Activity and Versions

**File activity:**
- Drive tracks all file activity
- Shows who viewed/edited and when
- Can't be disabled

**Version history:**
- Drive keeps file versions
- Can restore older versions
- Also means deleted content may remain

**To minimize:**
- Delete files you no longer need
- Empty trash regularly (auto-empties after 30 days)

---

## Google Account Privacy (Affects Drive)

See **[Google Account Settings](account-settings.md)** guide for full details.

**Critical settings:**
- Turn off "Web & App Activity" or auto-delete
- Disable ad personalization
- Pause "Location History"

---

## What Data Google Collects from Drive

### Always Collected:
- File metadata (names, sizes, types, timestamps)
- Who you share with and what permissions
- Your IP address and device info
- File access patterns and frequency

### Collected Unless Disabled:
- File content scanning for features/personalization
- Usage for ad targeting (if smart features enabled)
- Integration with other Google services data

### Google's Access:
- Google can access all files (no E2E encryption)
- Used for spam/malware detection
- Can be accessed for legal compliance
- Employees may access for abuse investigations

---

## Alternative Cloud Storage

For better privacy:

**End-to-End Encrypted:**
- **ProtonDrive** - E2E encrypted, privacy-focused
- **Tresorit** - Swiss privacy, zero-knowledge
- **Sync.com** - Canadian, true privacy

**Encrypted Wrappers (Use with any cloud):**
- **Cryptomator** - Encrypt files before uploading
- **VeraCrypt** - Create encrypted containers
- **Boxcryptor** - Encryption layer for cloud storage

**Privacy-Respecting (Not encrypted):**
- **Nextcloud** - Self-hosted, complete control
- **Filen** - German privacy laws, affordable

---

## Summary: Essential Actions

1. **Disable smart features** in Drive and Docs
2. **Review all shared files** - Audit regularly
3. **Use specific people sharing** - Avoid "anyone with link"
4. **Remove third-party apps** - Check Google Account security
5. **Consider encrypted alternatives** - For sensitive files

**For truly sensitive files:** Don't use Google Drive. Use ProtonDrive, Tresorit, or Cryptomator.

---

**Last Updated:** February 15, 2026  
*Part of the [PrivacyGuard](https://github.com/mechobliterate/privacyguard) project*
