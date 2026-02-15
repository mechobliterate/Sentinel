# Brave Privacy Settings

<div align="center">
  <img src="../images/browsers/brave/brave-logo.svg" alt="Brave Logo" width="120" height="120">
</div>

## Overview

Brave is a privacy-focused browser built on Chromium with aggressive built-in ad and tracker blocking. Founded by Brendan Eich (co-founder of Mozilla and creator of JavaScript), Brave prioritizes privacy by default while maintaining Chrome compatibility. Unlike Chrome, Brave removes Google services and adds extensive privacy features without requiring extensions.

**Key Privacy Features:**
- Built-in ad and tracker blocking (no extensions needed)
- Automatic HTTPS upgrading
- Script blocking capabilities
- Fingerprinting protection
- Tor integration for anonymous browsing
- No telemetry sent to Brave (minimal opt-in only)
- Blocks third-party cookies by default
- Brave Search (privacy-focused, optional)
- Brave Shields (customizable protection)

**Privacy Advantages:**
- Privacy-first by default (unlike Chrome/Edge)
- No Google services or tracking
- Based on Chromium (fast, compatible)
- Built-in features don't require extensions
- Open source and auditable
- Aggressive blocking out of the box
- Optional Brave Rewards (crypto-based)

**Considerations:**
- Brave Rewards has privacy implications (optional)
- Some cryptocurrency integrations (optional)
- Smaller company than Mozilla/Google/Microsoft
- Business model based on optional ad replacement

**This guide will help you:**
- Maximize Brave's already excellent default privacy
- Configure Brave Shields optimally
- Disable optional features that may reduce privacy
- Use Tor mode effectively
- Avoid privacy pitfalls with Brave Rewards

---

## Quick Settings Checklist

### Essential Privacy Settings (Already Default)
- [x] Shields enabled (blocks ads and trackers)
- [x] Block third-party cookies
- [x] Upgrade connections to HTTPS
- [ ] Verify "Send usage ping to Brave" is OFF
- [ ] Disable Brave Rewards (unless you want it)
- [ ] Disable autocomplete in address bar
- [ ] Review WebRTC policy
- [ ] Disable "Get Notification Suggestions"
- [ ] Turn off social media blocking exceptions (if any)

### Advanced Privacy Settings
- [ ] Enable "Forget me when I close this site"
- [ ] Configure Brave Shields to Aggressive
- [ ] Disable WebRTC (if not needed)
- [ ] Use Brave Search as default
- [ ] Review and remove site exceptions
- [ ] Disable IPFS (unless you use it)
- [ ] Turn off Google services remaining
- [ ] Configure search engine suggestions

---

## Detailed Configuration

### 1. Brave Shields (Core Privacy Feature)

**Access:** Click the lion icon in the address bar, or Settings > Shields

Brave Shields is the heart of Brave's privacy protection. It's enabled by default and highly effective.

#### Default Shield Settings

