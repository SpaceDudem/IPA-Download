# Pastel (The Most Powerful IPA Download Tool to Date)

A tool for installing historical versions of IPA files. It can retrieve older versions of apps and automatically capture the required data packets. After downloading an IPA, you can transfer it directly to an iPhone or iPad through AirDrop, then install and use it.

Currently, it supports only Macs running macOS 26 or later with Apple silicon. Since the developer does not currently own a Windows PC, there are no plans to develop a Windows version at this time.

Built with SwiftUI and fully adapted to the Liquid Glass visual effects in macOS 26.

# Main Page

Pastel makes it easy to browse and search for apps in the App Store for a selected region. More importantly, it can automatically select the appropriate store based on the region associated with your chosen Apple Account.

When switching regions, it will also automatically switch to a signed-in Apple Account associated with that region. It even supports downloading an app that has never previously been downloaded using that Apple Account.

<img width="1214" height="881" alt="image" src="https://github.com/user-attachments/assets/690166e2-78ad-42f8-9db2-40b79e435b71" />
<img width="956" height="656" alt="image" src="https://github.com/user-attachments/assets/f3685fee-445f-41bc-8fea-2d1e602dec92" />

# Supported Languages

Pastel currently supports Simplified Chinese, Traditional Chinese, Japanese, Korean, and Thai as its primary interface languages.

<img width="1032" height="732" alt="image" src="https://github.com/user-attachments/assets/e6ef07a0-8834-457d-87f7-0bea14b45633" />

# An Exceptionally Powerful Downloads Page

You can find downloaded IPA files directly on the Downloads page and preview each app’s icon.

This is especially useful for apps that temporarily change their icons for advertising during specific holidays or sales events, such as China’s June 18 shopping festival.

Click the Share button to AirDrop the IPA directly to your iPhone or iPad for installation.

<img width="1138" height="805" alt="image" src="https://github.com/user-attachments/assets/1de14592-ebc6-4ee7-9b0c-17e7e0073171" />

# First-Time Setup

When using Pastel for the first time, go to:

“Settings” > “Apple Accounts”

Add your Apple Account. All account data is stored securely in iCloud Keychain.

After signing in and completing two-factor authentication, Pastel will automatically detect the region associated with the Apple Account and complete the login process.

This solves several common problems found in existing IPA download tools, such as two-factor authentication failing to trigger and saved account data frequently being lost.

Pastel uses GSA technology to trigger two-factor authentication, making the process more stable and secure.

<img width="556" height="301" alt="image" src="https://github.com/user-attachments/assets/c9efab09-2c9e-4593-908a-f01845b88465" />

# Multiple Version Sources

Pastel combines version ID information from the Timbrd, Agsy, and Bilin download sources, making it easier to quickly locate the required version ID.

You can also retrieve version information directly from Apple. Click “Apple,” and Pastel will use your Apple Account to obtain and display the available version IDs for that app.

If the Apple Account has never acquired the app before, Pastel will automatically acquire it first, except for paid apps.

You may also manually enter a known app version ID and download that specific version.

<img width="460" height="90" alt="image" src="https://github.com/user-attachments/assets/4de67361-8727-4705-8718-f9be81bc7b01" />

# Acknowledgements

This project references some of the code and techniques used by ipatool.ts:

[https://github.com/beer-psi/ipatool.ts](https://github.com/beer-psi/ipatool.ts)

The login process relies on SideStore’s GSA implementation.

Multilingual translations were produced with Claude.

# Building From Source

After cloning the repository for the first time, install the Node.js dependencies:

```bash
cd NodeProject
npm install
```

Then open `Pastel.xcodeproj` in Xcode and build and run the project.
