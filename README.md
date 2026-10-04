# Home WiFi Manager
Kotlin + Jetpack Compose + Room. Offline-first. Open this folder in Android Studio (Koala or newer), let Gradle sync, press Run.

Notes
- Payment rows are unique per member+month+year; "Undo" flips status, rows are never deleted. Removing a member = INACTIVE (archived).
- Backup = JSON (WiFiManager_Backup_YYYY-MM-DD.json) via the Android save dialog (phone storage / Drive / any cloud app).
- Auto backup writes to the app's own folder (last 10). Reminder = WorkManager, checked twice a day, works offline.
- Settings > "Load sample data" creates W001–W005 with payment history for testing.
