# Firefox Privacy Settings

<div align="center">
  <img src="../images/browsers/firefox/firefox-logo.svg" alt="Firefox Logo" width="120" height="120">
</div>

## Overview

Mozilla Firefox is an open-source browser with a strong privacy focus and commitment to user freedom. Unlike Chrome and Edge, Firefox is developed by the non-profit Mozilla Foundation, which doesn't rely on advertising revenue. Firefox offers extensive privacy features, customization options, and transparency that make it one of the best choices for privacy-conscious users.

**Key Privacy Features:**
- Enhanced Tracking Protection (blocks trackers by default)
- Total Cookie Protection (isolates cookies per-site)
- DNS over HTTPS by default
- Open source and auditable
- Extensive privacy-focused extensions
- No forced account sign-in
- Facebook Container built-in
- HTTPS-Only Mode
- Query stripping

**Privacy Advantages:**
- Mozilla's mission prioritizes privacy over profit
- Independent from Google/Microsoft ecosystems
- Highly customizable with about:config
- Strong anti-fingerprinting measures
- Minimal telemetry (can be fully disabled)
- Regular security updates

**This guide will help you:**
- Maximize Firefox's already strong privacy
- Configure advanced privacy settings
- Disable optional telemetry
- Select privacy-respecting extensions
- Use Firefox's unique privacy features effectively

---

## Quick Settings Checklist

### Essential Privacy Settings
- [ ] Set Enhanced Tracking Protection to "Strict"
- [ ] Enable "Delete cookies and site data when Firefox is closed"
- [ ] Disable telemetry and data collection
- [ ] Enable DNS over HTTPS
- [ ] Enable HTTPS-Only Mode
- [ ] Disable Firefox Suggest
- [ ] Turn off address bar suggestions
- [ ] Configure custom search engine (DuckDuckGo, etc.)
- [ ] Disable autofill for passwords and addresses
- [ ] Review and limit permissions

### Advanced Privacy Settings
- [ ] Configure about:config privacy settings
- [ ] Enable Resist Fingerprinting (power users)
- [ ] Install privacy extensions (uBlock Origin)
- [ ] Use Multi-Account Containers
- [ ] Disable WebRTC (if not needed)
- [ ] Set privacy-focused DNS provider
- [ ] Review add-on permissions

---

## Detailed Configuration

### 1. Privacy & Security Settings