**Path:** `Settings` > `Shields` (or brave://settings/shields)

**Trackers & ads blocking:**

Options:
- **Aggressive** - Blocks all third-party trackers and ads, may break sites
- **Standard** (Default) - Blocks most trackers and ads
- **Allow** - No blocking (not recommended)

**Recommended:** Start with "Standard", upgrade to "Aggressive" if comfortable

**What Standard Blocks:**
- ✅ Ad tracking scripts
- ✅ Known ad domains
- ✅ Third-party tracking cookies
- ✅ Most analytics

**What Aggressive Adds:**
- ✅ All third-party resources (more aggressive)
- ✅ Some first-party trackers
- ⚠️ May break more sites but maximum privacy

**Upgrade connections to HTTPS:**

✅ **Leave enabled** (Default)

Automatically upgrades all connections to HTTPS when available. Critical security and privacy feature.

**Block Scripts:**

Options:
- **On** - Blocks all JavaScript (breaks most sites)
- **Off** (Default) - Allows JavaScript

**Recommended:** Leave Off for daily browsing

**When to enable:**
- Reading articles (often works)
- Avoiding tracking on specific sites
- Maximum privacy on sensitive sites

💡 **Tip:** Enable per-site via Shield icon when needed, not globally.

**Block Fingerprinting:**

Options:
- **Strict** - Blocks all fingerprinting, randomizes info
- **Standard** (Default) - Blocks cross-site fingerprinting
- **Allow** - No fingerprinting protection

**Recommended:** Standard (Strict may break sites)

**What it does:**
- Randomizes canvas fingerprints
- Blocks fingerprinting scripts
- Makes browser less unique
- Protects against device identification

**Block Cookies:**

Options:
- **Block all cookies** - Maximum privacy, breaks most sites
- **Block cross-site cookies** (Default) - Good balance
- **Allow all cookies** - No privacy

**Recommended:** Block cross-site cookies (Default)

**Forget me when I close this site:**

✅ **Enable this**

Automatically deletes cookies and site data when you close a tab. Excellent privacy feature unique to Brave.

**Block Social media embeds:**

❌ **Disable this** (or leave optional)

- **Blocks**: Facebook, Twitter, LinkedIn, Google embedded content
- Can break sites that rely on these
- Provides privacy but reduces functionality

**Recommended:** Enable if you don't need social media embeds

**Additional Settings:**

**Send "Do Not Track":**
- ✅ Enable
- Standard feature, many sites ignore but no harm

**Auto-redirect AMP pages:**
- ✅ Enable
- Loads original site instead of Google AMP
- Better privacy (avoids Google)

**Auto-redirect tracking URLs:**
- ✅ Enable
- Removes tracking parameters from URLs
- Prevents click tracking

**De-AMP:**
- ✅ Enable
- Redirects from AMP to real page

#### Per-Site Shield Configuration

Click shield icon (lion) in address bar to adjust for specific sites:

**If a site breaks:**
1. Click shield icon
2. Turn shields down or off
3. Reload page
4. Only disable what's necessary

**Review exceptions regularly:**
Settings > Shields > View and manage shields on every site you visit

### 2. Privacy and Security Settings

**Path:** `Settings` > `Privacy and security` (or brave://settings/privacy)

#### Clear browsing data

**On exit:**
- Settings > Privacy and security > Clear browsing data > On exit
- Choose what to clear automatically

**Recommended to clear on exit:**
- ✅ Browsing history
- ✅ Download history
- ✅ Cookies and other site data
- ✅ Cached images and files
- ⚠️ Passwords (only if using password manager)
- ⚠️ Autofill form data (if contains sensitive info)

**Manual clearing:**
- Do weekly even if auto-clear enabled
- Select "All time" for time range

#### Site and Shields Settings

**Cookie settings:**

Already configured in Shields, but can fine-tune here:
- Block third-party cookies (Default)
- See sites with cookies stored
- Remove unwanted cookies

**Default permissions:**

Set restrictive defaults:

| Permission | Recommended Setting |
|------------|---------------------|
| Location | Block |
| Camera | Ask |
| Microphone | Ask |
| Notifications | Block |
| Background sync | Block |
| Motion sensors | Block |
| USB devices | Block |
| Serial ports | Block |
| MIDI devices | Block |
| Bluetooth | Block |
| File editing | Block |
| Clipboard | Ask |
| Window Management | Block |
| Fonts | Block (anti-fingerprinting) |
| Ethereum | Block |
| Solana | Block |
| Google Sign-In | Block |

#### WebRTC IP handling policy

**Critical Privacy Setting**

**Path:** Settings > Privacy and security > WebRTC

**Options:**
- **Default** - May leak IP
- **Default public interface only** - Limits leak
- **Disable non-proxied UDP** - Best privacy

**Recommended:** "Disable non-proxied UDP"

**To completely disable WebRTC:**
`brave://flags/#disable-webrtc` - Set to "Disabled"

⚠️ **Note:** Disabling WebRTC breaks video calls (Zoom, Meet, etc.)

#### Web3

**Brave Wallet (Crypto):**

If you don't use crypto:
- Settings > Web3 > "Nothing" (None)
- Removes wallet functionality
- Reduces attack surface

If you use crypto:
- Configure carefully
- Be aware of privacy implications
- Transactions may be traceable

**IPFS:**

❌ **Set to "Disabled"** if you don't use IPFS
- IPFS is decentralized storage protocol
- Not needed for regular browsing
- Disabling improves privacy

#### Search engine

**Default:** Brave Search (privacy-focused)

**Alternatives:**
- DuckDuckGo
- Startpage  
- Qwant

**Brave Search Advantages:**
- No tracking
- Independent index (not Google)
- Owned by Brave
- Anonymous

**To change:**
Settings > Search engine > Select from dropdown

#### Autocomplete

❌ **Disable search suggestions:**
- Settings > Search engine
- Uncheck "Show autocomplete suggestions in address bar"

**Why:**
- Sends keystrokes to search engine
- Leaks search intent
- Not necessary for functionality

#### Google Services

**Remaining Google Services:**

Brave removes most Google services but check:
- ❌ Disable "Autocomplete searches and URLs"
- ❌ Disable "Use Google services for push messaging"
- ❌ Disable any remaining Google integrations

### 3. Sync Settings

**Path:** `Settings` > `Sync` (or brave://settings/sync)

**Brave Sync:**

Brave Sync uses end-to-end encryption and doesn't go through Brave servers (peer-to-peer).

**Privacy Recommendation:** Use carefully or avoid

**Why exercise caution:**
- Still links devices together
- Potential single point of failure
- Browser profile becomes more valuable

**If You Use Sync:**

Choose what to sync:
- ⚠️ Bookmarks (okay)
- ❌ History (avoid for privacy)
- ❌ Extensions (manual install better)
- ❌ Open tabs (avoid)
- ❌ Passwords (use password manager)
- ❌ Addresses and more (avoid)
- ⚠️ Settings (can leak privacy preferences)

**Sync Chain Setup:**
- Creates QR code or code words
- Devices connect peer-to-peer
- More private than cloud sync
- But still connects devices

### 4. Autofill and Passwords

**Path:** `Settings` > `Autofill and passwords`

**Recommended:** ❌ Disable everything

Use a dedicated password manager instead:

**Passwords:**
- ❌ Disable "Offer to save passwords"
- ❌ Disable "Auto Sign-in"
- Delete any saved passwords

**Payment methods:**
- ❌ Disable "Save and fill payment methods"
- Delete any saved cards

**Addresses and more:**
- ❌ Disable "Save and fill addresses"
- Delete any saved addresses

**Why use password manager:**
- **Bitwarden** - Open source, excellent
- **1Password** - Great UX, cross-platform
- **KeePassXC** - Local only, maximum security

Better security, cross-platform, and not tied to browser.

### 5. Appearance Settings

**Path:** `Settings` > `Appearance`

**No major privacy implications** but:

**Brave Rewards button:**
- Remove from toolbar if not using Rewards
- Reduces clutter
- Minor privacy benefit

**Home button:**
- Show if desired
- Set to blank page or custom URL
- Avoid default Brave/sponsored pages

**Sidebar:**
- Disable if not using
- Reduces features that may call home

### 6. New Tab Page

**Path:** `Settings` > `New tab page` (or brave://settings/newTabPage)

**Recommended Minimal Configuration:**

❌ Disable:
- "Show Brave News" (may load content)
- "Show sponsored images" (ads, even if privacy-respecting)
- "Show Brave Rewards" (if not using)

✅ Keep if desired:
- Top sites (local only)
- Clock (local)
- Stats (local)

**Background images:**
- Choose solid color or none
- Sponsored images load from Brave servers
- Even if privacy-respecting, not necessary

### 7. Social Media Blocking

**Path:** `Settings` > `Social media blocking`

**Brave blocks social media trackers and embeds:**

✅ **Enable blocking for:**
- Google
- Facebook
- Twitter
- LinkedIn

**What it does:**
- Blocks login buttons
- Blocks social media widgets
- Prevents social media tracking
- May break sites using "Login with [Platform]"

**Recommended:** Enable all unless you use social login

### 8. Extensions

**Path:** `Settings` > `Extensions` (or brave://extensions)

**Key Advantage:** Brave's built-in blocking means fewer extensions needed

**Recommended Extensions (Optional):**

1. **uBlock Origin** (Even more blocking)
   - Additional blocking beyond Brave's
   - Custom filter lists
   - Advanced users only (Brave Shields usually sufficient)

2. **Privacy Badger**
   - Redundant with Brave Shields
   - But provides additional learning-based blocking

3. **Decentraleyes**
   - Local CDN emulation
   - Complements Brave nicely

4. **ClearURLs**
   - Brave does some of this
   - But ClearURLs is more comprehensive

**Generally:** Brave Shields handle most needs. Only add extensions if specific requirements.

**Managing Extension Permissions:**
- Review what each can access
- Disable in private windows by default
- Only enable trusted extensions

### 9. Brave Rewards (Optional - Privacy Implications)

**Path:** `Settings` > `Brave Rewards` (or brave://rewards)

**What is Brave Rewards:**
- Optional ad system
- Earn BAT (Basic Attention Token) cryptocurrency
- Privacy-respecting ads (local matching)
- Replace blocked ads with Brave ads
- Can tip creators

**Privacy Analysis:**

**✅ Private aspects:**
- Ad matching done locally
- No tracking across sites
- Doesn't send browsing history to Brave
- More private than traditional ads

**⚠️ Privacy concerns:**
- Creates Brave Rewards profile
- Wallet activity may be traceable
- Crypto transactions potentially linkable
- Engagement with system tracked locally

**Recommendation:**

**For Maximum Privacy:** ❌ Don't enable Brave Rewards

**If You Want Rewards:**
- Be aware of privacy trade-offs
- Understand crypto is pseudonymous not anonymous
- Brave can't see browsing, but sees reward interactions
- Consider using with Tor for maximum privacy

**To Disable Completely:**
- Settings > Brave Rewards > Leave disabled
- Remove Rewards icon from toolbar

---

## Private Browsing with Tor

**Path:** Menu > `New private window with Tor` or `Ctrl+Shift+N`

**What is Tor in Brave:**
- Routes traffic through Tor network
- Changes IP address
- Anonymous browsing
- Fingerprinting protection

**How to Use:**

1. Click menu (three lines)
2. Select "New private window with Tor"
3. New window opens with onion icon
4. All traffic routed through Tor

**What Tor Mode Does:**
- ✅ Hides IP address
- ✅ Routes through multiple nodes
- ✅ Encrypted connection
- ✅ Block fingerprinting
- ✅ Don't save history

**Limitations:**
- ❌ Slower than regular browsing
- ❌ Some sites block Tor
- ❌ Not full Tor Browser (less hardened)
- ❌ Extensions don't work in Tor windows

**When to Use Tor:**
- Accessing sensitive information
- Whistleblowing
- Avoiding censorship
- Maximum anonymity needed
- Political activism

**Best Practices with Tor:**
1. **Don't sign into accounts** - Defeats anonymity
2. **Don't enable extensions** - Can leak identity
3. **Don't maximize window** - Reduces fingerprinting effectiveness
4. **Use for entire session** - Don't switch between Tor and regular
5. **Avoid downloads** - Can reveal IP

**Tor vs VPN:**
- Tor: Maximum anonymity, slower, free
- VPN: Hides IP from sites, faster, usually paid
- Can use both together for maximum privacy

---

## Regular Private Windows (Without Tor)

**Access:** `Ctrl+Shift+N` (regular private window)

**What It Does:**
- ✅ Doesn't save history
- ✅ Cookies deleted on close
- ✅ Strict Shields settings
- ✅ No sync

**What It Doesn't Do:**
- ❌ Doesn't hide IP
- ❌ Doesn't prevent ISP visibility
- ❌ Doesn't provide anonymity

**Use regular private windows for:**
- Shopping without recommendations
- Checking sites without being logged in
- Temporary sessions
- Quick privacy (not anonymity)

**Use Tor windows for:**
- True anonymity
- Hiding from ISP
- Accessing blocked content
- Sensitive research

---

## Brave Flags (Advanced)

**Path:** Type `brave://flags` in address bar

⚠️ **Warning:** Experimental features. Change carefully.

**Privacy-Enhancing Flags:**

Most privacy features are built into settings. Flags are rarely needed for Brave.

**Useful Flags:**

| Flag | Setting | Purpose |
|------|---------|---------|
| `#brave-rewards` | Disabled | Completely remove Rewards (if desired) |
| `#brave-news` | Disabled | Remove Brave News feature |
| `#brave-wayback-machine` | Enabled/Disabled | Your preference |

**Generally:** Brave's settings are comprehensive. Flags rarely needed for privacy.

---

## What Data Brave Still Collects

Even with optimal settings:

### Always Collected (By Nature):

1. **Technical Data:**
   - IP address (visible to websites unless using Tor)
   - Browser fingerprint (Brave actively fights this)
   - Screen resolution, timezone, language
   - User agent

2. **Website Data:**
   - First-party cookies (necessary)
   - Sites can still attempt fingerprinting
   - Session data

3. **Network Visibility:**
   - ISP can see domains visited (unless using Tor/VPN)
   - Websites see IP (unless Tor/VPN)

### Brave Collects:

**With Default Settings:**
- Nothing sent to Brave servers
- No analytics
- No telemetry
- Completely local processing

**Only if Opted-In:**
- Crash reports (if enabled)
- Brave Rewards interactions (if using Rewards)
- Diagnostic data (if explicitly enabled)

**Brave's Transparency:**
- Open source - can verify claims
- No hidden telemetry
- Privacy policy is clear
- Independent audits available

**Brave's Advantage:** Among mainstream browsers, Brave collects the least data by default.

---

## Verifying Your Privacy Settings

### 1. Brave's Built-in Tools

**Brave Shields Stats:**
- Settings > Shields
- View "Total shields count"
- See lifetime blocking statistics

**Site-Specific Shields:**
- Click lion icon on any site
- See what's blocked on that page
- Adjust settings if needed

### 2. External Privacy Tests

**Cover Your Tracks:**
- Visit [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- Tests fingerprinting protection
- Brave scores excellently

**Browser Leaks:**
- Visit [browserleaks.com](https://browserleaks.com)
- Comprehensive leak testing
- Test WebRTC, canvas, audio
- Check for IP leaks

**DNS Leak Test:**
- Visit [dnsleaktest.com](https://dnsleaktest.com)
- Verify DNS privacy
- Test when using VPN

### 3. Brave Internal Pages

**Useful brave:// pages:**

- `brave://settings/shields` - Shield settings
- `brave://settings/privacy` - Privacy settings
- `brave://adblock` - Ad blocking lists
- `brave://rewards` - Rewards settings
- `brave://sync-internals` - Sync status
- `brave://flags` - Experimental features

---

## Brave vs Other Browsers

### Privacy Comparison

| Feature | Brave | Chrome | Firefox | Safari | Edge |
|---------|-------|--------|---------|--------|------|
| **Default Privacy** | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ |
| **Built-in Blocking** | ⭐⭐⭐⭐⭐ | ⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ |
| **Fingerprinting Protection** | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐ |
| **Tor Integration** | ⭐⭐⭐⭐⭐ | ⭐ | ⭐ | ⭐ | ⭐ |
| **Open Source** | ⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐ |
| **Performance** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Extension Support** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Ease of Use** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **No Telemetry** | ⭐⭐⭐⭐⭐ | ⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐ |

### Brave's Unique Advantages

✅ **Best privacy by default** - No configuration needed  
✅ **Built-in ad/tracker blocking** - No extensions required  
✅ **Tor integration** - Anonymous browsing built-in  
✅ **Brave Search** - Privacy-focused search  
✅ **Chrome compatible** - All Chrome extensions work  
✅ **Fast** - Chromium base, optimized  
✅ **No telemetry** - Respects privacy completely  
✅ **Fingerprinting protection** - Randomizes identifying info  

### Considerations

⚠️ **Cryptocurrency focus** - May not appeal to everyone  
⚠️ **Smaller company** - Less established than Mozilla/Google  
⚠️ **Brave Rewards** - Optional but promoted  
⚠️ **Chromium-based** - Google's dominance in web standards  

### When to Choose Brave

**Choose Brave if:**
- You want maximum privacy with zero configuration
- You're switching from Chrome and want compatibility
- You want built-in ad blocking without extensions
- You need Tor integration
- You want privacy without complexity

**Choose Firefox if:**
- You want a non-Chromium alternative
- You prefer full open source
- You want maximum customization
- You trust Mozilla's mission more

**Choose Safari if:**
- You're on Apple devices exclusively
- You want best battery life and performance on Mac
- You trust Apple's privacy claims

---

## Frequently Asked Questions

**Q: Is Brave really more private than Chrome/Firefox?**  
A: Brave has the best privacy BY DEFAULT. Firefox can be configured to match or exceed Brave's privacy, but Brave is more private out-of-the-box. Both are vastly better than Chrome.

**Q: Should I use Brave for privacy?**  
A: Absolutely. Brave is one of the two best privacy browsers (alongside Firefox). It's especially good if you want privacy without configuration.

**Q: What about Brave Rewards - is it private?**  
A: Brave Rewards is more private than traditional ads (local matching), but it's still ad-based and creates a profile. For maximum privacy, don't use Rewards.

**Q: Is Brave Search better than DuckDuckGo?**  
A: Both are excellent for privacy. Brave Search has an independent index. DuckDuckGo aggregates from various sources. Both don't track. Choose based on result quality preference.

**Q: Can I use Chrome extensions in Brave?**  
A: Yes! Brave supports all Chrome extensions from the Chrome Web Store. But you need fewer extensions because Brave has built-in blocking.

**Q: Should I use Tor mode in Brave or Tor Browser?**  
A: For maximum anonymity, use Tor Browser. For convenient anonymous browsing, Brave's Tor mode is good. Tor Browser is more hardened against fingerprinting.

**Q: Does Brave collect any data?**  
A: No telemetry by default. Only if you explicitly opt into diagnostics or use Brave Rewards. Brave is transparent and open source - you can verify.

**Q: How does Brave make money if ads are blocked?**  
A: Optional Brave Rewards (users can earn BAT). Some users enable Rewards, some don't. Brave also has Brave Search (no tracking, may have sponsored results).

---

## Summary: Essential Actions

Brave is private by default, but optimize further:

### 1. Verify Shields Are Aggressive (Optional)
- Settings > Shields
- Consider upgrading to "Aggressive" mode
- Standard is already excellent

### 2. Disable Brave Rewards (If Not Using)
- Settings > Brave Rewards
- Keep disabled
- Remove from toolbar

### 3. Configure Search Engine
- Settings > Search engine
- Select Brave Search or DuckDuckGo
- Disable autocomplete suggestions

### 4. Review WebRTC
- Settings > Privacy and security
- Set to "Disable non-proxied UDP"
- Or disable completely in flags

### 5. Enable "Forget Me When I Close This Site"
- Settings > Shields
- Enable automatic cookie deletion

**Bonus Actions:**
- Use Tor mode for sensitive browsing
- Disable IPFS and Web3 if not using crypto
- Minimize extensions (Brave handles most needs)
- Use Brave Search instead of Google

---

## Resources

### Official Documentation
- [Brave Privacy Features](https://brave.com/privacy-features/)
- [Brave Privacy Policy](https://brave.com/privacy/browser/)
- [Brave Security](https://brave.com/security/)

### Community Resources
- [Brave Community](https://community.brave.com/)
- [Brave GitHub](https://github.com/brave/brave-browser)
- [Brave Privacy FAQ](https://support.brave.com/hc/en-us/categories/360001059151-Privacy)

### Testing Tools
- [Cover Your Tracks](https://coveryourtracks.eff.org/)
- [Browser Leaks](https://browserleaks.com/)
- [DNS Leak Test](https://dnsleaktest.com/)

### Brave Search
- [Brave Search](https://search.brave.com/)
- Privacy-focused alternative to Google
- Independent index

---

## Changelog

### Version 1.0 - February 15, 2026
- Initial release
- Covers Brave 1.63 (current release)
- Brave Shields configuration
- Tor integration guide
- Brave Rewards privacy analysis
- WebRTC configuration
- Built-in privacy features

---

**Last Updated:** February 15, 2026  
**Brave Version Tested:** 1.63.x (Release Channel)  
**Next Review:** April 2026 (Brave 1.65)

⚠️ **Note:** Brave updates frequently. Settings are generally stable but check periodically.

---

*This guide is part of the [Sentinel](https://github.com/mechobliterate/sentinel) project - comprehensive privacy settings documentation for all platforms.*
