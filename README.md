# Khan Enterprise — স্টক ও বিক্রয় ব্যবস্থাপনা

এটি একটি browser-based stock and sales management app.

## GitHub Pages-এ প্রকাশ

1. GitHub-এ একটি নতুন repository তৈরি করুন।
2. এই ফোল্ডারের `index.html` এবং `README.md` repository-র মূল (root) অংশে upload করুন।
3. Repository → **Settings** → **Pages** খুলুন।
4. **Deploy from a branch** নির্বাচন করুন।
5. Branch হিসেবে `main` এবং folder হিসেবে `/ (root)` নির্বাচন করে **Save** চাপুন।
6. কিছুক্ষণ পর GitHub Pages-এর URL-এ অ্যাপটি খুলবে।

## গুরুত্বপূর্ণ: Firebase

এই HTML ফাইলে Firebase project configuration রয়েছে। GitHub Pages শুধু HTML ফাইলটি host করবে; Firebase Authentication ও Firestore আলাদাভাবে Firebase Console-এ সঠিকভাবে configure থাকতে হবে।

- Firebase Authentication-এ প্রয়োজনীয় sign-in method চালু করুন।
- Firebase Authentication → Settings → Authorized domains-এ আপনার GitHub Pages domain যোগ করুন (যেমন `username.github.io`)।
- Firestore Database তৈরি করে নিরাপদ Security Rules দিন।
- Security Rules কখনো সবার জন্য read/write উন্মুক্ত করবেন না।

## ফাইল

- `index.html` — মূল অ্যাপ।
- `README.md` — প্রকাশ ও Firebase সেটআপের নির্দেশনা।

নোট: GitHub-এ upload করলেই Firebase-এর login, database rules বা app-এর সব feature স্বয়ংক্রিয়ভাবে যাচাই/সম্পূর্ণ হয়ে যায় না। প্রকাশের পর login, data save, date history এবং অন্য feature পরীক্ষা করুন।
