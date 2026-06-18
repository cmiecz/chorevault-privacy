---
layout: default
title: ChoreVault Privacy Policy
---

# ChoreVault Privacy Policy

**Effective date:** June 18, 2026
**Last updated:** June 18, 2026

ChoreVault is a family chore and allowance app. This policy explains what we collect, why we collect it, who we share it with, and how you can delete it.

## Who this policy is for

ChoreVault is used by parents/guardians and by children whose parents have added them to a family on the app. Parents create accounts; children sign in to their parent's family with a 4-digit PIN their parent sets.

## What we collect

**From parents:**
- Email address and password (used to sign in)
- Display name
- The name you give your family

**From or about each child a parent adds:**
- Display name
- Birth year (optional, used only to age-appropriately tailor the experience)
- 4-digit PIN (stored as a salted hash; we never store the PIN in clear text)
- Avatar image (optional)
- Records of chores assigned, completed, approved, or rejected
- Photos a child submits for a chore that requires photo verification
- Sunshine Bucks earned, spent, saved, and given
- Savings goals the child creates
- Purchase requests the child makes from the family's Reward Vault

**From every device that signs in:**
- An anonymous APNs (Apple Push Notification Service) device token, used solely to send notifications about chore submissions, approvals, and purchase activity

We do **not** collect: location, contacts, microphone audio, advertising identifiers, browsing history, or any third-party analytics about you.

## Why we collect it

| Data | Purpose |
|---|---|
| Email + password | Authentication for parents |
| PIN (hashed) | Authentication for children |
| Display names | Showing whose chore is whose |
| Chore + completion records | Running the chore + allowance flow |
| Photos | Letting a parent (or our AI verifier) confirm a chore was done |
| Wallet records | Tracking earned and spent Sunshine Bucks |
| APNs token | Sending push notifications about family activity |

## Where the data lives

All data is stored on **Supabase**, a managed Postgres + Storage platform, in US data centers. Access is gated by row-level security policies — each family can only read and write its own data. Photos are stored in a private storage bucket.

## Who we share it with

We share data with three categories of service providers, all to make ChoreVault work:

1. **Supabase** (database, file storage, authentication) — stores all the data described above.
2. **Anthropic** — when a child submits a photo for an AI-verified chore, the child's submitted photo and one or more reference photos set by the parent are sent to Anthropic's Claude API to be scored. Per Anthropic's API terms, this content is **not used for training models** and is **not retained beyond the time required to process the request**. We never send personally identifying information along with the photos.
3. **Apple** — APNs device tokens are sent to Apple's push notification service to deliver alerts.

We do **not** sell or rent your or your child's information to anyone. We do **not** show ads.

## Children's privacy (COPPA)

ChoreVault is designed for family use and may be used by children under the age of 13. We follow the U.S. Children's Online Privacy Protection Act ("COPPA").

- A child can only have a profile in ChoreVault if a parent or guardian creates that profile from a signed-in parent account. Creation of the parent account, which requires a verified email address, serves as **verifiable parental consent** for the child profile(s) the parent then creates.
- A parent can review, edit, or delete their child's profile at any time from the **Family** tab.
- A parent can reset their child's wallet history, chore history, or both from **Settings → Reset a kid**.
- A parent can ask us to delete the entire family — every profile, all photos, all records — by emailing the contact below.
- We collect from children only the minimum needed to operate the family economy: display name, PIN (hashed), optional birth year, optional avatar, and the chore-related records they generate while using the app.
- We never ask children to disclose more than is needed to participate, and we don't condition participation on disclosing more.
- We don't share children's personal information with third parties except as described in the "Who we share it with" section above, which is limited to running the service.

## Photo retention

Photos a child submits for chore verification are retained on the parent's chosen schedule (default: 7 days), set in **Settings → Photo retention**. After that window the photo file is automatically deleted from storage. The parent can also delete every submitted photo immediately from **Settings → Delete all submitted photos**.

Reference photos parents add to a chore stay until the parent removes them or deletes the chore.

## Push notifications

Push notifications are off by default. A parent can turn them on or off in **Settings → Notifications**, or anytime in iOS **Settings → ChoreVault → Notifications**.

## How to delete your data

- **Reset a child's wallet or chore history:** Settings → Reset a kid (in the app).
- **Delete a child profile:** Family tab → swipe on the kid.
- **Delete a chore and all its photos:** Chores tab → swipe-delete the chore.
- **Delete the entire family account and every record we have:** email us at the address below and we'll erase it within 30 days.

## Changes to this policy

If we change this policy in a way that materially affects what we collect or how we use it, we'll update the "Last updated" date above and post the new version at this URL. If you want to see the previous text, the file's full history is in the [GitHub repo](https://github.com/cmiecz/chorevault-privacy).

## Contact

Questions, requests, or data-deletion requests:
**cass.miecz@gmail.com**
