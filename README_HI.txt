आवाज़ पहचानो — नन्हे दोस्त
Android Studio प्रोजेक्ट (सोर्स कोड)

विशेषताएँ:
- हिंदी इंटरफ़ेस और बड़े जानवर इमोजी/नाम
- 8 जानवरों के लिए नमूना इलेक्ट्रॉनिक ध्वनि प्रभाव
- हल्का सिंथेसाइज़ किया गया बैकग्राउंड म्यूजिक, जिसे चालू/बंद किया जा सकता है
- ऑफलाइन चलने के लिए कोई इंटरनेट अनुमति नहीं
- नीचे क्रेडिट: App developed by DEEVAKAR DAVE, बाड़मेर

महत्वपूर्ण:
यह Android Studio सोर्स प्रोजेक्ट है, तैयार APK नहीं। इस वातावरण में Android SDK/Gradle उपलब्ध नहीं थे, इसलिए APK बनाकर सत्यापित नहीं किया जा सका। ध्वनियाँ असली जानवरों की रिकॉर्डिंग नहीं, बल्कि डेमो के लिए बनाई गई ध्वनियाँ हैं।

APK बनाने के चरण:
1. कंप्यूटर पर Android Studio स्थापित करें।
2. Android Studio में Open चुनकर इस फोल्डर को खोलें।
3. Gradle sync पूरा होने दें (पहली बार इंटरनेट की जरूरत हो सकती है)।
4. Build > Build Bundle(s) / APK(s) > Build APK(s) चुनें।
5. APK आमतौर पर app/build/outputs/apk/debug/app-debug.apk में मिलेगा।

Google Play Store पर डालने से पहले ऐप को असली डिवाइस पर टेस्ट करें, बेहतर/लाइसेंस-प्राप्त पशु आवाज़ रिकॉर्डिंग जोड़ें, बच्चों की गोपनीयता व Families नीतियों का पालन करें और signed release AAB बनाएँ।
मोबाइल से Cloud Build (GitHub Actions):
इस ZIP में .github/workflows/build-apk.yml शामिल है। यह GitHub Actions में APK बनाने के लिए workflow है।
ध्यान दें: GitHub पर ZIP को सिर्फ एक फ़ाइल की तरह अपलोड करने से build नहीं चलेगा। ZIP को पहले extract करके प्रोजेक्ट की फाइलें/फोल्डर repository में डालने होंगे, और .github/workflows/build-apk.yml का path ज्यों का त्यों रहना चाहिए।
GitHub Actions के लिए public repository में standard hosted runner का उपयोग आम तौर पर मुफ्त है। Public repository बनाने पर source code सार्वजनिक होगा; इसमें कोई निजी जानकारी न डालें।
