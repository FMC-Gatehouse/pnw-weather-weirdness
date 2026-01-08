PNW Weather Weirdness - Game Design Document
Core Concept
A gamified weather app that turns daily weather checking into a collection game. Users log weather conditions to unlock regional cryptids, phenomena, and achievements while building a community of weather spotters across the Pacific Northwest (and eventually the West Coast).
Unique Value Proposition
Not another boring weather app - it's a collection game that happens to involve weather
Hyper-regional personality - embraces PNW weirdness and culture
Community-driven - user sightings create FOMO and engagement
Shareable moments - unlock graphics designed for social media

Core Gameplay Loop
Daily Check-in - User opens app, confirms/logs current weather conditions
Progress tracking - Streaks, patterns, and conditions contribute to unlocks
Unlock rewards - Stickers, cryptids, achievements, phenomena
Community feed - See what others have spotted nearby
Share wins - Post rare unlocks to social media
Return tomorrow - New weather = new opportunities

Key Features - Phase 1 (MVP)
Weather Logging
Simple daily check-in: "What's it like outside?"
Quick-select common conditions (rainy, cloudy, sunny, foggy, etc.)
Optional: Temperature, "vibe" tags (cozy, gloomy, crisp)
Bonus: Photo upload of the sky/conditions
Collection System
Stickers: Collectible weather phenomena
Common: Rain drops, clouds, sun breaks
Uncommon: Rainbows, fog banks, wind
Rare: Sun dogs, atmospheric rivers, "the mountain is out"
Legendary: Double rainbows, Sasquatch sightings, perfect days
Cryptids & Characters
Sasquatch (appears in fog after X days)
Orcas (rainy day streaks)
Banana slugs (consistent drizzle)
More regional creatures as you expand
Achievements
"Touched Grass 7 Days Straight"
"Rain for 30 Days"
"The Mountain Is Out" (logged clear day with mountain visibility)
"Survived June-uary"
"Microclimates" (4 different conditions in one day via location)
"Sun Break Champion" (logged 10 sun breaks)
Community Feed
Local sightings map: "User spotted a sun dog 2 miles away!"
Recent unlocks in your area
Optional: React/comment on sightings
Privacy: Location shown as general area, not exact
Profile & Progress
Personal collection gallery
Stats: Days logged, streak count, rarest finds
Badges displayed
Shareable profile card

Monetization Strategy
Free Tier
Full core experience
Daily check-ins and logging
Standard sticker collection
Community feed access
Basic achievements
Premium ($2.99/month or $19.99/year)
Exclusive legendary cryptids
Custom weather journal notes
Advanced stats and graphs
Early access to new regions
Ad-free experience
Premium profile customization
"Weather historian" - access to your full log history with visualizations
One-time Purchases
Regional expansion packs ($1.99 each) - NorCal, SoCal, Desert Southwest
Special event collections (seasonal packs)

Technical Stack (Flutter)
Core Tech
Flutter - Cross-platform (iOS/Android to start)
Weather API - OpenWeatherMap or WeatherAPI.com (free tier for MVP)
Backend - Firebase
Authentication (email, Google, Apple)
Firestore (user data, collections, community posts)
Cloud Storage (user photos)
Cloud Functions (achievement triggers, notifications)
Maps - Google Maps API or Mapbox for community sightings
State Management - Riverpod or Bloc
Local Storage - Shared Preferences or Hive for offline collection viewing
Key Packages
geolocator - Location services
weather - Weather data parsing
cached_network_image - Performance
flutter_local_notifications - Daily check-in reminders
share_plus - Social sharing
image_picker - Photo uploads

User Flow - First Time Experience
Onboarding
"Welcome to PNW Weather Weirdness!"
Explain the collection concept
Request location permission (with clear explanation)
Create account (email or social login)
First Check-in
"What's the weather like right now?"
User selects conditions
First unlock! - Common sticker + encouraging message
Tutorial: "Come back tomorrow to build your streak!"
Home Screen
Current weather display (with personality)
Today's check-in button (prominent)
Collection preview (locked silhouettes = intrigue)
Community feed teaser
Achievement progress

Content Roadmap
Phase 1 - Portland/PNW Launch
30 stickers/phenomena
5 cryptids
20 achievements
Community feed
Basic profile
Phase 2 - Expansion
NorCal region
Social features (friends, challenges)
Weather journal entries
Historical data visualization
Phase 3 - West Coast Complete
SoCal region
Desert Southwest
Seasonal events
User-submitted phenomena (moderated)
Phase 4 - Beyond
Other US regions?
International?
API for other devs?

Marketing & Launch Strategy
Pre-Launch (2-4 weeks)
Build hype on r/Portland, r/PNW
TikTok teasers showing cryptid unlocks
Instagram stories: "Coming soon..."
Beta testing with local friends
Launch Day
Reddit post: "I made a weird weather app for Portland"
Submit to Product Hunt
Press release to local tech blogs (Portland Mercury, Willamette Week)
TikTok launch video
Post-Launch
User-generated content campaign: "Show us your rarest unlock!"
Engagement with community on social
Regular content drops (new stickers, achievements)
Local partnerships? (Coffee shops, outdoor brands)

Success Metrics
Week 1
1,000 downloads
30% daily active users
500 check-ins logged
Month 1
5,000 downloads
40% DAU
10,000+ check-ins
100+ community posts
Month 3
15,000 downloads
5% conversion to premium
Strong retention (7-day: 40%, 30-day: 25%)

Risk Mitigation
Risk: Weather APIs are expensive at scale
Mitigation: Cache aggressively, use free tiers initially, consider user-submitted data
Risk: Community toxicity
Mitigation: Moderation tools from day 1, report system, positive-only interactions
Risk: Low engagement after initial novelty
Mitigation: Regular content updates, seasonal events, social challenges
Risk: App stores reject for "duplicate content"
Mitigation: Emphasize collection/game mechanics in store listing, not weather forecasting

Open Questions to Resolve
Should we allow multiple check-ins per day or just one?
How much location granularity? Neighborhood vs city-wide?
Do achievements unlock stickers, or are they separate?
Should there be trading/gifting between users?
Notification strategy - daily reminders or just special events?

Next Steps:
Wireframe the core screens
Set up Firebase project
Build basic weather API integration
Create first 10 sticker designs
Prototype the check-in flow


