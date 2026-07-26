# Varq — Sahi Tarike Se APK Banane Ka Poora Process

Pichli baar galti ye hui thi: PWABuilder ko `github.com/sajid199/book.git`
(repo link) diya gaya tha, jo ek **code page** hai, live website nahi. Isliye
APK khulte hi GitHub khul raha tha.

Is ZIP mein 4 files hain:
- `index.html` → tumhara Varq reader (naam already `index.html` hai — badalna mat)
- `manifest.json` → app ka sahi naam "Varq", icon, colors set hain
- `icon-192.png`, `icon-512.png`, `icon-512-maskable.png` → app icons

## Step 1 — GitHub par naya (ya wahi) repo banao
1. github.com par jao → **New repository** → naam do: `varq`
2. "Public" rakho, "Add README" ki zarurat nahi

## Step 2 — Saari 5 files upload karo
1. Repo ke andar **"Add file" → "Upload files"**
2. Is ZIP ki saari 5 files (index.html, manifest.json, 3 icons) ek saath
   drag-drop karo — **folder ke andar mat dabo, seedha root mein daalo**
3. "Commit changes"

Repo ka structure aisa dikhna chahiye:
```
varq/
├── index.html
├── manifest.json
├── icon-192.png
├── icon-512.png
└── icon-512-maskable.png
```

## Step 3 — GitHub Pages ON karo
1. Repo ke **Settings → Pages** (left sidebar mein)
2. "Branch" → `main` select karo, folder `/ (root)`, **Save**
3. 1-2 minute wait karo, refresh karo — upar ek green box mein link milega:
   `https://sajid199.github.io/varq/`

## Step 4 — Check karo ki sahi khula
Us link ko phone ya laptop ke browser mein kholo. **Varq** ka cover screen
(burgundy book icon) dikhna chahiye — GitHub nahi. Agar ye sahi dikh raha hai,
tabhi aage badho.

## Step 5 — PWABuilder mein SAHI link daalo
1. `pwabuilder.com` kholo
2. Is baar ye daalo (bina `.git` ke, bina extra kuch): 
   `https://sajid199.github.io/varq/`
3. "Start" → scan hone do → is baar icon/manifest ke warnings kam honge
   (kyunki humne pehle se manifest.json aur icons set kar diye hain)
4. **"Package For Stores"** → **Android** icon choose karo → "Generate"
5. ZIP download hogi → usme `GitHub.apk` ki jagah ab shayad `Varq.apk` ya
   similar naam se APK milegi

## Step 6 — Phone mein install
1. `.apk` file phone mein transfer karo
2. Tap karo → "Install anyway" / "allow from this source"
3. Ab **Varq** naam aur icon ke saath app khulegi, cover screen sahi dikhega

---
**Agar kahin bhi atko** (Pages link kaam na kare, ya PWABuilder mein error
aaye), screenshot bhej dena — turant fix kar dunga.
