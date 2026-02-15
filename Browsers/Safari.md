# Safari Privacy Settings

<div align="center">
  <img src="../images/browsers/safari/safari-logo.svg" alt="Safari Logo" width="120" height="120">
</div>

## Overview

Safari is Apple's web browser, available on macOS, iOS, and iPadOS. Apple positions Safari as a privacy-focused browser with features like Intelligent Tracking Prevention, Privacy Report, and minimal data collection. Unlike Chrome, Apple's business model doesn't rely on advertising, giving Safari a natural privacy advantage.

**Key Privacy Features:**
- Intelligent Tracking Prevention (ITP) blocks cross-site tracking
- Privacy Report shows blocked trackers
- Built-in fingerprinting protection
- Private Relay for iCloud+ subscribers (hides IP address)
- Minimal telemetry compared to other browsers
- On-device processing for many features
- Automatic HTTPS upgrading

**Privacy Concerns:**
- Closed-source components
- Google is default search engine (but easily changed)
- iCloud sync can expose browsing data if iCloud compromised
- Limited extension ecosystem
- Some tracking prevention can be bypassed

**This guide will help you:**
- Maximize Safari's privacy features
- Disable unnecessary data collection
- Configure tracking prevention
- Manage website permissions
- Optimize iCloud sync settings

---

## Quick Settings Checklist

### Essential Privacy Settings (macOS)
- [ ] Enable "Prevent cross-site tracking"
- [ ] Enable "Hide IP address from trackers"
- [ ] Disable "Allow privacy-preserving measurement of ad effectiveness"
- [ ] Set "Block all cookies" or "Block cookies from third parties"
- [ ] Disable AutoFill for sensitive data
- [ ] Turn off search engine suggestions
- [ ] Configure iCloud sync (disable History if privacy-focused)
- [ ] Review and limit website permissions
- [ ] Enable "Warn when visiting a fraudulent website"
- [ ] Disable preloading of top hit

### iOS/iPadOS Settings
- [ ] Enable "Prevent Cross-Site Tracking" 
- [ ] Enable "Hide IP Address" (for iCloud+ subscribers)
- [ ] Disable "Privacy Preserving Ad Measurement"
- [ ] Block all cookies or cookies from third parties
- [ ] Turn off Safari suggestions
- [ ] Review Camera & Microphone access
- [ ] Disable Location Services for Safari

---

## Detailed Configuration (macOS)

### 1. Privacy Settings

**Path:** `Safari` > `Preferences` > `Privacy` (macOS Ventura and earlier)  
**Path:** `Safari` > `Settings` > `Privacy` (macOS Sonoma and later)

#### Prevent Cross-Site Tracking

**Setting:** ✅ Enabled (Default)

This is Safari's most powerful privacy feature:
- Blocks cookies and website data from tracking you across sites
- Uses machine learning to identify tracking domains
- Automatically deletes tracking data after 30 days
- Constantly updated by Apple

**Keep this enabled** - It's one of the best anti-tracking features in any browser.

#### Hide IP Address

**Options:**
- **Trackers only** (Recommended) - Hides IP from known trackers
- **Trackers and websites** - Maximum privacy, requires iCloud+
- **Off** - Your IP is visible

**Recommended Setting:** "Trackers only" or "Trackers and websites" (if you have iCloud+)

**What it does:**
- Routes requests through Apple's servers
- Trackers can't use your IP to identify you
- Similar to a VPN but only for Safari
- "Trackers and websites" option provides more comprehensive protection

⚠️ **Note:** "Trackers and websites" requires iCloud+ subscription and may slow down browsing slightly.

#### Website Tracking: Prevent Cross-Site Tracking

**Setting:** ✅ Enable "Prevent cross-site tracking"

Already covered above - keep this on.

#### Privacy Preserving Ad Measurement

**Setting:** ❌ Disable "Allow privacy-preserving measurement of ad effectiveness"

**What it is:**
- Apple's alternative to traditional ad tracking
- Allows advertisers to measure ad effectiveness
- Claims to preserve privacy through aggregation
- Processes data on-device

