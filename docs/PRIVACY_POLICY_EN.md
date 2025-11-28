# Privacy Policy for Game4You

**Last Updated:** 2024

## 1. Introduction

Welcome to Game4You! This privacy policy explains how we collect, use, share, and protect your information when you use our mobile application Game4You (hereinafter referred to as "the App", "We", "Us", or "Our").

By using the App, you agree to the practices described in this privacy policy. If you do not agree to this policy, please do not use the App.

## 2. Data Controller

**App Developer:** Emil Hakanzon  
**Email:** hakanzon.dev@gmail.com  
**App:** Game4You

## 3. What Information Do We Collect?

### 3.1 Information Stored Locally on Your Device

The App stores the following information locally on your device using AsyncStorage:

#### 3.1.1 Personal Game Library

- Games you have added to your library
- Your game ratings (0-10)
- Your reviews and comments about games
- Hours played per game
- Game status (currently playing, completed, backlog, wishlist)
- Games you have liked
- Custom game lists (public or private)
- Dates when games were added and updated

#### 3.1.2 User Settings

- Selected genres for personalization
- Selected country/region for price searches
- Theme settings (dark/light mode)
- Onboarding status (whether you have completed the introduction)

#### 3.1.3 User Statistics

- Experience points (XP)
- User level
- Game statistics (total number of games, average rating, etc.)

#### 3.1.4 Search History

- Recent searches
- Search results and filter settings

#### 3.1.5 Cached Game Data

- Trending games
- New releases
- Pre-orders
- Fan favorites
- Game information from IGDB API

### 3.2 Automatically Collected Information

#### 3.2.1 Device Information

- Country/region (automatically identified from device language and region settings via `expo-localization`)
- Platform (iOS, Android, Web)
- Device type and screen size

#### 3.2.2 Technical Information

- App version
- Operating system version
- Errors and warnings (only for app improvement, stored locally)

### 3.3 Information We Do NOT Collect

The App does **NOT** collect:

- Personally identifiable information (name, email, phone number)
- Login credentials (authentication is currently not implemented)
- Location data (GPS)
- Contact information
- Payment information
- Biometric data
- Camera or microphone access

## 4. How Do We Use Your Information?

### 4.1 Local Data Storage

All your personal data is stored **only locally** on your device. We do not collect or transfer your data to our servers. Data is stored using:

- **AsyncStorage** - for persistent local storage
- **Zustand Store** - for application state with local persistence

### 4.2 Usage Purposes

We use the collected information to:

1. **Deliver App Functionality**
   - Display your personal game library
   - Save your ratings, reviews, and game statistics
   - Personalize your content based on your preferences
   - Cache game data for faster loading and offline use

2. **Improve User Experience**
   - Remember your settings and preferences
   - Show relevant game recommendations
   - Save your search history for quicker access

3. **App Improvement**
   - Identify and fix technical issues (errors are only logged locally)
   - Improve app performance and functionality

## 5. Third-Party Services and APIs

The App uses the following third-party services to deliver functionality:

### 5.1 IGDB (Internet Game Database) API

