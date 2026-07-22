# Daniel Reyes

Android engineer working in Kotlin and Jetpack Compose. I'm drawn to the parts of an app that are easy to get subtly wrong — data correctness, sync behavior, and architecture that holds up as an app grows.

**Currently:** looking for my first full-time Android role. Open to relocation.

---

### Tracker for Minifigures Series

An offline-first Android app for browsing and tracking LEGO® Collectible Minifigures. Shipped on Google Play, now open-sourced.

The interesting problems weren't in the UI — they were in keeping local and remote state consistent:

- **Incremental sync** against a persisted last-fetched timestamp, so the client pulls only what changed
- **Single-transaction upserts** using partial entity models, updating server-owned catalog data while preserving user state like collected, favorited, and wishlisted
- **SQLite triggers** enforcing invariants at the schema level, so the rules hold no matter which code path writes
- **Migration tests** with Room's `MigrationTestHelper`, verifying data survives every schema version

Kotlin · Jetpack Compose · Room · Coroutines & Flow · Hilt · WorkManager · Retrofit · Material 3

→ [TrackerForMinifiguresSeriesPublic](https://github.com/danielcoderman/TrackerForMinifiguresSeriesPublic)

### Series & Minifigure Catalog REST API

The backend the app talked to — which meant designing the sync contract from both sides. Normalized PostgreSQL schema with database-level triggers, per-IP rate limiting, and a transactional seeder with rollback support.

Node.js · Express · PostgreSQL · Sequelize

→ [SeriesMinifigCatalogRestApiPublic](https://github.com/danielcoderman/SeriesMinifigCatalogRestApiPublic)

---

### Reach me

[LinkedIn](https://linkedin.com/in/danielreyesp)