**Why disable it:**
- Still enables ad tracking, just in a "private" way
- You're helping advertisers even if anonymously
- Not necessary for browsing functionality
- True privacy is not measuring ads at all

#### Cookies and Website Data

**Options:**
1. **Block all cookies** - Maximum privacy, breaks many sites
2. **Block cookies from third parties** - Good balance (Recommended)
3. **Allow cookies from websites you visit** - Minimal protection
4. **Always allow cookies** - No privacy protection

**Recommended:** "Block cookies from third parties"

**Managing Existing Cookies:**
1. Click `Manage Website Data`
2. Review sites with stored data
3. Remove sites you don't recognize or trust
4. Click `Remove All` for clean slate (requires re-login to sites)

💡 **Tip:** Regularly clear website data (monthly recommended)

#### Website Use of Location Services

**Recommended:** Set to "Deny without prompting" or "Prompt for each website once per day"

Most websites don't need your location. Only allow when necessary (maps, weather).

### 2. General Settings

**Path:** `Safari` > `Settings` > `General`

#### Safari Opens With

**Recommended:** "A new private window" (for maximum privacy)

Alternative: "A new window" with empty page

Avoid: "All windows from last session" - Can leak browsing history

#### Remove History Items

**Recommended:** "After one year" or more frequently

Options:
- After one day (most private)
- After one week  
- After two weeks
- After one month
- After one year
- Manually

Consider: Manually clear history regularly for sensitive browsing

#### Remove Download List Items

**Recommended:** "Upon successful download" or "Manually"

Prevents download history from accumulating.

### 3. AutoFill Settings

**Path:** `Safari` > `Settings` > `AutoFill`

**Privacy Risk:** AutoFill data can be exposed to malicious websites through various attacks.

**Recommended Settings:**

- ❌ Disable "Using information from my contacts"
- ❌ Disable "User names and passwords" (use password manager instead)
- ❌ Disable "Credit cards" (enter manually or use Apple Pay)
- ❌ Disable "Other forms"

**Why?**
- Safari passwords sync to iCloud (security risk if compromised)
- Malicious sites can extract autofill data
- Password managers (Bitwarden, 1Password) offer better security
- Credit card info should never be stored in browsers

**Alternative:** Use dedicated password manager and Apple Pay for payments.

### 4. Search Settings

**Path:** `Safari` > `Settings` > `Search`

#### Search Engine

**Default:** Google (tracks all searches)

**Privacy-Focused Alternatives:**
1. **DuckDuckGo** - No tracking, decent results (Recommended)
2. **Ecosia** - Privacy-focused, plants trees
3. **Startpage** - Google results without tracking

**To Change:**
1. Click "Search engine" dropdown
2. Select alternative
3. Click away to save

#### Search Engine Suggestions

**Setting:** ❌ Disable "Include search engine suggestions"

**Why disable:**
- Sends every keystroke to search provider as you type
- Leaks search intent before you even search
- Creates detailed profile of your interests
- Not necessary for functionality

#### Safari Suggestions

**Setting:** ❌ Disable "Include Safari Suggestions"

**What it does:**
- Sends browsing data to Apple
- Provides suggestions based on your activity
- Uses Apple's servers to process suggestions

**Why disable:**
- Sends data to Apple servers
- Not necessary for basic browsing
- Reduces data exposure

#### Quick Website Search

**Setting:** Your choice (minimal privacy impact)

Allows searching within sites (e.g., "wiki penguins" searches Wikipedia)

#### Preload Top Hit in the Background

**Setting:** ❌ Disable

**Why:**
- Loads pages before you click them
- Wastes bandwidth
- Can trigger tracking pixels
- Sends your browsing intent prematurely

### 5. Security Settings

**Path:** `Safari` > `Settings` > `Security`

#### Fraudulent Website Warning

**Setting:** ✅ Enable "Warn when visiting a fraudulent website"

**What it does:**
- Checks URLs against known phishing sites
- Sends limited data to Apple/Google Safe Browsing
- Protects against scams and malware

