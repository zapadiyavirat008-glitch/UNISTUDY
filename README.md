# UNISTUDY — College Study Guides & Materials (GitHub Pages Ready)

Yeh folder aapke GitHub Pages repository ke liye bilkul ready hai.

## Folder Structure
- `index.html` — Puri website ka main code (har section ke upar `[SECTION ...]` aur `[POINT ...]` ke instructions likhe hain).
- `assets/` — Website ka Eye Logo (`eye_logo.png`), Home Page Study Table image (`hero_study_art.jpg`), 3 Feature images (`feat_1.png`, `feat_2.png`, `feat_3.png`), aur 9 Banner backgrounds (`banner_*.jpg`).
- `pdfs/UNISTUDY_English_Sem6_Major14_Unit1_That_Long_Silence.pdf` — English Sem 6 Major 14 Unit 1 (*That Long Silence*) ki clean, spacious PDF file.

## Kisi Bhi Section Ko Kaise Badlein (Easy Customization Points in `index.html`)
1. **[SECTION 1: THEME COLORS & FONTS]** — Site ke background colors aur fonts badalne ke liye.
2. **[HEADER / TOP NAVIGATION BAR]** — Top bar me `UNISTUDY` name ya logo change karne ke liye.
3. **[PAGE 1: HOME PAGE VIEW]** — Home page ka main title, 4 Subject boxes (`English`, `History`, `Sociology`, `Gujarati`), ya niche ke 3 benefits (`College Studies, Explained Better`) badalne ke liye.
4. **[POINT A: BANNER IMAGES DICTIONARY]** — Kisi bhi page ka top banner change karne ke liye (`BANNERS.blueStudy`, `BANNERS.tealClouds`, `BANNERS.maroonCaps`, `BANNERS.greenBooks`, etc.).
5. **[POINT C: COMPLETE WEBSITE DATA (`SITE_DATA`)]** — Naya Topic / Subject Paper (uske saare Units, Theory pages, Question Bank, aur MCQs ke sath) ek sath add karne ke liye!

### Naya Topic Ek Sath Kaise Paste Karein?
Jab bhi aapko kisi Subject (jaise `english`, `history`, `sociology`, `gujarati`) ke kisi Semester (`sem1` se `sem6`) me naya Topic dalna ho, to `SITE_DATA` me us semester ke `[ ... ]` ke andar niche jaisa block paste kar dein:

```javascript
{
  id: "major-15-new-topic",
  code: "Major - 15",
  title: "Topic Ka Naam Yahan Likhein",
  author: "Author Name (Optional)",
  banner: BANNERS.tealClouds,
  readingBanner: BANNERS.blueClouds,
  units: [
    {
      unitNumber: "Unit - 1",
      unitShortLabel: "Unit 1",
      items: [
        {
          id: "m15-unit1-theory",
          type: "theory", // 'theory' | 'mcq' | 'question'
          unitBadge: "Unit 1",
          majorBadge: "Major - 15",
          title: "Unit 1 Theory Title",
          preview: "Yahan 2 line ka preview likhein jo card par dikhega...",
          pages: [
            {
              pageTitle: "Page 1 Heading",
              htmlContent: `<p>Yahan Page 1 ka pura text aayega...</p>`
            },
            {
              pageTitle: "Page 2 Heading",
              htmlContent: `<p>Agar text lamba hai to Page 2 me aayega...</p>`
            }
          ]
        }
      ]
    }
  ]
}
```
Jaise hi aap yeh block paste karenge, Menu Bar, Semester Page, Unit Filters (`All`, `Theory`, `MCQ`, `Question`), Next/Prev Reading Pages, aur Clean PDF option sab apne-aap set ho jayenge!
