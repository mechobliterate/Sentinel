# Google Chrome Privacy Settings

<div align="center">
  <img src="../images/browsers/chrome/chrome-logo.svg" alt="Google Chrome Logo" width="120" height="120">
</div>

## Overview

Google Chrome is the world's most popular web browser, but it's also known for extensive data collection to power Google's advertising ecosystem. While Chrome offers convenience through Google account integration and sync features, these same features can compromise your privacy if not properly configured.

**Key Privacy Concerns:**
- Extensive telemetry and usage data collection
- Ad personalization through browsing history tracking
- Automatic Google account sync (history, passwords, settings)
- Third-party cookie tracking (being phased out)
- Search and navigation predictions sent to Google
- Safe Browsing data sharing
- Enhanced ad targeting through Topics API

**This guide will help you:**
- Minimize data sent to Google
- Disable personalized advertising
- Control site permissions and tracking
- Manage sync settings strategically
- Configure Safe Browsing appropriately
- Protect against fingerprinting

---

## Quick Settings Checklist

Use this checklist to quickly configure the most important privacy settings:

### Essential Privacy Settings
- [ ] Disable ad personalization (Ad Topics, Site-suggested ads, Ad Measurement)
- [ ] Turn off prediction services (preloading, autocomplete)
- [ ] Disable "Help improve Chrome" data collection
- [ ] Configure Safe Browsing (recommend Standard over Enhanced)
- [ ] Review and limit Google account sync
- [ ] Block third-party cookies
- [ ] Disable autofill for sensitive data
- [ ] Turn off site permissions (location, camera, microphone)
- [ ] Clear browsing data regularly
- [ ] Disable payment methods and address saving

### Advanced Privacy Settings
- [ ] Enable "Do Not Track" request
- [ ] Disable site engagement metrics
- [ ] Turn off Chrome sign-in prompts
- [ ] Manage permissions for installed extensions
- [ ] Review and revoke site permissions
- [ ] Configure search engine (consider privacy-focused alternatives)
- [ ] Disable network action predictions

---

## Detailed Configuration

### 1. Privacy and Security Settings

**Path:** `Settings` > `Privacy and security`

This is the main hub for all privacy-related settings in Chrome.

#### Ad Privacy

Chrome's new Ad Privacy features replace third-party cookies with new tracking mechanisms. You should disable all of these.

**Steps:**
1. Click `Settings` (three dots menu) > `Privacy and security`
2. Click `Ad privacy`
3. Disable all three features:

**Ad topics:**
- Toggle off: This prevents Chrome from creating interest profiles based on your browsing
- Chrome tracks which sites you visit and categorizes your interests
- Up to 3 topics are shared with sites at a time
- Topics auto-delete after 4 weeks, but new ones keep being created

**Site-suggested ads:**
- Toggle off: Prevents sites from storing ad preferences in Chrome
- Sites can suggest ads based on your activity on their platform
- Suggestions auto-delete after 30 days but regenerate on revisits

**Ad measurement:**
- Toggle off: Stops sites from measuring ad effectiveness through your browsing
- Prevents cross-site tracking for ad performance metrics
- This is essentially conversion tracking

⚠️ **Important:** Even with these disabled, you'll still see ads - they just won't be personalized based on Chrome's tracking of your browsing history.

#### Cookies and Other Site Data

**Path:** `Privacy and security` > `Cookies and other site data`

**Recommended Setting:** "Block third-party cookies"

**Steps:**
1. Select `Block third-party cookies`
2. Enable `Send a "Do Not Track" request with your browsing traffic`
3. Consider enabling `Preload pages for faster browsing and searching` ONLY if you trust Google with your browsing patterns

**Understanding Cookie Options:**

- **Allow all cookies:** Maximum privacy invasion - avoid
- **Block third-party cookies in Incognito:** Insufficient protection
- **Block third-party cookies (Recommended):** Good balance - stops most tracking
- **Block all cookies:** Breaks many websites - too restrictive for daily use

**Managing Cookie Exceptions:**

Some sites may break with blocked third-party cookies. Add exceptions only when necessary:
1. Click `See all site permissions and data`
2. Add specific sites to "Allowed to use cookies"
3. Review and remove exceptions regularly

💡 **Note:** Google is planning to fully deprecate third-party cookies, but their replacement (Privacy Sandbox/Topics API) may still enable tracking - which is why we disabled Ad Privacy features above.