**Service:** Twitch/IGDB API  
**Purpose:** Retrieve game information, images, trailers, metadata  
**Data Shared:** Only game names and search terms (no personal data)  
**Privacy Policy Link:** [Twitch Privacy Policy](https://www.twitch.tv/p/legal/privacy-policy/)  
**Terms Link:** [IGDB Terms of Service](https://www.igdb.com/terms)

**What Happens:**

- The App makes API calls to IGDB to retrieve game data
- We use OAuth 2.0 client credentials flow (no user authentication)
- Only game names and search terms are sent to IGDB
- No personally identifiable information is shared

### 5.2 CheapShark API

**Service:** CheapShark Game Deals API  
**Purpose:** Display game prices and deals from various stores  
**Data Shared:** Only game names for price searches  
**Privacy Policy Link:** [CheapShark Privacy Policy](https://www.cheapshark.com/api/1.0)

**What Happens:**

- The App searches for game prices based on game names
- Only game names are sent to CheapShark
- No personal data is shared

### 5.3 Twitch Integration

**Service:** Twitch  
**Purpose:** Open game streams and trailers in Twitch app or browser  
**Data Shared:** Only game names to find relevant streams  
**Privacy Policy Link:** [Twitch Privacy Policy](https://www.twitch.tv/p/legal/privacy-policy/)

**What Happens:**

- The App can open Twitch links to display game streams
- This occurs via external browser or Twitch app
- No data is shared directly from our app

### 5.4 Expo Framework

**Service:** Expo (Expo SDK)  
**Purpose:** App development platform and runtime  
**Data Shared:** Technical app information (version, platform)  
**Privacy Policy Link:** [Expo Privacy Policy](https://expo.dev/privacy)

**What Happens:**

- Expo is used as the development platform
- Some Expo modules may collect technical information for functionality
- No personal data is shared with Expo

### 5.5 Expo Application Services (EAS)

**Service:** EAS Build  
**Purpose:** Build and distribute the app  
**Data Shared:** Only during the build process  
**Privacy Policy Link:** [Expo Privacy Policy](https://expo.dev/privacy)

## 6. Data Security

### 6.1 Local Security

We implement the following security measures to protect your data:

- **Local Storage:** All data is stored only on your device
- **No Server Transfer:** No personal data is transferred to our servers
- **Encryption:** Data is stored using AsyncStorage which uses the platform's secure storage mechanisms
- **No External Database:** We do not use any cloud database or external server

### 6.2 API Security

- **OAuth 2.0:** We use secure OAuth 2.0 flows for API authentication
- **HTTPS:** All API calls are made over secure HTTPS connections
- **Rate Limiting:** We implement rate limiting to protect against overuse
- **Token Management:** Access tokens are handled securely and automatically renewed

### 6.3 Security Limitations

Please note that:

- Data is stored locally and may be lost if the app is uninstalled
- We recommend regular backups of your device
- If your device is compromised, local data may be accessible

## 7. Data Sharing and Transfer

### 7.1 No Data Sharing

We do **NOT** share your personal data with third parties for marketing or other commercial purposes.

### 7.2 API Calls

When the App makes API calls to third-party services:

- Only necessary information (game names) is sent
- No personally identifiable information is shared
- API calls are made directly from your device to the third-party service

### 7.3 International Data Transfer

Since we use third-party services (IGDB, CheapShark), data may be transferred internationally. These services may have servers outside the EU/EEA. Please refer to each service's privacy policy for more information.

## 8. Your Rights

Since all data is stored locally on your device, you have full control over your data:

### 8.1 Access to Your Data

- All your data is directly available in the App
- You can view all stored data in your settings and library

### 8.2 Right to Delete

You can at any time:

- Clear all data by uninstalling the App
- Clear specific data via the App's settings (e.g., search history)
- Delete individual games from your library

### 8.3 Right to Correct

- You can update your data at any time directly in the App
- Change ratings, reviews, settings, etc.

### 8.4 Data Portability

- Data is stored locally on your device
- You can back up your device to retain data
- Currently, there is no export function, but this may be added in future versions

## 9. Data Retention

### 9.1 Local Storage

- Data is stored on your device until you delete it or uninstall the App
- Cached game data is automatically updated and old data is cleared
- Cache duration: 1 hour for game data

### 9.2 Data Loss

Please note that:

- If you uninstall the App, all local data will be deleted
- We recommend that you regularly back up your device
- We are not responsible for data loss upon uninstallation

## 10. Children's Privacy

The App is not specifically targeted at children under 13 years of age. We do not knowingly collect information from children. If you are a parent or guardian and discover that your child has provided us with personal information, please contact us.

## 11. Cookies and Tracking

The App does **NOT** use cookies or tracking technologies. We do not collect data for marketing or advertising purposes.

## 12. Changes to This Privacy Policy

We may update this privacy policy from time to time. We will:

- Update the "Last Updated" date
- Notify you of significant changes via the App
- Request your consent if the changes require it

We recommend that you review this policy regularly to stay informed about how we protect your information.

## 13. GDPR and Data Protection Regulation

### 13.1 Legal Basis

Since all data is stored locally on your device and we do not collect personal data on our servers, GDPR applies limitedly. We only process data that you actively create in the App.

### 13.2 Your GDPR Rights

You have the right to:

- **Access:** View all your data in the App
- **Rectification:** Update your data at any time
- **Erasure:** Delete data by uninstalling the App
- **Restriction:** Restrict data processing (do not use specific features)
- **Data Portability:** Back up your device to retain data
- **Object:** Stop using the App

## 14. California Consumer Privacy Act (CCPA)

If you are a California resident, you have the right to:

- Know what personal information is collected
- Know if your personal information is sold or shared
- Say no to the sale of personal information (we do not sell data)
- Access your personal information
- Deletion of your personal information

## 15. Contact Information

If you have questions or concerns about this privacy policy or our handling of your information, please contact us:

**App Developer:** Emil Hakanzon  
**Email:** hakanzon.dev@gmail.com  
**App:** Game4You

## 16. Third-Party Privacy Policies

For more information on how third-party services handle your information, see:

- **Twitch/IGDB:** [Twitch Privacy Policy](https://www.twitch.tv/p/legal/privacy-policy/)
- **CheapShark:** [CheapShark Privacy Policy](https://www.cheapshark.com/api/1.0)
- **Expo:** [Expo Privacy Policy](https://expo.dev/privacy)

## 17. Summary

**Key Points:**

- ✅ All data is stored locally on your device
- ✅ No personal data is shared with third parties
- ✅ No server or cloud database is used
- ✅ You have full control over your data
- ✅ You can delete all data by uninstalling the App
- ✅ API calls are made only to retrieve game information (no personal data)

## 18. Consent

By using the Game4You app, you acknowledge that you have read, understood, and agree to this privacy policy. If you do not agree to this policy, please uninstall the App and do not use it.

---

**Game4You** - Your personal gaming companion, powered by the world's most comprehensive game database.

_This privacy policy is written in English. In case of translations to other languages, the English version shall prevail in case of conflicts._
