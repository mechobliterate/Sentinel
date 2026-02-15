# Google Photos Privacy Settings

<div align="center">
  <img src="../../images/cloud-services/google/photos-logo.svg" alt="Google Photos Logo" width="120" height="120">
</div>

## Overview

Google Photos automatically backs up photos and videos, organizes them with AI, and creates albums/animations. Google's AI scans all photos for facial recognition, object detection, and content analysis.

**Major Privacy Concerns:**
- All photos scanned by Google's AI
- Facial recognition creates searchable database of people
- Location data extracted from photos (EXIF)
- Shared albums may expose private moments
- Photos used to improve Google's AI
- No end-to-end encryption

---

## Quick Settings Checklist

- [ ] Turn off "Backup & sync" (consider manual backups instead)
- [ ] Disable facial recognition features
- [ ] Remove location data from photos before uploading
- [ ] Review shared albums and permissions
- [ ] Disable "Smart features and personalization"
- [ ] Check "Archive" for private photos
- [ ] Review partner sharing settings

---

## Critical Settings

### 1. Backup and Sync

**Path:** Google Photos app > Settings > Backup

**Consider:** ❌ Turn OFF automatic backup

**Why:**
- Every photo/video uploaded is scanned by Google
- Location, faces, objects all analyzed
- Used for AI training and features

**Alternative:**
- Manual backups to external drive
- Use privacy-focused photo backup (Cryptomator + any cloud)
- Self-hosted solutions (Nextcloud, PhotoPrism)

### 2. Face Grouping

**Path:** Settings > Group similar faces

❌ **Turn OFF**

**What it does:**
- Creates facial recognition database
- Identifies people across photos
- Highly invasive privacy concern

### 3. Location Data

**Two approaches:**

**Option A:** Remove before uploading
- Use ExifTool or similar to strip location
- Prevents Google from ever seeing location

**Option B:** Disable location access
- Phone settings > Google Photos > Location > Never
- But already-uploaded photos retain location

### 4. Shared Albums and Partner Sharing

**Review all shared albums:**
1. Photos app > Shared
2. Review each album
3. Remove unnecessary sharing

**Partner sharing:**
- Path: Settings > Partner sharing
- Gives another person access to all/selected photos
- ❌ Disable unless absolutely necessary

---

## What Google Learns from Photos

- **Faces:** Who you spend time with
- **Locations:** Where you go, when
- **Activities:** What you do (hiking, parties, etc.)
- **Objects:** What you own, what you buy
- **Relationships:** Family, friends, relationships
- **Timeline:** Complete visual timeline of your life

This creates extremely detailed profile.

---

## Privacy-Focused Alternatives

**End-to-End Encrypted:**
- **Ente Photos** - E2E encrypted, open source
- **PhotoPrism** - Self-hosted, AI features without privacy invasion
- **Cryptomator + Any Cloud** - Encrypt before uploading

**Privacy-Respecting:**
- **Nextcloud Photos** - Self-hosted, complete control
- **iCloud Photos** (with Advanced Data Protection) - Apple can't access

---

## Summary: Essential Actions

1. **Turn off automatic backup** - Or use encrypted alternative
2. **Disable face grouping** - Prevents facial recognition database
3. **Strip location data** - Before uploading photos
4. **Review shared albums** - Remove unnecessary sharing
5. **Consider alternatives** - Ente Photos, PhotoPrism, or Cryptomator

**Bottom line:** Google Photos is convenient but extremely invasive. For private photos, use encrypted alternatives.

---

**Last Updated:** February 15, 2026  
*Part of the [PrivacyGuard](https://github.com/mechobliterate/privacyguard) project*
