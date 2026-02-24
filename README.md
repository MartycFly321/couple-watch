# CoupleWatch

**A shared moment tracker for couples, built around a beautiful 24-hour clock.**

CoupleWatch lets you and your partner track moods, share moments, and stay connected throughout the day — all visualized on a dual-ring clock that tells the story of your shared time.

---

## What is CoupleWatch?

CoupleWatch is a native iOS app that gives couples a private, visual way to stay emotionally connected. At its core is a 24-hour dual-ring clock — the outer ring represents your partner, the inner ring represents you. Moments appear as emoji markers at the time they happened, and moods shift the colors of the rings in real time.

No social feeds. No accounts. No servers. Just you, your partner, and a shared clock synced through iCloud.

---

## Features

### Dual-Ring Clock
A 24-hour clock where the outer ring shows your partner and the inner ring shows you. Emoji markers appear at the exact time moments were shared, creating a visual timeline of your day together.

### Mood Tracking
Set your mood by dragging on a 2D grid — happiness on one axis, energy on the other. Four natural zones emerge: excited, calm, tired, and stressed. Your partner sees your mood instantly, reflected in the ring colors.

### Shared Moments
Send emoji-based moments with a single tap. Use quick-access emojis, pick from the full emoji set, or send a love poke with the heart button. Every moment lands on the clock at the time it was created.

### Partner Notifications
Get notified when your partner shares a mood or creates a moment. Love pokes arrive with dedicated romantic messages.

### Home Screen Widget
A full-featured widget mirrors the clock on your home screen — dual rings, mood colors, emoji markers, and quick actions to set your mood or send moments without opening the app.

### Customization
Pick your own ring color, your partner's ring color, and a background color that dynamically generates the mood palette. Optionally set a photo as the clock center. Floating heart animations add warmth.

---

## How It Works

1. One partner creates an invite from Settings
2. Share the link via Messages, AirDrop, email — any share method
3. The other partner taps the link to accept
4. Both devices sync automatically via iCloud

That's it. No sign-ups, no passwords, no third-party servers.

---

## Privacy

CoupleWatch is built entirely on Apple's iCloud infrastructure. All data syncs privately between you and your partner through CloudKit. There are no external servers, no analytics, and no data collection. Your moments and moods stay between the two of you.

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| UI | SwiftUI |
| State | @Observable (Observation framework) |
| Persistence | Core Data |
| Sync | CloudKit (CKSyncEngine, dual-engine) |
| Widget | WidgetKit + App Intents |
| Notifications | Local notifications |
| Sharing | CKShare (zone-wide) |

**Requires iOS 17+**

---

## Project Structure

```
CoupleWatch/
├── Models/              # Core Data entity definitions
├── Services/            # CloudKit sync, sharing, notifications, haptics
├── Storage/             # Repositories and user management
├── ViewModels/          # View models for Home and event creation
├── Views/
│   ├── HomeView/        # Main clock, mood picker, moment creator
│   ├── EventHistoryView/# Chronological timeline of shared moments
│   └── SettingsView/    # Partner connection, colors, widget setup
├── Shared/              # App Intents and shared utilities
└── Couple​Watch​Widget/   # Home screen widget
```

---

## Contact

Built by [Martijn van Veen](https://github.com/martijnvanveen).

For feedback or questions, reach out through the in-app feedback button or open an issue on this repository.

---

*Built with SwiftUI, Core Data, CloudKit, and WidgetKit.*