**Privacy consideration:**
- Minimal data shared (hashed URLs)
- Security benefit outweighs minor privacy cost
- Keep enabled unless extremely privacy-focused

#### JavaScript

**Setting:** ✅ Leave enabled

Disabling JavaScript breaks most modern websites. Only disable for specific sites via per-site settings.

### 6. Websites Settings (Per-Site Permissions)

**Path:** `Safari` > `Settings` > `Websites`

Configure default permissions for all websites:

**Recommended Defaults:**

| Permission | Setting | Reasoning |
|------------|---------|-----------|
| **Camera** | Deny | Require explicit permission |
| **Microphone** | Deny | Require explicit permission |
| **Location** | Deny | Most sites don't need location |
| **Screen Sharing** | Ask | Only for conferencing sites |
| **Downloads** | Ask | Review each download |
| **Pop-up Windows** | Block | Prevents malicious pop-ups |
| **Auto-Play** | Stop Media with Sound | Reduces annoyance |
| **Content Blockers** | On | Enable for all installed |
| **Page Zoom** | 100% | Personal preference |

**Managing Site-Specific Settings:**

1. Visit a website
2. Click Safari menu > `Settings for This Website`
3. Adjust permissions for that specific site
4. Changes apply only to that domain

**Review Existing Permissions:**
1. Go to `Websites` tab in Settings
2. Click each permission type
3. Review which sites have access
4. Revoke unnecessary permissions

### 7. Extensions

**Path:** `Safari` > `Settings` > `Extensions`

**Privacy Risk:** Extensions can read everything you do in Safari.

**Best Practices:**

1. **Minimize Extensions**
   - Only install what you absolutely need
   - More extensions = more privacy risk

2. **Review Permissions**
   - Check what each extension can access
   - Uninstall extensions with excessive permissions

3. **Recommended Privacy Extensions:**
   - **1Blocker** - Content blocking (paid but excellent)
   - **AdGuard** - Ad and tracker blocking
   - **Wipr** - Simple content blocker
   - **Hush** - Cookie consent banner blocker
   - **Ghostery** - Tracker blocker

4. **Extension Permissions:**
   - Click extension in toolbar
   - Select "Always Allow on Every Website" cautiously
   - Use "Only on This Website" when possible

### 8. Advanced Settings

**Path:** `Safari` > `Settings` > `Advanced`

#### Show Features for Web Developers

Optional - enables Develop menu for advanced users

#### Show Full Website Address

**Setting:** ✅ Enable

Shows complete URL in address bar - helps identify phishing attempts.

#### Default Encoding

Leave as "Default" unless you have specific needs.

---

## Detailed Configuration (iOS/iPadOS)

### 1. Safari Settings

**Path:** `Settings` > `Safari`

#### Privacy & Security Section

**Prevent Cross-Site Tracking:**
- ✅ Enable - Blocks cross-site cookies and data

**Hide IP Address:**
- Options: "Off", "Trackers", "Trackers and Websites"
- Recommended: "Trackers and Websites" (requires iCloud+)
- Or "Trackers" if you don't have iCloud+

**Privacy Preserving Ad Measurement:**
- ❌ Disable - Prevents ad tracking measurement

**Block All Cookies:**
- Recommended: Leave OFF (too restrictive)
- Alternative: Rely on "Prevent Cross-Site Tracking"

**Fraudulent Website Warning:**
- ✅ Enable - Protects against phishing

**Check for Apple Pay:**
- Personal preference - minimal privacy impact

#### Search Section

**Search Engine:**
- Default: Google
- Recommended: DuckDuckGo (Privacy-focused)

**Search Engine Suggestions:**
- ❌ Disable - Stops sending keystrokes to search provider

**Safari Suggestions:**
- ❌ Disable - Reduces data sent to Apple

**Quick Website Search:**
- Personal preference - minimal privacy impact

**Preload Top Hit:**
- ❌ Disable - Prevents preloading pages you might not visit

#### General Section

