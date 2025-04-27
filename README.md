# 🧠 Epics & User Stories for **Places**

## 👤 Identitas
>- **Nama:** Andreandhiki Riyanta Putra
>- **NIM:** 23/517511/PA/22191
>- **Kelas:** WRPL KOM A
>- **Dosen Pengampu:** Guntur Budi Herwanto, S.Kom., M.Cs.

---

## 🌍 Initiative: Places – Interactive Maps for Exploring UGM
> **Description:**  
> **Places** is an interactive map platform designed to help UGM students explore the campus and surrounding areas. Users can discover, bookmark, and check the status of key locations such as study spots, discussion rooms, food places, and more — whether for personal use or public sharing.

---

## 🎯 Objectives
- Help new and current students explore areas around the UGM campus more easily.
- Build a stronger sense of community by sharing recommended places.
- Allow users to save personal favorite spots privately.
- Provide helpful information about important and interesting places near campus.
- Encourage community participation through student-to-student place recommendations.

---

## 🧠 Features
- View opening and closing hours.
- Open locations in Google Maps.
- 3D interactive UI (using Mapbox).
- Show if a place is currently crowded.
- Allow anonymous comments or place suggestions (with content filtering).

---

## 🛠️ Tech Stack

| Frontend               | Backend                | Other                        |
|-------------------------|-------------------------|-------------------------------|
| Next.js / React         | Node.js / Express        | Mapbox (3D maps)              |
| Tailwind CSS            | REST API                | Google Maps Redirect          |
| Zustand or Context API  | MongoDB / PostgreSQL    | Bad-words filtering for comments |

---


# 🚩 Epic 1 – Display Available Spots on the Map
*Focus: Show pre-defined spots on an interactive map, complete with key information.*

### ✅ US-1: View available spots on the map
**As a student**, I want to see available spots on an interactive map so I can explore interesting places around UGM.
- [ ] Display all spots as markers on the map.
- [ ] Fetch spot data from a database or API.
- [ ] Use icons or color codes based on categories.

### ✅ US-2: View opening and closing hours
**As a student**, I want to know the opening and closing times of each spot so I can plan my visits better.
- [ ] Add open/close information to each spot.
- [ ] Display hours in the spot’s detail popup.
- [ ] Highlight spots that are currently open.

### ✅ US-3: View detailed spot information
**As a student**, I want to click on a spot to see detailed information, including its description, image, and category.
- [ ] Implement a detail modal or side drawer.
- [ ] Display description, photo, and category tags.
- [ ] Optional: Add a "visited" or "favorite" toggle inside the modal.

---

# 🚩 Epic 2 – Personalization & Filtering
*Focus: Help users customize their experience and find places more easily.*

### ✅ US-4: Filter spots by category
**As a student**, I want to filter spots by categories like "Study", "Eat", or "Discussion" to find what I need faster.
- [ ] Add category tags or dropdown filters.
- [ ] Display only the spots that match selected categories.
- [ ] Optional: Allow multiple category selections.

### ✅ US-5: View spots in a list view
**As a student**, I want to see all spots in a list format so I can explore without relying solely on the map.
- [ ] Add a toggle to switch between map and list views.
- [ ] Create a clean, scrollable list with category badges.
- [ ] Enable sorting by name or category.

---

# 🚩 Epic 3 – Community Interaction & Contributions
*Focus: Allow users to anonymously suggest and interact with places, safely and easily.*

### ✅ US-6: Suggest new spots anonymously
**As an anonymous user**, I want to suggest a new spot that hasn’t been added yet.
- [ ] Create a "Suggest a Spot" form (name, category, location, note).
- [ ] Validate and sanitize inputs.
- [ ] Queue suggestions for moderation.

### ✅ US-7: Filter inappropriate comments
**As the system**, I want to automatically filter inappropriate or harmful comments to keep the community safe.
- [ ] Implement a basic bad-word filter (regex or word list).
- [ ] Auto-hide flagged comments and display a warning message.
- [ ] Optional: Allow manual moderation for complex cases.

### ✅ US-8: Indicate spot crowdedness
**As a user**, I want to know if a spot is currently crowded before I go.
- [ ] Let users vote "Full" or "Not Full" anonymously.
- [ ] Show recent crowd status based on user votes.
- [ ] Optional: Votes expire after a few hours to keep info fresh.

---