#### Site Settings

**Path:** `Privacy and security` > `Site Settings`

Configure default permissions for all websites:

**Recommended Settings:**

| Permission | Setting | Reasoning |
|------------|---------|-----------|
| Location | Blocked | Precise location tracking |
| Camera | Ask (Default) | Allow when needed only |
| Microphone | Ask (Default) | Allow when needed only |
| Notifications | Blocked | Reduces spam and tracking |
| Background sync | Blocked | Prevents apps from syncing without use |
| Motion sensors | Blocked | Can fingerprint device |
| JavaScript | Allowed | Required for most sites |
| Images | Allowed | Required for browsing |
| Pop-ups and redirects | Blocked | Security and annoyance |
| Ads | Blocked on intrusive sites | Reduces malicious ads |
| File editing | Blocked | Security risk |
| Clipboard | Ask | Prevents silent data theft |
| Payment handlers | Blocked | Unless you actively use them |
| USB devices | Blocked | Prevents malicious hardware access |
| Serial ports | Blocked | Security risk |
| File System | Blocked | Prevents unauthorized file access |
| Local fonts | Blocked | Anti-fingerprinting |

**Steps to Change Permissions:**
1. Click on each permission type
2. Select the most restrictive option that doesn't break your workflow
3. Add site-specific exceptions as needed

**Reviewing Existing Permissions:**
1. Click `View permissions and data stored across sites`
2. Review each site's permissions
3. Click on any site to revoke unnecessary permissions
4. Delete site data you no longer need

#### Clear Browsing Data

**Path:** `Privacy and security` > `Clear browsing data`

**Recommended Frequency:** Weekly or more often

**What to Clear:**

**Basic Tab:**
- ✅ Browsing history
- ✅ Cookies and other site data
- ✅ Cached images and files