**AutoFill:**
- Tap "AutoFill"
- ❌ Disable "Use Contact Info"
- ❌ Disable "Names and Passwords" (use password manager)
- ❌ Disable "Credit Cards"

**Favorites:**
- Configure as preferred - no privacy impact

**Open Links:**
- Personal preference - no privacy impact

**Downloads:**
- Recommended: "Ask" before downloading

#### Tabs Section

Configure how tabs work - minimal privacy impact

**Close Tabs:**
- Recommended: "After One Week" or less
- Prevents old tabs from accumulating

### 2. System-Level Safari Settings

#### Location Services

**Path:** `Settings` > `Privacy & Security` > `Location Services` > `Safari Websites`

**Recommended:** "Never" or "Ask Next Time Or When I Share"

Most websites don't need your location.

#### Camera & Microphone

**Path:** `Settings` > `Privacy & Security` > `Camera/Microphone`

**Recommended:** Disable Safari access unless needed for specific sites

Safari will ask per-site when permission needed.

### 3. Clearing Browsing Data (iOS/iPadOS)

**Path:** `Settings` > `Safari` > `Clear History and Website Data`

**What it clears:**
- Browsing history
- Cookies and site data
- Cached files

**Recommended Frequency:** Weekly or after sensitive browsing

⚠️ **Note:** This logs you out of all websites.

**Advanced Clearing:**

**Path:** `Settings` > `Safari` > `Advanced` > `Website Data`

- Shows all sites storing data
- Can remove individual sites
- Click "Remove All Website Data" for complete wipe

---

## Private Browsing Mode

**How to Access:**
- **macOS:** `File` > `New Private Window` or `Cmd+Shift+N`
- **iOS/iPadOS:** Tap tabs button > "Private" > "+"

**What It Does:**
- ✅ Doesn't save browsing history
- ✅ Doesn't store cookies after closing
- ✅ Doesn't save form data
- ✅ Doesn't sync to iCloud
- ✅ Blocks known trackers more aggressively

**What It Doesn't Do:**
- ❌ Doesn't hide browsing from ISP or network admin
- ❌ Doesn't prevent websites from seeing your IP (unless using Hide IP feature)
- ❌ Doesn't make you anonymous
- ❌ Doesn't block all tracking

**Making Private Browsing More Effective:**

1. **Don't sign into accounts** in private windows
2. **Use with iCloud Private Relay** (if subscribed)
3. **Clear data** after each session
4. **Still use content blockers** - They work in private mode

💡 **Tip:** Private Browsing + iCloud Private Relay + Content Blockers = Maximum Safari privacy

---

## iCloud Sync Configuration

**Path (macOS):** `System Settings` > `Apple ID` > `iCloud` > `Safari`  
**Path (iOS):** `Settings` > `[Your Name]` > `iCloud` > `Safari`

**What Syncs:**

- Bookmarks
- Reading List
- Tabs (across devices)
- History
- Saved passwords
- AutoFill data
- Safari extensions

**Privacy Implications:**

- All data stored on Apple's iCloud servers
- Encrypted in transit and at rest
- Apple can decrypt if required by law
- Single point of failure if iCloud compromised

**Recommended Configuration:**

**For Maximum Privacy:**
- ❌ Disable Safari sync entirely
- Use local bookmarks only
- Use password manager instead of iCloud Keychain

**For Convenience with Some Privacy:**
- ✅ Enable Bookmarks sync
- ✅ Enable Reading List sync
- ❌ Disable History sync
- ❌ Disable passwords (use password manager)
- ⚠️ Enable Tabs sync only if needed

### Advanced iCloud Privacy

**Enable Advanced Data Protection (Recommended):**

**Path:** `System Settings` > `Apple ID` > `iCloud` > `Advanced Data Protection`

**What it does:**
- End-to-end encrypts most iCloud data
- Apple cannot decrypt your data
- Protects against breaches and government requests
- Requires iOS 16.2+ / macOS Ventura 13.1+

⚠️ **Important:** You must not lose your recovery key or you'll lose all data.

