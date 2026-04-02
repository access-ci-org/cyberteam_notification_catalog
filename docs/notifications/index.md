<!-- auto-generated, do not hand-edit -->
# All Notifications — Summary

This index lists every automated notification catalogued across all portals.

| Name | Portal(s) | Trigger | Method | Subject | Needs Review |
|------|-----------|---------|--------|---------|:------------:|
| Needs Adjustment | access-support | content moderation (request_adjustment / editorial) | email | Your [...] needs adjustment | — |
| Published | access-support | content moderation (publish / editorial) | email | Your [...] was published | — |
| Review Requested | access-support | content moderation (send_for_review / editorial) | email | [...] needs review | — |
| Event Registration Confirmation | access-support | user registers for event | email | `{{ email_title }}` | — |
| Registration Approved | access-support | event registration approved | email | `{{ email_title }}` | — |
| Waitlist Notification | access-support | registration waitlisted | email | Waitlist Status for `{{ title }}` | — |
| Registrant Digest | access-support | new event registrations (digest) | email | `{{ registration_count }}` new registration(s) for `{{ event_title }}` | — |
| Post-Event Survey | access-support | post-event trigger | email | Please participate in our survey for `{{ title }}` | — |
| Post-Event Survey Reminder | access-support | reminder cron/follow-up | email | Reminder: please participate in our survey for `{{ title }}` | — |
| Announcement Review | access-support | announcement content created | email | An announcement is ready for review | — |
| Ticketing Form Email | access-support | webform submission (ticketing form) | email | Derived from form data | ⚠️ |
| Account Support Request | access-support | webform submission (account support) | email | account support request from [name] | ⚠️ |
| Request to Add Org | access-support | webform submission (org list add) | email | Request to add an organization from [name] | ⚠️ |
| New CCMNet User (Admin) | ccmnet | new user registration | email | A new CCMNet participant has joined! | — |
| CCMNet Welcome | ccmnet | new user registration | email | Welcome to CCMNet... | — |
| Mentorship Interest (Author) | ccmnet | daily cron | email | Interest in your Mentorship | — |
| Mentorship Interest Digest (Role) | ccmnet | daily cron | email | Daily mentorship interest summary | — |
| Liaison/Mentor/Mentee Match | ccmnet | mentor match made | email | A new mentorship match | — |
| Mentee Selected | ccmnet | mentor/mentee pairing saved | email | You have been selected as a mentee | — |
| Mentor Selected | ccmnet | mentor/mentee pairing saved | email | You have been selected as a mentor | — |
| Mentorship Approved (PM) | ccmnet | mentorship approved | email | Mentorship Engagement approved | — |
| New Mentorship (Admin) | ccmnet | mentorship created | email | New Mentorship Created | — |
| Mentorship Created (Requestor) | ccmnet | mentorship created | email | Mentorship Engagement received | — |
| Mentorship In Progress | ccmnet | mentorship status → in-progress | email | Mentorship in progress | — |
| Allocation Import Error | campus-champions | allocations cron import error | email | Errors during allocations import | — |
| Constant Contact Error | campus-champions | Constant Contact API error | email | Constant Contact problem/error | — |
| Simplelists Error | campus-champions | Simplelists integration error | email | Simplelists problem | — |
| Appverse Review Requested | campus-champions | content moderation (send_for_review / appverse_editorial) | email | New Appverse App submitted | — |
| ACCESS Weekly Digest | campus-champions | weekly cron | constant-contact | The ACCESS Digest // [date] | ⚠️ |
| New Project Submission (Manager) | pascience | project node created | email | New Project Submission: `{{ project_title }}` | — |
| Project Submission Received (Author) | pascience | project node created | email | Project Submission Received: `{{ project_title }}` | — |
| Project Updated (Manager) | pascience | project node updated | email | Project Updated: `{{ project_title }}` | — |
| Project Approved (Author) | pascience | project approved/published | email | Project Approved and Published: `{{ project_title }}` | — |
| Project Interest Flagged | pascience | user flags interest in project | email | `{{ title }}` - interest shown on project | — |
| MATCH Engagement Draft | shared | content moderation (create_new_draft / match_engagement) | email | MATCH Engagement draft created | — |
| MATCH Engagement Received | shared | content moderation (save_as_submitted / match_engagement) | email | Your MATCH Engagement was received | — |
| MATCH Engagement Accepted *(disabled)* | shared | content moderation (start_recruiting / match_engagement) | email | Your MATCH Engagement is ready to recruit! | — |
| MATCH Engagement Review Requested *(disabled)* | shared | content moderation (request_review / match_engagement) | email | MATCH Engagement submitted for review | — |
| MATCH Engagement Final Review *(disabled)* | shared | content moderation (finished_adding_information / match_engagement) | email | MATCH Engagement ready for review | — |

---

## Totals by Source

| Source | Count |
|--------|-------|
| Content Moderation Notifications | 9 |
| Symfony Mailer Policies | 26 |
| EmailBuilder PHP Plugins | 0 new (all covered by Symfony Mailer) |
| Hook-based Emails (`drupal_mail` / `mailManager->mail`) | 0 new (all covered by WebformHandler PHP) |
| Constant Contact Campaigns | 1 |
| Webform YAML Email Handlers | 0 |
| WebformHandler PHP Plugins | 3 |
| **Total** | **39** |

## Totals by Portal

| Portal | Count |
|--------|-------|
| access-support | 13 |
| ccmnet | 11 |
| campus-champions | 5 |
| pascience | 5 |
| shared | 5 |
| open-ondemand | 0 |
| **Total** | **39** |