**Advanced Tab:**
- ✅ Browsing history
- ✅ Download history
- ✅ Cookies and other site data
- ✅ Cached images and files
- ✅ Site settings (if you don't mind reconfiguring permissions)
- ✅ Hosted app data
- ⚠️ Passwords (only if stored insecurely)
- ⚠️ Autofill form data (only if contains sensitive info)

**Time range:** Select "All time" for maximum privacy

💡 **Tip:** Chrome now automatically deletes some data:
- Ad topics older than 4 weeks
- Site-suggested ads older than 30 days
- One-time permissions when you leave a site

#### Security (Safe Browsing)

**Path:** `Privacy and security` > `Security`

Safe Browsing protects against malicious sites but shares data with Google.

**Three Options:**

1. **Enhanced Protection:** 
   - Most protection, most data sharing
   - Sends browsing data to Google proactively
   - Downloads analyzed in cloud
   - ❌ **Not recommended for privacy**

2. **Standard Protection (Recommended):**
   - Balanced protection
   - Checks URLs against known threats
   - Less data sent to Google
   - ✅ **Best balance of security and privacy**

3. **No protection:**
   - Maximum privacy, no security
   - ❌ **Not recommended - too risky**

**Additional Security Settings:**

- ✅ Enable: `Always use secure connections` (forces HTTPS)
  - Chrome 154+ (October 2026) will enable this by default
- ❌ Disable: `Use secure DNS` (prevents DNS leak but sends queries to Google)
  - Alternative: Configure DNS at OS/router level with privacy-focused provider

### 2. Sync and Google Services

**Path:** `Settings` > `You and Google`

#### Sign In Status

**Privacy Recommendation:** Don't sign in to Chrome with your Google account

**Why?**
- Sends all browsing history to Google
- Syncs data across devices (convenient but privacy-invasive)
- Links your browsing to your identity
- Makes you easier to track

**If You Must Sign In:**
1. Click `Manage what you sync`
2. Disable sync for:
   - ❌ History
   - ❌ Open tabs
   - ❌ Bookmarks (unless needed)
   - ❌ Passwords (use dedicated password manager instead)
   - ❌ Addresses and more
   - ❌ Payment methods
   - ❌ Settings (prevents privacy settings from syncing)
   - ⚠️ Extensions (enable only if essential)

**Alternative:** Use Chrome without signing in and:
- Bookmark important sites locally
- Use a password manager (Bitwarden, 1Password, KeePassXC)
- Manually back up bookmarks/settings as needed

#### Google Services

**Path:** `You and Google` > `Google services`

**Disable Everything:**

- ❌ `Allow Chrome sign-in` - Prevents accidental sign-ins
- ❌ `Make searches and browsing better` - Sends URLs/system info to Google
- ❌ `Help improve Chrome's features and performance` - Telemetry data
- ❌ `Make searches and browsing better in all Google services` - Broader tracking
- ❌ `Safe Browsing` - Already configured above
- ❌ `Preload pages for faster browsing and searching` - Sends prediction data

**Autocomplete Searches and URLs:**
- ❌ Disable if privacy is paramount
- This sends partial searches to Google as you type
- Alternative: Type full URL or use bookmarks

### 3. Autofill and Passwords

**Path:** `Settings` > `Autofill and passwords`

**Privacy Risks:**
- Passwords stored in Chrome are tied to Google account
- Addresses and payment info synced to Google servers
- Autofill can leak information to malicious sites

**Recommended Settings:**

#### Google Password Manager
- ❌ Disable `Offer to save passwords`
- ❌ Disable `Auto Sign-in`
- Delete all stored passwords
- Use dedicated password manager instead (Bitwarden, 1Password, KeePassXC)

**Why?**
- Chrome passwords sync to Google account
- Vulnerable if Google account is compromised
- Dedicated password managers have better security

#### Payment Methods
- Delete all saved payment methods
- ❌ Disable `Save and fill payment methods`
- Payment data is stored on Google servers

#### Addresses and More
- Delete all saved addresses
- ❌ Disable `Save and fill addresses`

### 4. Search Engine

**Path:** `Settings` > `Search engine`

**Default:** Google (tracks all searches)

**Privacy-Focused Alternatives:**

1. **DuckDuckGo** - No tracking, decent results
2. **Startpage** - Google results without tracking
3. **Brave Search** - Independent index, no tracking
4. **Qwant** - European, GDPR compliant

**To Change:**
1. Click `Manage search engines`
2. Find your preferred search engine in the list
3. Click the three dots > `Make default`
4. Or add a custom search engine manually

### 5. Extensions and Permissions

**Path:** `Extensions` > `Manage Extensions` (puzzle icon in toolbar)

**Privacy Risks:**
- Extensions can read everything you type
- Some extensions sell browsing data
- Extensions can inject ads and trackers

**Best Practices:**

1. **Minimize Extensions:**
   - Only install what you truly need
   - More extensions = larger attack surface

2. **Review Permissions:**
   - Click `Details` on each extension
   - Check `Site access` permissions
   - Change to `On specific sites` when possible
   - Remove extensions requesting excessive permissions

3. **Recommended Privacy Extensions:**
   - **uBlock Origin** - Content blocker (most important)
   - **Privacy Badger** - Automatic tracker blocker
   - **HTTPS Everywhere** - Force HTTPS (less needed with Chrome 154+)
   - **Decentraleyes** - Local CDN emulation
   - **ClearURLs** - Remove tracking parameters

4. **Extensions to Avoid:**
   - Free VPN extensions (often sell data)
   - "Privacy" extensions from unknown developers
   - Extensions with vague permission requests
   - Unmaintained extensions (check last update)

### 6. Downloads

**Path:** `Settings` > `Downloads`

**Recommended Settings:**

- ✅ Enable `Ask where to save each file before downloading`
  - Prevents automatic downloads
  - Lets you review files before saving
- Clear download history regularly
- Consider using a dedicated downloads folder that you clean regularly

### 7. Languages

**Path:** `Settings` > `Languages`

**Privacy Consideration:**

- ❌ Disable `Offer to translate pages that aren't in a language you read`
- Translation sends page content to Google servers
- This can leak sensitive information

**Alternative:**
- Use local translation tools
- Learn basic phrases in common languages
- Accept that some pages won't be translated

### 8. System

**Path:** `Settings` > `System`

**Recommended Settings:**

- ❌ Disable `Continue running background apps when Google Chrome is closed`
  - Prevents Chrome from running when closed
  - Stops background data collection
  - Saves system resources

- ❌ Disable `Use graphics acceleration when available` (optional)
  - May leak GPU information
  - Only disable if concerned about fingerprinting
  - Will impact performance

---

## Incognito Mode

**Path:** `File` > `New Incognito Window` or `Ctrl+Shift+N` / `Cmd+Shift+N`

**What It Does:**
- ✅ Doesn't save browsing history locally
- ✅ Deletes cookies when you close window
- ✅ Doesn't sync activity to Google account

**What It Doesn't Do:**
- ❌ Doesn't hide browsing from ISP, employer, or websites
- ❌ Doesn't prevent Google from tracking signed-in activity
- ❌ Doesn't block fingerprinting or trackers
- ❌ Extensions still work (unless disabled for Incognito)

**Making Incognito More Private:**

1. **Disable Extensions in Incognito:**
   - Go to `Extensions` > `Manage Extensions`
   - For each extension, click `Details`
   - Turn off `Allow in Incognito`
   - Exception: Keep privacy extensions (uBlock Origin, Privacy Badger)

2. **Don't Sign In:**
   - Never sign into Google or other accounts in Incognito
   - Defeats the purpose of private browsing

3. **Consider Using Alongside These:**
   - Private DNS configuration
   - VPN (trusted provider only)
   - Tor Browser (for maximum anonymity)

💡 **Better Alternative:** Use a separate browser profile or different browser entirely for sensitive browsing.

---

## Chrome Flags (Advanced)

**Path:** Type `chrome://flags` in the address bar

⚠️ **Warning:** These are experimental features. Change at your own risk.

**Privacy-Enhancing Flags:**

| Flag | Setting | Purpose |
|------|---------|---------|
| `#enable-parallel-downloading` | Enabled | Faster downloads (privacy neutral) |
| `#enable-quic` | Disabled | Disable Google's QUIC protocol (privacy) |
| `#enable-webrtc-hide-local-ips-with-mdns` | Enabled | Prevents WebRTC IP leaks |
| `#reduced-referrer-granularity` | Enabled | Limits referrer info sent to sites |

**To Change a Flag:**
1. Search for the flag name
2. Click the dropdown menu
3. Select `Enabled` or `Disabled`
4. Click `Relaunch` to apply changes

---

## Additional Privacy Hardening

### 1. Use Multiple Profiles

Create separate Chrome profiles for different activities:

**Steps:**
1. Click your profile icon in the top right
2. Click `Add` > `Sign in` or `Continue without an account`
3. Name the profile (e.g., "Work," "Personal," "Shopping")

**Benefits:**
- Compartmentalizes browsing data
- Different extensions per profile
- Separate cookie stores
- Makes tracking harder

### 2. Regular Maintenance

**Weekly:**
- Clear browsing data
- Review site permissions
- Check installed extensions

**Monthly:**
- Review Chrome flags
- Update Chrome to latest version
- Check for compromised passwords
- Review synced data (if signed in)

**Quarterly:**
- Audit all privacy settings
- Consider switching browsers
- Review Google account activity

### 3. DNS Configuration

**Why?**
- Your ISP can see every domain you visit
- DNS queries leak your browsing

**Options:**

1. **Browser-Level (Not Recommended):**
   - Chrome's "Use secure DNS" sends queries to Google
   - Better than nothing but still sends data to Google

2. **System-Level (Better):**
   - Configure at OS level
   - Privacy-focused providers:
     - **Quad9** (9.9.9.9)
     - **Cloudflare** (1.1.1.1) - Fast but Cloudflare sees queries
     - **NextDNS** - Customizable, privacy-focused

3. **Router-Level (Best):**
   - Configure on your router
   - Protects all devices on network
   - Same privacy DNS providers as above

### 4. Network Security

**Use HTTPS Always:**
- Chrome 154+ (October 2026) will enforce this by default
- Manually enable in `Privacy and security` > `Security` > `Always use secure connections`

**Be Cautious of:**
- Public WiFi networks (use VPN)
- Self-signed certificates
- Certificate warnings

### 5. Fingerprinting Protection

**What is Fingerprinting?**
- Sites identify you by unique browser characteristics
- Includes fonts, plugins, screen resolution, timezone, language
- Works even with cookies blocked

**Mitigation (Limited in Chrome):**

Chrome has weak fingerprinting protection. Consider:
- Use browser extensions (like Canvas Blocker)
- Disable WebGL, WebRTC (breaks some sites)
- Use privacy-focused browsers (Firefox, Brave) for sensitive activities
- Keep browser updated (less unique)
- Don't use unusual configurations

**Better Solution:** Use browsers with built-in fingerprinting protection:
- **Firefox** with privacy settings + extensions
- **Brave** - Built-in protection
- **Mullvad Browser** - Maximum protection
- **Tor Browser** - Complete anonymity

---

## What Data Chrome Still Collects

Even with all privacy settings maximized, Chrome still collects:

### Always Collected (Regardless of Settings):

1. **Technical Data:**
   - IP address (visible to sites you visit)
   - Browser version and OS
   - Screen resolution and viewport size
   - Installed fonts (used by sites for fingerprinting)
   - Timezone and language preferences
   - Hardware information (CPU, GPU for performance)

2. **Website-Provided Data:**
   - Sites can still track you with their own methods
   - First-party cookies remain functional
   - Fingerprinting scripts can still run
   - Analytics tools still work

3. **Google Integration:**
   - If you use any Google services (Gmail, YouTube, Search)
   - Google can correlate your activity across services
   - Even without Chrome sign-in

4. **Network-Level Data:**
   - ISP can see all domains you visit (unless using VPN)
   - DNS queries reveal browsing (unless using encrypted DNS)
   - Websites see your IP address

5. **Mandatory Telemetry:**
   - Crash reports (can be disabled)
   - Some security checks
   - Update checks

### Collected If Signed In (Even with Limited Sync):

- Sign-in status tied to Google account
- Relationship between device and account
- Basic account information
- Some activity even with sync disabled

### Cannot Be Prevented in Chrome:

- Google's proprietary components
- Some Chrome-specific tracking mechanisms
- Integration with Google services
- Closed-source portions of Chrome

---

## Verifying Your Privacy Settings

### 1. Privacy Check Tools

**Browser Leaks:**
- Visit [browserleaks.com](https://browserleaks.com)
- Check for WebRTC leaks, IP leaks, fingerprinting
- Review what information sites can collect

**Cover Your Tracks:**
- Visit [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- Tests browser fingerprinting protection
- Shows how unique your browser is

**DNS Leak Test:**
- Visit [dnsleaktest.com](https://dnsleaktest.com)
- Verify DNS queries aren't leaking

### 2. Google Account Activity

If signed into Chrome or Google services:

1. Visit [myactivity.google.com](https://myactivity.google.com)
2. Review Chrome history
3. Check Web & App Activity
4. Delete activity and pause tracking
5. Visit [myaccount.google.com/data-and-privacy](https://myaccount.google.com/data-and-privacy)
6. Review all privacy settings

### 3. Chrome Internal Pages

**Useful Chrome URLs:**

- `chrome://settings/content` - Quick access to site settings
- `chrome://settings/privacy` - Privacy settings
- `chrome://settings/syncSetup` - Sync configuration
- `chrome://settings/passwords` - Password manager
- `chrome://settings/clearBrowserData` - Clear data
- `chrome://components` - Component versions
- `chrome://extensions` - Manage extensions
- `chrome://net-internals/#dns` - DNS status
- `chrome://histograms` - Usage statistics (telemetry data)

---

## Alternative Browsers to Consider

If maximum privacy is your goal, Chrome may not be the best choice:

### Chromium-Based (Similar to Chrome):

1. **Brave**
   - Built-in ad blocker and tracker protection
   - Automatic HTTPS upgrades
   - Fingerprinting protection
   - Tor mode for anonymity
   - ✅ Recommended

2. **Ungoogled Chromium**
   - Chrome without Google services
   - More manual configuration required
   - No automatic updates
   - Advanced users only

3. **Microsoft Edge**
   - Similar privacy issues (Microsoft instead of Google)
   - Better than Chrome for Windows users
   - Enhanced tracking prevention

### Firefox-Based (Different Engine):

1. **Firefox**
   - Strong privacy features
   - Extensive customization
   - Open source
   - Good extension support
   - ✅ Highly recommended

2. **LibreWolf**
   - Firefox with privacy hardening by default
   - No telemetry
   - Strong fingerprinting protection

3. **Mullvad Browser**
   - Based on Tor Browser
   - Strong privacy without using Tor
   - Limited features for maximum privacy

### Maximum Privacy:

1. **Tor Browser**
   - Complete anonymity
   - Routes through Tor network
   - Best for sensitive activities
   - Slower than regular browsers

---

## Privacy-Respecting Chrome Alternatives Summary

| Browser | Privacy | Usability | Speed | Recommendation |
|---------|---------|-----------|-------|----------------|
| **Chrome (Hardened)** | ⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | Daily browsing, Google services |
| **Brave** | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | Best Chrome alternative |
| **Firefox** | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | Strong all-rounder |
| **Tor Browser** | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐ | Maximum privacy |

---

## Frequently Asked Questions

**Q: Is Chrome safe to use if I follow this guide?**  
A: Chrome can be made more private, but it will never be as privacy-respecting as Firefox or Brave. Google's business model relies on data collection. If privacy is critical, consider alternatives.

**Q: Will these settings break websites?**  
A: Most settings won't break sites. Blocking third-party cookies may cause issues on some sites (embedded content, payment processors). Add site-specific exceptions as needed.

**Q: Should I use Chrome's built-in password manager?**  
A: No. Use a dedicated password manager like Bitwarden, 1Password, or KeePassXC. These offer better security, encryption, and don't tie your passwords to Google.

**Q: What about Chrome on mobile (iOS/Android)?**  
A: Mobile Chrome has similar privacy issues. On iOS, consider Safari with privacy extensions. On Android, consider Brave or Firefox. Mobile Chrome settings are in the app's menu under Settings > Privacy and security.

**Q: Does Incognito mode make me anonymous?**  
A: No. Incognito only prevents local history storage. Websites, ISP, employer, and Google can still track you. Use Tor Browser for anonymity.

**Q: Can I use Chrome for work and a privacy browser for personal use?**  
A: Yes, this is a good strategy. Use separate browsers or Chrome profiles to compartmentalize activities.

**Q: What about Chrome's "Privacy Sandbox"?**  
A: Privacy Sandbox (Topics API, FLEDGE) replaces third-party cookies but still enables tracking. We recommend disabling all Ad Privacy features as shown in this guide.

**Q: Should I use a VPN with Chrome?**  
A: A VPN hides your IP from websites and your ISP but doesn't prevent Google or websites from tracking you through other means. It's complementary to, not a replacement for, privacy settings.

---

## Summary: Essential Actions

If you only do three things from this guide, do these:

### 1. Disable Ad Privacy Features
- Settings > Privacy and security > Ad privacy
- Turn off: Ad topics, Site-suggested ads, Ad measurement

### 2. Don't Sign Into Chrome
- Use Chrome without a Google account
- Use password manager instead of Chrome's
- Bookmark manually or export bookmarks

### 3. Block Third-Party Cookies
- Settings > Privacy and security > Cookies and other site data
- Select "Block third-party cookies"

**Additional Quick Win:**
- Install uBlock Origin extension
- This single extension blocks most trackers and ads

---

## Resources

### Official Documentation
- [Chrome Privacy Whitepaper](https://www.google.com/chrome/privacy/whitepaper.html)
- [Chrome Privacy Policy](https://www.google.com/chrome/privacy/)
- [Chrome Help Center - Privacy](https://support.google.com/chrome/answer/14225066)

### Privacy Tools
- [Privacy Badger](https://privacybadger.org/) - Automatic tracker blocker
- [uBlock Origin](https://ublockorigin.com/) - Content blocker
- [Have I Been Pwned](https://haveibeenpwned.com/) - Check for data breaches
- [Cover Your Tracks](https://coveryourtracks.eff.org/) - Browser fingerprinting test

### Learning Resources
- [Electronic Frontier Foundation](https://www.eff.org/)
- [Privacy Guides](https://www.privacyguides.org/)
- [The Markup](https://themarkup.org/) - Privacy journalism

---

## Changelog

### Version 1.0 - February 15, 2026
- Initial release
- Covers Chrome 145 (current stable version)
- Includes new one-time permissions feature
- Updated for HTTPS by default (Chrome 154, October 2026)
- Ad Privacy (Topics API) configuration
- Chrome Flags for privacy

---

**Last Updated:** February 15, 2026  
**Chrome Version Tested:** 145.x (Stable Channel)  
**Next Review:** April 2026 (Chrome 147 - Enhanced Safe Browsing HTTPS enforcement)

⚠️ **Important:** Chrome updates frequently. Some settings may move or change names. If you find outdated information, please [report it](https://github.com/mechobliterate/privacyguard/issues).

---

*This guide is part of the [Sentinel](https://github.com/mechobliterate/sentinel) project - comprehensive privacy settings documentation for all platforms.*