**What's protected:**
- Safari bookmarks
- iCloud Drive
- Notes
- Photos
- And much more

**Not protected:**
- iCloud Mail
- Contacts
- Calendar

✅ **Highly Recommended** if you use iCloud sync

---

## Privacy Report

**How to Access:**
- **macOS:** Click shield icon in toolbar
- **iOS:** Tap "AA" in address bar > "Privacy Report"

**What It Shows:**

1. **Trackers Prevented:**
   - Which trackers were blocked
   - Which websites had trackers
   - Tracker statistics over 30 days

2. **Websites Contacted:**
   - Which third-party sites were contacted
   - Helps identify tracking networks

**How to Use It:**

1. **Review regularly** to see tracking attempts
2. **Identify problematic sites** with many trackers
3. **Consider avoiding sites** with excessive tracking
4. **Share stats** to raise awareness

**Example Insights:**
- "This site contacted 37 trackers"
- "95% of trackers blocked in the last 30 days"
- "Google Analytics present on 45% of sites visited"

---

## Content Blockers

Safari supports content blocker extensions that remove ads, trackers, and unwanted content.

### Recommended Content Blockers

**1. 1Blocker** (Paid, $4.99/year)
- Comprehensive blocking rules
- Easy customization
- Excellent performance
- **Best overall option**

**2. AdGuard** (Free with pro version)
- Powerful blocking
- Custom filters
- Free tier is very capable

**3. Wipr** (Paid, $1.99)
- Simple, lightweight
- Minimal configuration
- "Set and forget"

**4. Hush** (Free)
- Specifically blocks cookie consent banners
- Makes browsing less annoying
- Use alongside other blockers

### How to Install Content Blockers

**macOS:**
1. Download from Mac App Store
2. Go to `Safari` > `Settings` > `Extensions`
3. Enable the content blocker
4. Configure rules if desired

**iOS/iPadOS:**
1. Download from App Store
2. Go to `Settings` > `Safari` > `Extensions`
3. Enable the extension
4. Or: `Settings` > `Safari` > `Content Blockers` and toggle on

### Configuring Content Blockers

Most allow customization:

**Recommended Settings:**
- ✅ Block ads
- ✅ Block trackers
- ✅ Block social media widgets
- ✅ Block cookie banners
- ✅ Remove annoyances
- ⚠️ Cosmetic filtering (can break some sites)

**Whitelisting Sites:**

If a site breaks:
1. Open site
2. Click content blocker icon
3. Disable for this site
4. Refresh page

---

## Developer Tools for Privacy (Advanced)

**Enable Develop Menu:**

**Path:** `Safari` > `Settings` > `Advanced` > `Show Develop menu in menu bar`

### Useful Privacy Tools in Develop Menu

**Empty Caches:**
- `Develop` > `Empty Caches`
- Clears cached resources
- More thorough than normal clearing

**Disable Images:**
- `Develop` > `Disable Images`
- Prevents image tracking pixels

**Disable JavaScript:**
- `Develop` > `Disable JavaScript`
- Breaks most sites but maximum privacy

**User Agent:**
- `Develop` > `User Agent` > Choose different browser
- Can reduce fingerprinting (limited effectiveness)

**Web Inspector:**
- Right-click > `Inspect Element`
- See what resources sites load
- Identify trackers manually

---

## What Data Safari Still Collects

Even with all settings optimized, Safari still collects some data:

### Always Collected:

1. **Technical Data:**
   - IP address (visible to websites unless using Hide IP)
   - User agent string (browser version, OS)
   - Screen resolution
   - Timezone and language preferences

2. **Website Data:**
   - Sites can still track with first-party cookies
   - Fingerprinting can still occur (though Safari fights this)
   - Session tracking within single sites

3. **Apple Telemetry:**
   - Minimal crash reports (can be disabled in System Settings)
   - Basic usage statistics if "Share with App Developers" enabled

4. **Search Provider Data:**
   - If using Google, all searches tracked by Google
   - Switch to DuckDuckGo to prevent this

