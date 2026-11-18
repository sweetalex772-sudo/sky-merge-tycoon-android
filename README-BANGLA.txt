SKY MERGE TYCOON — ANDROID APK PROJECT

এই প্রজেক্টটি তোমার বর্তমান Netlify গেম URL-কে Android WebView-এর মধ্যে চালায়:
https://thunderous-begonia-cf70d2.netlify.app/

গুরুত্বপূর্ণ:
- এটি APK-এর Android Studio/Gradle source project; APK এখনো build বা device-এ test করা হয়নি।
- Adsterra script ওয়েবসাইটে লোড হলেও Android WebView-তে সব ad format কাজ করবে—এ নিশ্চয়তা নেই। Popunder/new-window behavior বিশেষ করে পরীক্ষা করতে হবে।
- এই workflow GitHub Actions দিয়ে unsigned/debug APK তৈরি করবে। Play Store-এর জন্য আলাদা signed release build ও Play policy review দরকার।

Chromebook/Browser দিয়ে APK বানানোর ধাপ:
1. ZIP extract করো।
2. GitHub-এ নতুন repository তৈরি করো (যেমন sky-merge-tycoon-android)।
3. Extract করা project-এর ভেতরের সব ফাইল repository-তে upload করো; ZIP-টিকে একা upload করলে হবে না।
4. Commit changes করো।
5. GitHub repository-তে Actions tab খোলো।
6. "Build Sky Merge Tycoon APK" workflow নির্বাচন করে Run workflow চাপো।
7. Build শেষ হলে নিচে Artifacts থেকে sky-merge-tycoon-debug-apk ডাউনলোড করো।
8. ZIP artifact extract করে app-debug.apk Android ফোনে পাঠিয়ে install করে পরীক্ষা করো।

যদি GitHub Actions build fail করে, Actions-এর error screenshot পাঠাও।
