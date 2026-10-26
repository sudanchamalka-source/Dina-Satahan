# ICT දින සටහන් – PWA (Firebase Hosting + GitHub)

1. Firebase console එකේ project එකක් හදන්න (Hosting enable).
2. `.firebaserc` සහ `.github/workflows/firebase-hosting.yml` හි `YOUR-FIREBASE-PROJECT-ID` වෙනුවට ඔබේ project id දාන්න.
3. GitHub repo එකකට push කරන්න (branch: main).
4. GitHub → Settings → Secrets → Actions → `FIREBASE_SERVICE_ACCOUNT` එකතු කරන්න
   (Firebase console → Project settings → Service accounts → Generate new private key → JSON සම්පූර්ණයෙන්ම paste).
   නැතිනම් `firebase init hosting:github` දුවන්න – secret එක ස්වයංක්‍රීයව හදයි.
5. push කරන සෑම වාරයකම ස්වයංක්‍රීයව deploy වේ. `https://PROJECT-ID.web.app` ලිපිනය phone එකේ open කර "Add to Home screen".
