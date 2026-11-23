# ZEEFROSH test build

This branch is separate from main. The website uses Firebase Email/Password authentication and Firestore. Simulated mining points are local browser demo values only and are not cash, gold, or cryptocurrency. Demo withdrawal records do not send money.

## Setup
1. Enable Email/Password in Firebase Authentication.
2. Publish firestore.rules in Firebase Console > Firestore Database > Rules.
3. Create your admin login using the site's Register button, then sign in once.
4. In Firebase Console > Authentication, copy your admin account UID.
5. In Firestore, create collection admin_users and a document whose ID is that UID. Add boolean field active = true. Do not expose write access to this collection.
6. Create a second login for your friend. That account must not be added to admin_users.

## Not enabled yet
Proof image upload is disabled until a secure private upload endpoint is available. Firebase Storage requires a plan change; Cloudinary API secrets must never be placed in frontend code. Referral link is display-only. No real rewards or withdrawals are processed.