**Path:** `Settings` > `Privacy & Security` (or about:preferences#privacy)

This is Firefox's primary privacy control center.

#### Enhanced Tracking Protection (ETP)

**Location:** Top of Privacy & Security page

**Three Levels:**

1. **Standard** (Default)
   - Blocks known trackers in Private Windows
   - Blocks tracking cookies
   - Blocks cryptominers and fingerprinters
   - Good for most users

2. **Strict** (Recommended for Privacy)
   - Blocks all detected trackers
   - Blocks all third-party cookies
   - May break some websites
   - ✅ **Maximum privacy**

3. **Custom**
   - Choose what to block
   - For advanced users
   - Can fine-tune protection

**Recommended:** Set to "Strict"

**What Strict Blocks:**
- ✅ Trackers (Social media, Cross-site, all windows)
- ✅ Tracking cookies (all third-party cookies)
- ✅ Cryptominers
- ✅ Fingerprinters
- ✅ Known tracking content

**Managing Exceptions:**

If a site breaks with Strict:
1. Click shield icon in address bar
2. Toggle "Enhanced Tracking Protection is ON for this site"
3. Reload page
4. Review and remove exceptions regularly

**Site Report:**
- Click shield icon to see what's blocked
- View detailed protection report
- See tracking attempts across all sites

#### Website Privacy Preferences

**Send websites a "Do Not Track" signal:**

Options:
- Always
- Only when Enhanced Tracking Protection is set to Strict
- Never

**Recommended:** "Always"

Why: Tells websites you don't want tracking. Many ignore it, but no harm in enabling.

#### Cookies and Site Data

**Delete cookies and site data when Firefox is closed:**

✅ **Enable this** for maximum privacy

**What it does:**
- Automatically deletes all cookies on exit
- Clears site data
- Forces fresh login each session

⚠️ **Note:** You'll need to log in to sites each time you start Firefox.

**Exceptions:**
- Click "Manage Exceptions"
- Add sites you want to stay logged into
- Use sparingly - each exception reduces privacy

**Manage Data:**
- Click "Manage Data" to see all stored cookies
- Review and delete unwanted data
- Search for specific sites

#### Logins and Passwords

**Recommended:** ❌ Disable all Firefox password management

- Uncheck "Ask to save logins and passwords for websites"
- Uncheck "Autofill logins and passwords"
- Uncheck "Suggest and generate strong passwords"

**Why?**
- Firefox Sync stores passwords on Mozilla servers
- Dedicated password managers offer better security
- Better cross-platform support

**Recommended Alternative:**
- **Bitwarden** (open source, free)
- **1Password** (paid, excellent UX)
- **KeePassXC** (local, maximum security)

#### History

**Firefox will:**

Options:
1. Remember history (default)
2. Never remember history (always private)
3. Use custom settings for history

**Recommended for Privacy:** "Use custom settings for history"

**Custom Settings:**
- ✅ "Always use private browsing mode" - Maximum privacy, but less convenient
- ✅ "Clear history when Firefox closes" - Good balance
  - Select: Browsing & Download History, Cookies, Cache, Active Logins, Site Preferences

**Or:** Keep history but clear regularly (weekly)

#### Address Bar - Firefox Suggest

**Firefox Suggest shows suggestions based on:**

❌ **Disable all of these:**
- "Browsing history"
- "Bookmarks"
- "Open tabs"
- "Shortcuts"
- "Search engines"
- "Suggestions from sponsors" (ads)
- "Suggestions from the web"

**Why disable:**
- Reduces data leakage through suggestions
- Some "web suggestions" send queries to Mozilla
- Sponsored suggestions are ads
- More private to type complete URLs

**Alternative:**
- Use bookmarks for frequent sites
- Type complete URLs
- Use search engine directly

#### Permissions

**Default Permissions for All Sites:**

| Permission | Recommended Setting |
|------------|---------------------|
| Location | Block new requests |
| Camera | Block new requests |
| Microphone | Block new requests |
| Notifications | Block new requests |
| Autoplay | Block Audio and Video |
| Virtual Reality | Block new requests |

**To Configure:**
1. Scroll to "Permissions" section
2. Click "Settings" next to each permission
3. Check "Block new requests to access your [permission]"
4. Review existing exceptions and remove unnecessary ones

#### Firefox Data Collection and Use

**Disable All Data Collection:**

❌ Uncheck all of these:
- "Allow Firefox to send technical and interaction data to Mozilla"
- "Allow Firefox to install and run studies"
- "Allow Firefox to send backlogged crash reports on your behalf"

**Why disable:**
- Telemetry sends detailed usage data
- Studies can modify browser behavior
- Crash reports may contain sensitive information
- Not necessary for functionality

**Exception:** If you want to help Firefox development, keep crash reports enabled but disable the others.

#### Security

**Deceptive Content and Dangerous Software Protection:**

✅ **Keep these enabled:**
- "Block dangerous and deceptive content"
- "Block dangerous downloads"
- "Warn you about unwanted and uncommon software"

**Why keep enabled:**
- Real security benefit
- Minimal privacy cost (hashed URLs)
- Protects against malware and phishing

**HTTPS-Only Mode:**

✅ **Enable in all windows**

**What it does:**
- Attempts HTTPS connection first
- Warns if site only supports HTTP
- Prevents unencrypted connections

**Strong privacy and security benefit - always enable**

#### DNS over HTTPS

✅ **Enable "Max Protection"**

**What it is:**
- Encrypts DNS queries
- Prevents ISP from seeing domains you visit
- Prevents DNS hijacking

**Provider Selection:**

**Default:** Cloudflare or NextDNS

**Options:**
1. **Cloudflare** (1.1.1.1)
   - Fast, privacy-focused
   - Doesn't log queries (allegedly)
   
2. **NextDNS**
   - Highly customizable
   - Can block ads/trackers at DNS level
   - Free tier available

**Recommended:** NextDNS for customization, Cloudflare for simplicity

**To change provider:**
1. Select "Max Protection"
2. Choose "Custom" from dropdown
3. Enter DNS provider URL:
   - Cloudflare: `https://mozilla.cloudflare-dns.com/dns-query`
   - NextDNS: `https://dns.nextdns.io/[your-id]`

---

### 2. Search Settings

**Path:** `Settings` > `Search` (or about:preferences#search)

#### Default Search Engine

**Default:** Google (tracks all searches)

**Privacy-Focused Alternatives:**

1. **DuckDuckGo** - Best privacy, good results
2. **Startpage** - Google results, no tracking
3. **Brave Search** - Independent, no tracking
4. **Qwant** - European, GDPR compliant
5. **Searx** - Meta-search, customizable

**Recommended:** DuckDuckGo or Startpage

**To Change:**
1. Select preferred search engine from dropdown
2. Or click "Find more search engines" to add others

#### Search Suggestions

❌ **Disable both:**
- "Provide search suggestions"
- "Show search suggestions in address bar results"

**Why disable:**
- Sends every keystroke to search engine
- Leaks search intent before you search
- Creates detailed profile of interests

#### Search Shortcuts

**Optional:** Can disable if you prefer
- Shows one-letter shortcuts for searches (g for Google, etc.)
- Minimal privacy impact

---

### 3. General Settings

**Path:** `Settings` > `General` (or about:preferences#general)

#### Startup

**When Firefox starts:**

**Recommended:** "Show a blank page"

**Why:**
- Doesn't load content on startup
- Prevents tracking on startup page
- Faster startup

**Alternative:** "Show your windows and tabs from last time" if you need session restoration

#### Tabs

**Minimal privacy impact** - Configure as preferred

**Recommended Tab Settings:**
- ❌ Disable "Ctrl+Tab cycles through tabs in recently used order"
- ❌ Disable "Open links in tabs instead of new windows"
- Configure as preferred

#### Language and Appearance

**No privacy impact** - Set as preferred

**Theme:** Dark mode doesn't affect privacy

#### Digital Rights Management (DRM) Content

**Firefox will:**

Options:
- Play DRM-controlled content (default)
- Ask to activate (manual control)

**For Privacy:** Keep enabled but monitor

DRM is necessary for Netflix, Spotify, etc. Disabling breaks these services.

#### Browsing

**Recommended Settings:**

❌ Disable "Recommend extensions as you browse"
- Reduces data sent to Mozilla

❌ Disable "Recommend features as you browse"
- Reduces Mozilla tracking

✅ Enable "Use autoscrolling" (optional - no privacy impact)

✅ Enable "Use smooth scrolling" (optional - no privacy impact)

✅ Enable "Always check if Firefox is your default browser" (optional)

❌ Disable "Warn you when websites try to install add-ons"
- Personal preference

#### Network Settings

**Configure Proxy Access:**

If you use a VPN or proxy:
1. Click "Settings"
2. Configure proxy settings
3. Most users: "Use system proxy settings" or "No proxy"

**For Tor users:**
- Manual proxy configuration
- SOCKS Host: 127.0.0.1
- Port: 9050

---

### 4. Home Settings

**Path:** `Settings` > `Home` (or about:preferences#home)

**Firefox Home Content:**

❌ **Disable everything for maximum privacy:**
- "Shortcuts"
- "Sponsored shortcuts"
- "Recommended by Pocket" (Mozilla collects data)
- "Recent activity"
- "Snippets"

**Why disable:**
- Home page content requires loading data from Mozilla
- "Recommended by Pocket" tracks reading
- Sponsored shortcuts are ads
- Recent activity can expose history

**Alternative:** Set homepage to blank or custom URL

---

### 5. Sync Settings

**Path:** `Settings` > `Sync` (or about:preferences#sync)

#### Firefox Account and Sync

**Privacy Recommendation:** Don't use Firefox Sync for maximum privacy

**Why?**
- All sync data stored on Mozilla servers
- End-to-end encrypted (Mozilla can't read it)
- But creates single point of failure
- Links devices to single identity

**If You Must Sync:**

1. Create Firefox Account with dedicated email
2. Choose what to sync carefully:
   - ⚠️ Bookmarks (okay)
   - ❌ History (avoid)
   - ❌ Open Tabs (avoid)
   - ❌ Logins (use password manager)
   - ❌ Add-ons (manual install preferred)
   - ⚠️ Settings (can leak privacy preferences)
   - ❌ Addresses (avoid)
   - ❌ Payment Methods (avoid)

**Better Alternative:**
- Export/import bookmarks manually
- Use password manager for passwords
- Keep devices separate for privacy

---

### 6. Extensions and Add-ons

**Path:** `Settings` > `Extensions & Themes` (or about:addons)

#### Essential Privacy Extensions

**Must-Have:**

1. **uBlock Origin** (Content Blocker)
   - Blocks ads, trackers, malware
   - Highly customizable
   - Open source
   - **Most important extension**

2. **Privacy Badger** (Automatic Tracker Blocker)
   - Learns which trackers to block
   - Made by EFF
   - Complements uBlock Origin

**Highly Recommended:**

3. **Decentraleyes** (CDN Emulation)
   - Serves common libraries locally
   - Prevents CDN tracking
   - Improves privacy and speed

4. **ClearURLs** (URL Cleaner)
   - Removes tracking parameters from URLs
   - Prevents click tracking

5. **Facebook Container** (Built into Firefox)
   - Isolates Facebook from rest of browsing
   - Already included in Firefox

6. **Cookie AutoDelete** (Cookie Manager)
   - Automatically deletes cookies
   - More granular than Firefox's built-in option

7. **HTTPS Everywhere** (Force HTTPS)
   - Less needed with HTTPS-Only Mode
   - But still useful for extra protection

#### Managing Extension Permissions

**Best Practices:**

1. **Minimize Extensions**
   - Only install what you truly need
   - Each extension is potential privacy risk

2. **Review Permissions:**
   - Click on extension
   - Click "..." > "Manage"
   - Review permissions requested
   - Remove extensions with excessive permissions

3. **Extension Privacy:**
   - Prefer open-source extensions
   - Check developer reputation
   - Read reviews for privacy concerns
   - Avoid extensions from unknown sources

4. **Private Browsing Permissions:**
   - By default, extensions don't work in Private Windows
   - Only enable for trusted privacy extensions

#### Multi-Account Containers

**Built-in Firefox Feature** - Excellent for privacy

**What it does:**
- Isolates cookies, storage, and login sessions
- Different "containers" for different contexts
- Prevents cross-site tracking

**How to Use:**

1. Right-click tab
2. Select "Reopen in Container"
3. Choose container (Personal, Work, Banking, Shopping)

**Create Custom Containers:**

1. Install "Multi-Account Containers" extension (official Mozilla)
2. Create containers for different purposes
3. Assign sites to containers automatically

**Example Setup:**
- **Personal:** General browsing
- **Work:** Work-related sites
- **Shopping:** E-commerce sites
- **Social:** Social media (isolated from everything)
- **Banking:** Financial sites only

**Benefits:**
- Amazon can't track you on other sites
- Facebook isolated from browsing
- Work and personal completely separate
- Superior privacy compartmentalization

---

## Advanced Privacy Settings (about:config)

**Path:** Type `about:config` in address bar

⚠️ **Warning:** Advanced settings. Incorrect values can break Firefox.

**Accept the risk and continue**

### Essential Privacy Tweaks

**Search for each preference and modify:**

#### Disable Telemetry Completely

```
toolkit.telemetry.enabled = false
toolkit.telemetry.unified = false
toolkit.telemetry.archive.enabled = false
datareporting.healthreport.uploadEnabled = false
datareporting.policy.dataSubmissionEnabled = false
```

#### Disable Pocket

```
extensions.pocket.enabled = false
```

#### Disable Firefox Studies

```
app.shield.optoutstudies.enabled = false
```

#### Enhanced Privacy

```
privacy.firstparty.isolate = true
privacy.resistFingerprinting = true (see warning below)
privacy.trackingprotection.enabled = true
privacy.trackingprotection.fingerprinting.enabled = true
privacy.trackingprotection.cryptomining.enabled = true
```

⚠️ **Warning on Resist Fingerprinting:**
- `privacy.resistFingerprinting = true` provides strong anti-fingerprinting
- But can break some websites (timezone, screen resolution changes)
- Test before keeping enabled
- Power users only

#### WebRTC Privacy

```
media.peerconnection.enabled = false
```

⚠️ Disables WebRTC (video chat, voice calls). Only disable if you don't need it.

**Alternative (less breaking):**
```
media.peerconnection.ice.default_address_only = true
media.peerconnection.ice.no_host = true
```

#### Disable Prefetching

```
network.dns.disablePrefetch = true
network.prefetch-next = false
network.predictor.enabled = false
```

Prevents Firefox from loading pages before you click.

#### Disable Location Bar Suggestions

```
browser.urlbar.suggest.searches = false
browser.urlbar.suggest.history = false
browser.urlbar.suggest.bookmark = false
browser.urlbar.suggest.openpage = false
browser.urlbar.suggest.topsites = false
```

#### Disable Geolocation

```
geo.enabled = false
```

Completely disables geolocation API (more aggressive than per-site permission).

### Arkenfox User.js

**For Advanced Users:**

[Arkenfox user.js](https://github.com/arkenfox/user.js) is a comprehensive Firefox privacy configuration:

- Pre-configured privacy settings
- Extensively documented
- Regularly updated
- Aggressive privacy hardening

**Warning:** Very aggressive. Will break many websites. Only for advanced users comfortable with troubleshooting.

---

## Private Browsing Mode

**How to Access:** `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac)  
**Or:** Menu > `New Private Window`

**What It Does:**
- ✅ Doesn't save browsing history
- ✅ Doesn't save cookies (deleted on close)
- ✅ Doesn't save form data
- ✅ Enhanced Tracking Protection to "Strict" automatically
- ✅ Doesn't save searches

**What It Doesn't Do:**
- ❌ Doesn't hide browsing from ISP
- ❌ Doesn't prevent websites from seeing IP
- ❌ Doesn't make you anonymous
- ❌ Doesn't prevent all tracking

**Extensions in Private Windows:**

By default, extensions don't run in Private Windows.

**To Enable (for privacy extensions only):**
1. Go to about:addons
2. Click extension
3. Click "..." > "Manage"
4. Enable "Run in Private Windows"
5. Only enable for trusted privacy extensions (uBlock Origin, Privacy Badger)

---

## DNS Privacy Configuration

### Option 1: Firefox Built-in DNS over HTTPS

**Already covered above** - Enable in Privacy & Security settings

### Option 2: System-Level Configuration

**Windows:**
- Settings > Network & Internet > Properties > DNS
- Add DNS servers: 9.9.9.9 (Quad9) or 1.1.1.1 (Cloudflare)

**macOS:**
- System Settings > Network > Advanced > DNS
- Add DNS servers

**Linux:**
- Edit `/etc/resolv.conf` or use NetworkManager

### Recommended DNS Providers

1. **Quad9** (9.9.9.9)
   - Blocks malware
   - Privacy-focused
   - Non-profit

2. **Cloudflare** (1.1.1.1)
   - Fast
   - Privacy policy
   - But Cloudflare sees all queries

3. **NextDNS**
   - Customizable filtering
   - Blocks ads/trackers
   - Privacy-focused

---

## What Data Firefox Still Collects

Even with all settings optimized:

### Always Collected:

1. **Technical Data:**
   - IP address (visible to websites)
   - User agent (browser version, OS)
   - Screen resolution (can be randomized with resistFingerprinting)
   - Language and timezone

2. **Website Data:**
   - First-party cookies (necessary)
   - Sites can still fingerprint (Firefox fights this)
   - Session data

3. **Minimal Telemetry:**
   - Only if explicitly enabled
   - Can be completely disabled
   - Firefox is most transparent about this

4. **Network Visibility:**
   - ISP can see domains visited (unless using VPN/DoH)
   - Websites see IP address

### If Sync Enabled:

- Sync data on Mozilla servers
- End-to-end encrypted
- Mozilla can't read it
- But still centralized storage

### Cannot Be Prevented:

- Some website tracking techniques
- Network-level visibility (unless VPN)
- Hardware fingerprinting vectors

**Firefox's Advantage:** You can disable almost all Mozilla telemetry, unlike Chrome/Edge.

---

## Verifying Your Privacy Settings

### 1. Firefox Privacy Tools

**Enhanced Tracking Protection Report:**
- Visit about:protections
- See what Firefox has blocked
- Review statistics
- Check for data breaches (Firefox Monitor)

### 2. External Privacy Tests

**Cover Your Tracks:**
- Visit [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- Tests fingerprinting protection
- Firefox scores well with resistFingerprinting

**Browser Leaks:**
- Visit [browserleaks.com](https://browserleaks.com)
- Comprehensive leak testing
- Check WebRTC, canvas, audio fingerprinting

**DNS Leak Test:**
- Visit [dnsleaktest.com](https://dnsleaktest.com)
- Verify DNS over HTTPS working

### 3. Firefox Internal Pages

**Useful about: pages:**

- `about:config` - Advanced settings
- `about:preferences#privacy` - Privacy settings
- `about:protections` - Protection report
- `about:networking` - Network information
- `about:telemetry` - Telemetry data (should be empty if disabled)
- `about:support` - Troubleshooting information

---

## Firefox vs Other Browsers

### Privacy Comparison

| Feature | Firefox | Chrome | Safari | Brave | Edge |
|---------|---------|--------|--------|-------|------|
| **Default Privacy** | ⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ |
| **Tracking Prevention** | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ |
| **Open Source** | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐ |
| **Customization** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ |
| **Extension Support** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Performance** | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **No Telemetry** | ⭐⭐⭐⭐⭐ | ⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐ |

### Firefox Advantages

✅ **Fully open source**  
✅ **Strong default privacy**  
✅ **Can disable all telemetry**  
✅ **Non-profit backing (Mozilla)**  
✅ **Excellent extension ecosystem**  
✅ **Multi-Account Containers**  
✅ **Highly customizable**  
✅ **Independent engine (not Chromium)**  
✅ **Strong anti-fingerprinting**

### Firefox Limitations

❌ **Slightly slower than Chrome/Edge**  
❌ **Some website compatibility issues**  
❌ **Smaller market share (but improving)**  
❌ **Mozilla has some questionable partnerships (Google search, Pocket)**

---

## Frequently Asked Questions

**Q: Is Firefox really more private than Chrome?**  
A: Yes, significantly. Firefox is open source, disables tracking by default, and allows you to completely disable telemetry. Mozilla doesn't rely on advertising like Google.

**Q: Should I use Firefox for privacy?**  
A: Absolutely. Firefox is one of the best choices for privacy, alongside Brave. It's the best non-Chromium option.

**Q: Can I completely disable Firefox telemetry?**  
A: Yes, through Settings and about:config. Firefox respects your privacy choices, unlike Chrome/Edge.

**Q: What about Firefox Sync privacy?**  
A: Firefox Sync is end-to-end encrypted - Mozilla can't read your data. But it's still centralized. For maximum privacy, don't use sync.

**Q: Should I use resistFingerprinting?**  
A: For advanced users, yes. But it breaks some sites (timezone, screen resolution changes). Test before keeping enabled.

**Q: What's the difference between Firefox and LibreWolf?**  
A: LibreWolf is Firefox with privacy hardening by default (no telemetry, enhanced tracking protection). It's more aggressive but also more likely to break sites.

**Q: Can I use Firefox without a Mozilla account?**  
A: Yes, and this is recommended for maximum privacy. Firefox works perfectly without an account.

**Q: Is Firefox better than Brave for privacy?**  
A: Both are excellent. Firefox is more customizable and fully open source. Brave has stronger defaults and built-in ad blocking. Choose based on preference.

---

## Summary: Essential Actions

Minimum steps for Firefox privacy:

### 1. Set Enhanced Tracking Protection to Strict
- Settings > Privacy & Security
- Select "Strict"

### 2. Disable All Telemetry
- Settings > Privacy & Security
- Uncheck all data collection options

### 3. Enable HTTPS-Only Mode
- Settings > Privacy & Security
- Enable in all windows

### 4. Configure DNS over HTTPS
- Settings > Privacy & Security
- Enable "Max Protection"

### 5. Install uBlock Origin
- Visit addons.mozilla.org
- Search "uBlock Origin"
- Install

**Bonus Actions:**
- Use Multi-Account Containers
- Enable "Delete cookies when Firefox closes"
- Switch search engine to DuckDuckGo
- Configure about:config privacy settings

---

## Resources

### Official Documentation
- [Firefox Privacy Notice](https://www.mozilla.org/privacy/firefox/)
- [Firefox Security Best Practices](https://support.mozilla.org/kb/firefox-security-and-privacy)
- [Mozilla Privacy Policy](https://www.mozilla.org/privacy/)

### Privacy Hardening
- [Arkenfox user.js](https://github.com/arkenfox/user.js) - Advanced privacy config
- [PrivacyTools Firefox](https://privacytools.io/browsers/#firefox) - Privacy guide

### Extensions
- [uBlock Origin](https://addons.mozilla.org/firefox/addon/ublock-origin/)
- [Privacy Badger](https://addons.mozilla.org/firefox/addon/privacy-badger17/)
- [Multi-Account Containers](https://addons.mozilla.org/firefox/addon/multi-account-containers/)

### Testing
- [Cover Your Tracks](https://coveryourtracks.eff.org/)
- [Browser Leaks](https://browserleaks.com/)

---

## Changelog

### Version 1.0 - February 15, 2026
- Initial release
- Covers Firefox 123 (current release)
- Enhanced Tracking Protection configuration
- Total Cookie Protection
- DNS over HTTPS setup
- about:config privacy tweaks
- Multi-Account Containers guide

---

**Last Updated:** February 15, 2026  
**Firefox Version Tested:** 123.x (Release Channel)  
**Next Review:** April 2026 (Firefox 125)

⚠️ **Note:** Firefox updates every 4 weeks. Settings are generally stable but check for updates.

---

*This guide is part of the [Sentinel](https://github.com/mechobliterate/sentinel) project - comprehensive privacy settings documentation for all platforms.*
