<!-- auto-generated, do not hand-edit -->
# Campus Champions Notifications

This page catalogs all automated notifications for the Campus Champions portal.

## Summary Table

| Name | Trigger | Method | Subject | Recipient | Needs Review |
|------|---------|--------|---------|-----------|:------------:|
| Allocation Import Error | allocations cron import error | email | Errors during allocations import | Site admin | — |
| Constant Contact Error | Constant Contact API error | email | Constant Contact problem/error | Site admin | — |
| Simplelists Error | Simplelists integration error | email | Simplelists problem | Site admin | — |
| Appverse Review Requested | content moderation transition (send_for_review) | email | New Appverse App submitted | Appverse PM | — |
| ACCESS Weekly Digest | weekly cron via access_news | constant-contact | The ACCESS Digest // [date] | Affinity group members | ⚠️ |

## Notification Details

### Allocation Import Error

| Field | Value |
|-------|-------|
| **Portal(s)** | campus-champions |
| **Trigger** | Error occurs during the allocations users cron import |
| **Send Method** | email |
| **Timing** | immediate |
| **Recipient** | Site administrator |
| **Recipient Role** | site admin |
| **Subject** | `Errors during allocations import` |
| **Body Summary** | Reports errors that occurred during the allocations import process; body contains the error detail passed as `{{ body }}`. |
| **Edit Location** | `web/sites/default/config/default/symfony_mailer.mailer_policy.affinitygroup.allocation_error.yml` |

---

### Constant Contact Error

| Field | Value |
|-------|-------|
| **Portal(s)** | campus-champions |
| **Trigger** | Constant Contact API call fails |
| **Send Method** | email |
| **Timing** | immediate |
| **Recipient** | Site administrator |
| **Recipient Role** | site admin |
| **Subject** | `Constant Contact problem/error` |
| **Body Summary** | Notifies admin of a Constant Contact API problem or error; body contains the error message passed as `{{ message }}`. |
| **Edit Location** | `web/sites/default/config/default/symfony_mailer.mailer_policy.affinitygroup.cc_error.yml` |

---

### Simplelists Error

| Field | Value |
|-------|-------|
| **Portal(s)** | campus-champions |
| **Trigger** | Simplelists email list integration error |
| **Send Method** | email |
| **Timing** | immediate |
| **Recipient** | Site administrator |
| **Recipient Role** | site admin |
| **Subject** | `Simplelists problem` |
| **Body Summary** | Notifies admin of a problem with the Simplelists integration; body contains the error message passed as `{{ errmsg }}`. |
| **Edit Location** | `web/sites/default/config/default/symfony_mailer.mailer_policy.affinitygroup.simplelist_error.yml` |

---

### Appverse Review Requested

| Field | Value |
|-------|-------|
| **Portal(s)** | campus-champions |
| **Trigger** | Content moderation transition: `send_for_review` in `appverse_editorial` workflow |
| **Send Method** | email |
| **Timing** | immediate |
| **Recipient** | Appverse PM |
| **Recipient Role** | appverse_pm |
| **Subject** | `New Appverse App submitted` |
| **Body Summary** | Notifies the Appverse PM that a new Appverse app has been submitted for review, with a link to the app node. |
| **Edit Location** | `web/sites/default/config/default/content_moderation_notifications.content_moderation_notification.appverse_review_requested.yml` |

---

### ACCESS Weekly Digest

> ⚠️ **Needs manual verification** — extracted via regex scan.

| Field | Value |
|-------|-------|
| **Portal(s)** | campus-champions |
| **Trigger** | Weekly cron (manual trigger also available via admin form) |
| **Send Method** | constant-contact |
| **Timing** | cron (weekly) |
| **Recipient** | Affinity group members (subscribed CC contact lists) |
| **Recipient Role** | any (affinity group member) |
| **Subject** | `The ACCESS Digest // [date]` |
| **Body Summary** | Compiles and sends a weekly digest of ACCESS announcements (last 14 days) and upcoming events (next 30 days) to affinity group Constant Contact lists via `sendEmailCampaign()`; HTML built by `EmailWrapper`. |
| **Edit Location** | `web/modules/custom/access/modules/access_news/access_news.module` (function `weeklyNewsReport`) |
| **is_shared** | true (also touches access-support news content) |
