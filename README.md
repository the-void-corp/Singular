# SINGULAR

### Messenger for Everyone!

#### (Now in Pre-Alpha)

## Manifest

The modern internet is divided by a false compromise. Users are forced to choose. On one side — privacy from commercial giants; on the other — comfort for gamers and regular users.

**Singular breaks this compromise.**

We are collapsing the best mechanics from the leaders of internet chatting into one app.

## Features

This messenger will have:

- **Direct Messages** with E2E encryption, which gives you full privacy and protection from malicious actors.
- **Groups** which let you speak with your friends or partners using text or voice.
- **Spheres** — massive spaces for many people who want to find a friend or just talk in a group of other people. Spheres can be both public and private.
- Spheres will have voice chats and text chats inside them.

## Security & Moderation

The messenger will have strong moderation to filter harmful content.

We cannot just look into your private chats and ban hostile people. Instead, we have the **Application Board**, which contains all reports about Spheres or users. Our moderators — **Wardens** — can take one report from the board.

If it is a public Sphere, the Warden can examine the reported messages to see what is going on, and then issue a formal verdict by creating an obligatory cryptographic **Distortion Log**. If it is a private Sphere or a DM, the Warden will only look at the provided proof and give an answer. If a Junior Warden makes a mistake, you can file an appeal; a free Senior Warden will review it and deliver a judgment.

### The Rules of the Board:

- **Zero AI Censorship:** Every report is reviewed by a live human Warden who understands context and dark humor. No automated bans for text triggers.
- **Strict Evidence Requirement:** A Warden can only issue a ban if the report contains direct, unalterable evidence. No evidence — no ban.
- **Accountability:** Every action taken by a Warden is logged for 1 year to protect Void Corporation from legal liability and prevent moderator abuse. Users always have the right to appeal a verdict to a Senior Warden.

## Tech Stack

- **Server:** Rust, built on `tokio` for async networking.
- **Client:** Rust with **Tauri** for a lightweight cross-platform desktop app.
- **Transport:** WebSocket connections carrying binary **Protobuf** messages.
- **Philosophy:** KISS and Unix — small, focused components over monolithic code.

## Development Roadmap

- **Pre-Alpha (Current State):** Basic message relay between two hardcoded test accounts over WebSocket. No encryption, no accounts system, no advanced features yet. No compiled application is available yet.
- **Alpha:** Will introduce encryption, real authentication (logins & keys), and some other core features. Testing is conducted strictly among the developer's close associates. No public application is available yet.
- **Beta (Final Testing Stage):** Will include all planned user-facing features — Groups, Spheres, and more. This stage is dedicated to bug testing and the occasional addition of small improvements. Compiled applications will be available for Windows, macOS, and most Linux distributions.
- **Release:** All bugs fixed, all features fully implemented, third-party libraries progressively replaced with in-house alternatives. Applications will be available on all previously supported desktop platforms, as well as Android and iOS.
