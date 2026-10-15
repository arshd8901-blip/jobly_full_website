JOBLY — WEBSITE PROTOTYPE FOR TEENS AGES 16-18

OPEN THE WEBSITE
1. Extract the zip and open index.html in Chrome (or use a local server such as VS Code Live Server).
2. To turn on sign-in, follow SETUP-GUIDE.txt (Supabase URL + public key needed).

LAYOUT
The site now has separate pages (Home, Find jobs, Summer & seasonal, Resume builder, My applications, Learn, Stay safe, Contact). The top menu switches between them and the browser Back button works.

WHAT'S INCLUDED (all 10 teen-focused features)
1. First-job filter: "No experience", "Training provided" tags and filters.
2. School-friendly schedules: availability grid (Mon-Sun x morning/afternoon/evening), After school / Weekends only / Summer / Part-time / Flexible filters, "Fits your schedule" badges.
3. Clear pay: hourly range on every card, minimum $/hr filter, estimated weekly earnings from your weekly hours, minimum weekly earnings filter.
4. Beginner resume builder: school, volunteering, clubs/sports/projects, skills, languages, certifications; 3 templates; Print / Save as PDF. Stays in the browser.
5. Age-eligible listings: every job shows a minimum age (16+/18+); an "I'm 16/17/18" selector hides jobs you can't take; age-related restrictions shown in job details.
6. First-job learning center: applying with no experience, interview questions, what to wear, first day, paychecks & taxes, workplace rights.
7. Safety: red-flag/scam warnings, "Employer checked" badge (sample), Report-listing button, apply-on-employer-site design.
8. Application tracker: Saved -> Applied -> Interview -> Decision, notes, follow-up reminders, add jobs found elsewhere.
9. Nearby jobs: ZIP/city search + max distance + near-transit filter. Location is used only in the browser. (Demo knows only sample Sacramento-area ZIPs.)
10. Summer & seasonal section: summer/camp jobs and holiday/seasonal retail tabs.

FIXED FROM THE FIRST VERSION
- Password reset now works end to end (recovery link opens a "choose a new password" form).
- All job/tracker/resume text is inserted as plain text (no innerHTML), closing the XSS risk.
- "View details" is now a proper dialog instead of an alert with a stray "\n".
- Supabase library pinned to an exact version (2.45.4) instead of "@2".
- Added a Content-Security-Policy, a privacy & terms draft, and an age/terms checkbox at sign-up (password minimum is now 10 characters).
- Dialogs close with Escape, trap Tab focus, and restore focus.
- Saved jobs, schedule, resume and tracker now persist on the device (localStorage) with an "Erase my data" button.

STILL A PROTOTYPE
Listings, employers and "Employer checked" badges are FICTIONAL SAMPLES. The contact form doesn't send. Data is stored only in the user's browser; nothing is synced to a server yet, and no real database tables exist. Before a public launch: real verified job sources and employer verification, state-by-state child-labor rules review, a lawyer-reviewed privacy policy/terms (minors), Supabase RLS for any private table, HTTPS hosting, SMTP/abuse protection, moderation, and a security review. Check the Jobly name/domain/trademark.
