# Vedic Lifestyle Digital Well-being Companion
**Platform:** Android (Jetpack Compose)  
**Backend:** Spring Boot  
**Image Storage:** Cloudinary

## High-Level Architecture

- **Frontend:** Jetpack Compose UI, Kotlin coroutines, Navigation Compose.
- **Backend:** Spring Boot REST APIs, JWT Auth, Challenge/Leaderboard logic, User profile management.
- **Cloudinary:** Store user-uploaded images (challenge proofs, avatars, badges).

---

## 1. Authentication Flow

### Screens
- **Splash Screen:** Logo, animated intro.
- **Sign In / Sign Up:** Email, Google, Apple options. Vedic-themed background.
- **Onboarding:**  
  - Welcome message.
  - Ask for favorite apps (list + icons).
  - Ask for self-set daily limits (slider/input per app).
  - Suggest healthier limits if too high ("How about trying 4 hrs instead of 5?").
  - Set motivational preferences (quotes, health tips).

---

## 2. Home Dashboard

### Screens
- **Main Dashboard:**
  - Greeting (“Namaste [Name], here’s your Vedic wisdom for today”).
  - Animated motivational quote.
  - Daily health fact (dynamic, personalized).
  - Challenge of the Day (“Try reading 15 min before bed!”).

- **Quick Stats Bar:**
  - Today’s screen time.
  - App limit progress.
  - “Mind Balance Meter” (visual scale).

- **Wisdom Chest Button:**
  - Opens mystery reward (quote, small bonus, mini-challenge).

---

## 3. Vedic Health Insights

### Screens
- **Vedic Health Insights Dashboard:**
  - Infographics: Health risks (eye strain, anxiety, insomnia).
  - Animated charts comparing Pre-Digital Era vs Today (Cloudinary images or Compose charts).
  - “Positive change” meter showing improvements as usage drops.

- **Journey Map Screen:**
  - Users see their “Vedic Journey” progress (Brahmacharya → Moksha).
  - Unlock artifacts (quotes, symbols, music) as they move forward.

---

## 4. Smart App Usage & Review

### Screens
- **App Usage Limits:**
  - List of favorite apps.
  - Customizable daily limits.
  - Negotiation prompts if over limits (“Reduce by 1 hour = 7 hours extra per week!”).

- **Weekly Review Screen:**
  - Compare actual vs set limits.
  - Suggestions for improvement.
  - Celebratory animations for progress.

---

## 5. Social Detox Challenges

### Screens
- **Challenges Hub:**
  - List public challenge rooms (7-day, 21-day, weekend).
  - Join or create custom challenge.

- **Challenge Detail:**
  - Description, rules, participants.
  - Daily screen time screenshot post (Cloudinary upload).
  - Like & motivational comments.

- **Friend Challenge:**
  - Invite friends to “3-hour no-phone” group.
  - All lose points if one fails; shared leaderboard.

- **Global Leaderboard:**
  - Weekly refresh.
  - Top profiles, badges, medals.
  - Filter by friends, location, challenge type.

---

## 6. Reward System & Profile

### Screens
- **Profile Screen:**
  - Avatar, theme, badge showcase.
  - Stats: Points, completed challenges, streaks.
  - Unlockables (themes, badges, artifacts).

- **Badges & Medals:**
  - Earned for milestones (challenge wins, streaks, inspiring others).
  - Premium: Custom badge creator.

---

## 7. Gamified Mini-Features

### Screens/Widgets
- **Wisdom Chest:**  
  - Daily “open chest” reward if under limit.

- **Focus Streak Meter:**  
  - Shows consecutive days of success, increases reward multiplier.

- **Mind Balance Meter:**  
  - Animated scale; more phone = digital side heavier, more offline = wellness side heavier.

---

## 8. App Blocker/Timer System

### Screens
- **Allowed Apps Picker:**  
  - User selects what to block, set custom rules (premium).

- **Timer Widget:**  
  - Floating timer on blocked apps, gentle reminders.

- **App Blocker Screen:**  
  - Configure schedules, emergency access, etc.

---

## 9. Notification System

- Motivational push (quotes, health facts).
- “Challenge reminder” notifications.
- “Streak achieved!” celebratory push.

---

## 10. Settings & Support

- Privacy settings.
- Data export.
- Support/FAQ (Vedic health, digital detox guidance).
- Feedback form.

---

## Backend APIs (Spring Boot)
- Auth: Register, login, JWT validation.
- User: Profile, preferences, streaks, points.
- App Usage: Log, review, negotiate limits.
- Challenges: Create/join, progress, leaderboard.
- Rewards: Badges, medals, chest.
- Artifacts: Vedic quotes, music, symbols.
- Cloudinary integration: Upload, fetch images.
- Notification: Push tokens, reminders.

---

## Implementation Notes

- **Jetpack Compose:** Use Material3, custom Vedic color palette, animated transitions.
- **Spring Boot:** Use JPA/Hibernate for DB, schedule weekly leaderboard resets, integrate Cloudinary SDK.
- **Cloudinary:** Store images for posts, avatars, artifacts, badge designs.

---

## Extra Feature Ideas

- **Offline Activities Recommendations:** Suggest Vedic lifestyle tasks (meditation, reading, yoga).
- **Wellness Journal:** Let users log feelings, track mood over time.
- **Group Chat:** Support for challenge rooms.
- **Seasonal Events:** Special Vedic festivals with themed challenges and rewards.

---

## Gamified Alternatives to "Forest"
- **Journey Map Progress:** Instead of planting, progress through a Vedic journey/stages.
- **Unlock Ancient Artifacts:** Earn points to unlock and display rare Vedic symbols/music in profile.
- **Balance Scale Visualization:** Show overall mind balance as users succeed in digital detox.

---

### Your Next Steps

1. **Wireframe all screens (Figma/Whimsical).**
2. **Set up Jetpack Compose navigation & theme.**
3. **Build backend API contracts (OpenAPI spec).**
4. **Integrate Cloudinary image handling.**
5. **Plan out leaderboard and reward logic.**
6. **Draft motivational quote/health fact database.**
7. **Design challenge and group participation logic.**

---

Let me know if you want a breakdown of any specific screen, API contract, or UI/UX flows!