5. **Network-Level Visibility:**
   - ISP can see all domains visited (unless using VPN/Private Relay)
   - DNS queries reveal browsing (use encrypted DNS)

### Collected If Signed Into iCloud:

- Sync data stored on iCloud servers
- Associated with your Apple ID
- Can be accessed by Apple if legally required (unless Advanced Data Protection enabled)

### Cannot Be Prevented:

- Safari's proprietary anti-tracking mechanisms (closed source)
- Some Apple telemetry
- Integration with macOS/iOS system features

---

## Verifying Your Privacy Settings

### 1. Privacy Check Tools

**Cover Your Tracks (EFF):**
- Visit [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- Tests browser fingerprinting
- Safari generally scores well

**Browser Leaks:**
- Visit [browserleaks.com](https://browserleaks.com)
- Check for various leaks
- Test WebRTC, IP, DNS

### 2. Safari Privacy Report

Check your Privacy Report regularly:
- Click shield icon in toolbar
- Review blocked trackers
- Identify problematic websites

### 3. Network Monitoring

**macOS:**
- Use Activity Monitor to see network connections
- Identify unexpected connections
- Look for data being sent to trackers

**iOS:**
- Limited native tools
- Consider network monitoring apps from App Store

---

## Advanced Privacy Enhancements

### 1. DNS Configuration

Safari uses system DNS settings.

**macOS Configuration:**

**Path:** `System Settings` > `Network` > Select connection > `Details` > `DNS`

**Privacy-Focused DNS Providers:**
- **Quad9:** 9.9.9.9 (Malware blocking)
- **Cloudflare:** 1.1.1.1 (Fast, privacy-focused)
- **NextDNS:** Customizable, privacy-focused

**Enable DNS over HTTPS/TLS:**
- Many providers support encrypted DNS
- Prevents ISP from seeing DNS queries

### 2. VPN Usage

VPNs complement Safari's privacy features:

**When to Use VPN:**
- Public WiFi networks
- Hiding browsing from ISP
- Accessing geo-restricted content
- Additional privacy layer

**iCloud Private Relay vs VPN:**

**Private Relay (iCloud+):**
- Safari only
- Free with iCloud+
- Two-hop architecture
- Apple + third party

**VPN:**
- System-wide protection
- Choose your own provider
- More control
- Usually paid

**Can use both together** for maximum privacy

### 3. Multiple Profiles (macOS Sonoma+)

**Path:** `Safari` > `Preferences` > `Profiles`

Create separate profiles for different uses:

**Example Setup:**
- **Personal:** General browsing
- **Work:** Work-related sites
- **Banking:** Financial sites only
- **Shopping:** E-commerce

**Benefits:**
- Separate cookies and data
- Different extensions per profile
- Compartmentalized tracking
- Clearer organization

### 4. Script Blocking

While Safari doesn't have native script blocking, content blockers can block scripts:

**Using 1Blocker/AdGuard:**
- Enable script blocking in settings
- Whitelist sites as needed
- Improves privacy and speed

---

## Safari vs Other Browsers

### Privacy Comparison

| Feature | Safari | Chrome | Firefox | Brave |
|---------|--------|--------|---------|-------|
| **Tracking Prevention** | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Default Privacy** | ⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Data Collection** | ⭐⭐⭐⭐ | ⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Fingerprinting Protection** | ⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Extension Support** | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Open Source** | ⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **macOS Performance** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Battery Efficiency** | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ |

### Safari Advantages

✅ **Excellent default privacy**  
✅ **Minimal data collection**  
✅ **Strong tracking prevention**  
✅ **Best macOS/iOS integration**  
✅ **Superior battery efficiency**  
✅ **Fast performance on Apple hardware**  
✅ **iCloud Private Relay option**

### Safari Limitations

❌ **Limited to Apple devices**  
❌ **Smaller extension ecosystem**  
❌ **Some closed-source components**  
❌ **Less customizable than Firefox**  
❌ **Occasional web compatibility issues**

---

## Frequently Asked Questions

**Q: Is Safari really more private than Chrome?**  
A: Yes. Apple doesn't rely on advertising revenue, giving Safari fewer privacy conflicts. Intelligent Tracking Prevention is more aggressive than Chrome's approach.

**Q: Should I use Safari if I care about privacy?**  
A: On Apple devices, Safari is an excellent choice. It balances privacy, performance, and usability well. For maximum privacy, consider Firefox or Brave, but Safari is very good.

**Q: What about iCloud sync - is it safe?**  
A: iCloud sync is encrypted but Apple holds the keys (unless you enable Advanced Data Protection). For maximum privacy, disable sync or enable Advanced Data Protection.

**Q: Can I use Safari extensions from Chrome?**  
A: No. Safari uses a different extension system. Many popular extensions have Safari versions, but not all.

**Q: Does Private Browsing make me anonymous?**  
A: No. It prevents local history storage but doesn't hide your identity from websites, ISP, or network admin. Use with VPN/Private Relay for better privacy.

**Q: Should I enable iCloud Private Relay?**  
A: If you have iCloud+, yes. It adds significant privacy by hiding your IP address and encrypting DNS queries. It's essentially a built-in VPN for Safari.

**Q: Is Safari fingerprinting protection effective?**  
A: Yes, Safari actively fights fingerprinting by limiting information exposed to websites. It's not perfect but better than most browsers.

**Q: Can I use Safari without an Apple ID?**  
A: Yes, Safari works without an Apple ID. You lose iCloud sync features but gain privacy.

---

## Summary: Essential Actions

If you only do five things from this guide:

### 1. Enable All Tracking Prevention
- Prevent Cross-Site Tracking: ON
- Hide IP Address: "Trackers" or "Trackers and Websites"
- Block third-party cookies

### 2. Disable Ad Measurement
- Privacy Preserving Ad Measurement: OFF

### 3. Disable Search Suggestions
- Search Engine Suggestions: OFF
- Safari Suggestions: OFF

### 4. Change Search Engine
- Switch from Google to DuckDuckGo

### 5. Install Content Blocker
- Install 1Blocker, AdGuard, or Wipr
- Enable in Safari settings

**Bonus Action:**
- Enable Advanced Data Protection for iCloud (if you use iCloud sync)

---

## Resources

### Official Documentation
- [Safari Privacy Overview](https://www.apple.com/safari/docs/Safari_White_Paper_Nov_2019.pdf)
- [Apple Platform Security Guide](https://support.apple.com/guide/security/welcome/web)
- [iCloud Advanced Data Protection](https://support.apple.com/en-us/HT212520)

### Privacy Tools
- [1Blocker](https://1blocker.com/) - Premium content blocker
- [AdGuard](https://adguard.com/en/adguard-safari/overview.html) - Free/paid content blocker
- [Wipr](https://giorgiocalderolla.com/wipr.html) - Simple content blocker
- [Hush](https://oblador.github.io/hush/) - Cookie banner blocker

### Testing Tools
- [Cover Your Tracks](https://coveryourtracks.eff.org/) - Fingerprinting test
- [Browser Leaks](https://browserleaks.com/) - Comprehensive leak testing

---

## Changelog

### Version 1.0 - February 15, 2026
- Initial release
- Covers Safari 17.3+ (macOS Sonoma)
- Safari 17.3+ (iOS 17.3/iPadOS 17.3)
- Includes iCloud Private Relay configuration
- Advanced Data Protection guidance
- macOS Sonoma profile features

---

**Last Updated:** February 15, 2026  
**Safari Version Tested:**
- macOS: Safari 17.3 (macOS Sonoma 14.3)
- iOS: Safari 17.3 (iOS 17.3)  
**Next Review:** May 2026 (Safari 17.5 / WWDC 2026)

⚠️ **Note:** Safari updates with macOS/iOS updates. Settings may vary slightly between versions.

---

*This guide is part of the [Sentinel](https://github.com/mechobliterate/sentinel) project - comprehensive privacy settings documentation for all platforms.*
