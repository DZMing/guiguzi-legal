# Placeholders still to fill

These pages are still drafts. The draft banner stays on purpose. Nothing in the “Suggestions” section is written into the HTML. Do not paste a suggestion into a page until the app actually behaves that way.

Replace each token, including the square brackets. The same token is one value: every place it appears in that language should get the same text. Tokens are highlighted on the page (`span.placeholder`). Words inside the draft banner are instructions, not tokens.

`DZMing/think-the-chinese-way` still returned 404 to this environment. That includes `docs/store/privacy/guiguzi-legal-android-corrections.patch` on PR #3 (commit `4bd8965`), `docs/store/privacy/release-gaps.md`, and `docs/store/privacy/google-data-safety.md`. The Android corrections in the HTML were written from the requested claims because `git am` had no patch to apply. Device free-use records are the 730-day side of the sweep and safety-attempt records are the 35-day side, in that order. Confirm that split against the quota sweep before publication. Other mismatches are at the end.

## Contact email

Value needed: a monitored mailbox controlled by Qayvi LLC. No address is suggested here.

| File | Line | Token |
| --- | --- | --- |
| index.html | 85 | `[联系邮箱]` |
| index.html | 88 | `[聯絡信箱]` |
| index.html | 91 | `[contact email]` |
| index.html | 95 | `[correo de contacto]` |
| privacy/zh-Hans.html | 27 | `[联系邮箱]` |
| privacy/zh-Hans.html | 29 | `[联系邮箱]` |
| privacy/zh-Hans.html | 87 | `[联系邮箱]` |
| privacy/zh-Hans.html | 96 | `[联系邮箱]` |
| privacy/zh-Hans.html | 103 | `[联系邮箱]` |
| privacy/zh-Hans.html | 106 | `[联系邮箱]` |
| privacy/zh-Hant.html | 27 | `[聯絡信箱]` |
| privacy/zh-Hant.html | 29 | `[聯絡信箱]` |
| privacy/zh-Hant.html | 87 | `[聯絡信箱]` |
| privacy/zh-Hant.html | 96 | `[聯絡信箱]` |
| privacy/zh-Hant.html | 103 | `[聯絡信箱]` |
| privacy/zh-Hant.html | 106 | `[聯絡信箱]` |
| privacy/en.html | 27 | `[contact email]` |
| privacy/en.html | 29 | `[contact email]` |
| privacy/en.html | 87 | `[contact email]` |
| privacy/en.html | 96 | `[contact email]` |
| privacy/en.html | 103 | `[contact email]` |
| privacy/en.html | 106 | `[contact email]` |
| privacy/es-419.html | 27 | `[correo de contacto]` |
| privacy/es-419.html | 29 | `[correo de contacto]` |
| privacy/es-419.html | 87 | `[correo de contacto]` |
| privacy/es-419.html | 96 | `[correo de contacto]` |
| privacy/es-419.html | 103 | `[correo de contacto]` |
| privacy/es-419.html | 106 | `[correo de contacto]` |
| delete-account/zh-Hans.html | 68 | `[联系邮箱]` |
| delete-account/zh-Hans.html | 80 | `[联系邮箱]` |
| delete-account/zh-Hant.html | 68 | `[聯絡信箱]` |
| delete-account/zh-Hant.html | 80 | `[聯絡信箱]` |
| delete-account/en.html | 68 | `[contact email]` |
| delete-account/en.html | 80 | `[contact email]` |
| delete-account/es-419.html | 68 | `[correo de contacto]` |
| delete-account/es-419.html | 80 | `[correo de contacto]` |

## Effective date

Value needed: the calendar date this policy is first published with the store release. Do not reuse 2026-10-25. That date stays in the draft banner as the date of the draft.

| File | Line | Token |
| --- | --- | --- |
| privacy/zh-Hans.html | 25 | `[生效日期]` |
| privacy/zh-Hant.html | 25 | `[生效日期]` |
| privacy/en.html | 25 | `[effective date]` |
| privacy/es-419.html | 25 | `[fecha de vigencia]` |

## Retention periods

Three periods below are still blank. Device-quota retention is filled and is not one of them. Do not fill the three blank periods with one shared number.

### Session and request-hash retention

Value needed: how long server-side session, usage, and completed-request hash records are kept when the account is not deleted and the server is not restarted. The 24-hour figure already on the page is only how long the session credential works. It is not this period.

Suggestion only, not inserted: 30 days after the session credential stops working, and delete the records immediately when account deletion is confirmed. Do not insert 30 days while these records exist only in memory and disappear on restart. A durable 30-day copy would be new behavior.

| File | Line | Token |
| --- | --- | --- |
| privacy/zh-Hans.html | 61 | `[会话与请求摘要的保留期限]` |
| privacy/zh-Hant.html | 61 | `[工作階段與請求摘要的保留期限]` |
| privacy/en.html | 61 | `[session and request-hash retention period]` |
| privacy/es-419.html | 61 | `[plazo de conservación de sesiones y resúmenes de solicitudes]` |
| delete-account/zh-Hans.html | 57 | `[会话与请求摘要的保留期限]` |
| delete-account/zh-Hant.html | 57 | `[工作階段與請求摘要的保留期限]` |
| delete-account/en.html | 57 | `[session and request-hash retention period]` |
| delete-account/es-419.html | 57 | `[plazo de conservación de sesiones y resúmenes de solicitudes]` |

### Device-quota retention

Filled. Not a token. A scheduled sweep deletes device free-use records older than 730 days and safety-attempt records older than 35 days. The records can remain after the random account is deleted until the sweep removes them. This release does not create paid daily records. The same sentences are in privacy section 4, the retention table, the accounts-without-sign-in subsection, and the deletion pages. Do not put the old 12-month suggestion back in.

### Logs and third-party retention

Value needed: the retention period for app logs, hosting logs, operating-system logs, and records held by Google Play, the download host, and the model provider. This release does not include RevenueCat, so that name is not in the sentence. Section 8 of each privacy policy uses the same token for InstaBox connection logs. If those periods differ, split the sentences before filling one number into every line.

Suggestion only, not inserted: 30 days for Qayvi’s own request logs (route, status, response size, duration, and error code). Do not invent one number for InstaBox, the operating system, Google Play, Hugging Face, or Alibaba Cloud Bailian. State each provider’s own period, or say the records follow that provider’s policy.

| File | Line | Token |
| --- | --- | --- |
| privacy/zh-Hans.html | 81 | `[日志与第三方记录的保留期限]` |
| privacy/zh-Hans.html | 90 | `[日志与第三方记录的保留期限]` |
| privacy/zh-Hant.html | 81 | `[日誌與第三方紀錄的保留期限]` |
| privacy/zh-Hant.html | 90 | `[日誌與第三方紀錄的保留期限]` |
| privacy/en.html | 81 | `[logs and third-party retention period]` |
| privacy/en.html | 90 | `[logs and third-party retention period]` |
| privacy/es-419.html | 81 | `[plazo de conservación de registros y datos de terceros]` |
| privacy/es-419.html | 90 | `[plazo de conservación de registros y datos de terceros]` |
| delete-account/zh-Hans.html | 62 | `[日志与第三方记录的保留期限]` |
| delete-account/zh-Hant.html | 62 | `[日誌與第三方紀錄的保留期限]` |
| delete-account/en.html | 62 | `[logs and third-party retention period]` |
| delete-account/es-419.html | 62 | `[plazo de conservación de registros y datos de terceros]` |

### Model-provider retention

Value needed: the retention period Alibaba Cloud Bailian (Beijing; Qwen for the answer, GLM for the semantic precheck) actually applies to confirmed conversation text and analysis context. The pages already refuse a zero-retention promise and a no-training promise. Leave this token blank until the contract states a period.

Suggestion only, not inserted: negotiate the shortest period Bailian will put in the contract. A useful target is no training use, and prompt retention of no more than 24 hours, or zero retention if they offer it. Do not publish “24 hours” or “zero” as if it were already agreed.

| File | Line | Token |
| --- | --- | --- |
| privacy/zh-Hans.html | 91 | `[模型服务商的保留期限]` |
| privacy/zh-Hant.html | 91 | `[模型服務商的保留期限]` |
| privacy/en.html | 91 | `[model-provider retention period]` |
| privacy/es-419.html | 91 | `[plazo de conservación del proveedor del modelo]` |

## Deletion processing time

Value needed: how long Qayvi takes to finish a deletion request that can be matched to an account. On-device deletion is already described as immediate. This token is only the server-side request.

Suggestion only, not inserted: 30 days from a request that contains enough information to find the account. If the account cannot be found, reply that it was not found. Do not start the 30 days, and do not describe the on-device wipe as taking 30 days.

| File | Line | Token |
| --- | --- | --- |
| privacy/zh-Hans.html | 87 | `[删除处理时间]` |
| privacy/zh-Hant.html | 87 | `[刪除處理時間]` |
| privacy/en.html | 87 | `[deletion processing time]` |
| privacy/es-419.html | 87 | `[plazo de procesamiento de la eliminación]` |
| delete-account/zh-Hans.html | 68 | `[删除处理时间]` |
| delete-account/zh-Hant.html | 68 | `[刪除處理時間]` |
| delete-account/en.html | 68 | `[deletion processing time]` |
| delete-account/es-419.html | 68 | `[plazo de procesamiento de la eliminación]` |

## Information needed to find the account

Value needed: what a person must include in the email so Qayvi can find the random account, and where that identifier is shown in the app. The pages say the app does not collect an email address or a Google sign-in identity, so the mailbox alone cannot be matched to an account. No identifier format is suggested. If the app does not show an installation id or the random account id, this token cannot be filled with a working instruction. In-app deletion of that random account is already described and is not this token.

| File | Line | Token |
| --- | --- | --- |
| delete-account/zh-Hans.html | 68 | `[用于查找账号的信息]` |
| delete-account/zh-Hant.html | 68 | `[用於查找帳號的資訊]` |
| delete-account/en.html | 68 | `[information needed to find the account]` |
| delete-account/es-419.html | 68 | `[datos necesarios para encontrar la cuenta]` |

## Already stated (not placeholders)

These periods are written as current practice. They are not tokens.

- Session credential: stops working after 24 hours. That is an access window, not the retention period of the underlying records.
- Minimal consent proof after deletion: 365 days from the latest consent or refusal decision, not from account deletion. A server restart may remove it sooner.
- Deletion confirmation receipt: no expiry. It holds only the deletion-credential hash, the first confirmation time, and the fact that deletion was confirmed.
- Separate in-memory marker of local deletion: 365 days. It does not prove that a provider deleted data.
- Local deletion credentials and queued retries: kept, encrypted, until confirmation and local cleanup succeed. No fixed expiry. Retry needs the app to run again online.
- Saved analyses: on the device until that record is deleted or the account is deleted.
- Downloaded speech models: until removed in model settings or with the app files. Account deletion does not normally remove them.
- Unsaved text, screenshots, and audio copies: current operation only. Cleanup is attempted; there is no guaranteed immediate-erasure time.
- Device free-use records: a scheduled sweep deletes records older than 730 days. They can remain after the random account is deleted until that sweep.
- Safety-attempt records: the same sweep deletes records older than 35 days.
- Paid daily records: not created in this release.
- Purchases: this release does not include RevenueCat, in-app purchases, subscription restore, or a Google Play subscription. Deleting the random account is not a Google Play refund. The app is offered on Google Play only.
- Device summary: a one-way hash of ANDROID_ID combined with an app namespace. The raw ANDROID_ID is not sent to the backend. The hash goes only to Qayvi’s backend, not to the analysis model.
- On-device OCR: ML Kit. On-device audio transcription remains separate. Apple Vision is not named.

## Mismatches to confirm

This environment could not read `DZMing/think-the-chinese-way` (`docs/store/privacy/guiguzi-legal-android-corrections.patch`, `release-gaps.md`, and `google-data-safety.md`). The repository returns 404. The notes below are what these pages now say, set against the product named for this release (口袋里的鬼谷子, Android `com.guiguzi.app`, Qayvi LLC) and the answers a Google Play Data safety form would have to give. Confirm each open item against those files before publication. This pull request does not publish the pages.

1. Android text is now on the pages. The device summary is a one-way hash of ANDROID_ID combined with an app namespace. The raw ANDROID_ID is not sent. There is no iOS Keychain sentence and no iOS Offload App sentence. OCR is ML Kit. The store named on the pages is Google Play only. Confirm `google-data-safety.md` uses that same device-id description.

2. RevenueCat is described as not included in this release, along with in-app purchases and subscription restore. Confirm that `release-gaps.md` still has purchases off. If a later build adds Google Play billing, section 5 is wrong until it is rewritten. Sign-in is still described as absent: the server creates a random account, and the in-app flow deletes that account.

3. Device-quota retention is no longer a token. A scheduled sweep deletes device free-use records older than 730 days and safety-attempt records older than 35 days. They can remain after the random account is deleted until the sweep. This release does not create paid daily records. The 730/35 assignment follows the order those two record types already had, because the patch could not be read. Data safety still cannot say that a deletion request deletes all data while these records remain.

4. Model training and China transfer. Confirmed conversation text and analysis context go phone → InstaBox in the United States → Alibaba Cloud Bailian in Beijing (Qwen answer, GLM precheck), over HTTPS. Session credentials and device summaries stay on the US server and are not sent to the model. The pages do not promise zero retention or no training. If `google-data-safety.md` says conversation text is not shared with a third party, is not transferred internationally, or is not used for model training, that form does not match section 8.

5. Data-safety categories these pages imply, to check against `google-data-safety.md` rather than assume its answers:
   - Email, phone, and Google sign-in identity: not collected.
   - User text: sent to Qayvi’s backend and then to Bailian. Purpose is app functionality. Shared with a third party.
   - Photos and audio: processed on the device. Screenshot text recognition is ML Kit OCR. The analysis request is text only. If the form marks Photos or Audio as collected, that does not match.
   - Device or other IDs: a one-way hash of ANDROID_ID plus an app namespace, sent to Qayvi’s backend for quota control, not to the model, and not for advertising. This release does not include RevenueCat. Declare the hashed device id if the form currently says device IDs are not collected.
   - Approximate location: not collected by the app. This release does not include RevenueCat, so there is no transaction country or country inferred from IP in a purchase SDK.
   - Financial info: no card number in the app. This release does not send a store receipt or purchase token and does not create a subscription.
   - Diagnostics: server request logs omit conversation text, account and session credentials, and IP addresses. The pages still say hosting, network, and SDK logs are not necessarily the same, and they do not claim every connection is encrypted. “Encrypted in transit: yes” for every data type is stronger than section 9. The analysis path itself is described as HTTPS.
   - Advertising, data brokers, and cross-app ad tracking: not in the app. That is not a claim that providers receive no technical data (for example IP addresses on a Hugging Face model download).

6. Web account deletion. The deletion pages explain how to delete the random account in the app, what is deleted, what is kept, and an email fallback. Because there is no email or Google sign-in identity on the account, the email path works only if the user can supply another identifier. That identifier is still a token. Play’s deletion requirement is not met by an email address alone until that token is a real, visible id. Offline in-app deletion is queued until the next time the app is open and online. It does not finish while the app is closed. A server reply that the account mapping is gone is not proof that Bailian deleted its copies. This release does not create a RevenueCat or Google Play purchase record to delete.

7. Withdrawing analysis consent. Declining updates the device only. It does not notify the server, does not guarantee cancellation of a request already running, and does not delete saved analyses or quota records. The pages say this release does not create store transactions. If the store docs say users can withdraw consent and processing stops, that does not match section 7.

8. Age. The service is described as 18+ and the pages say age is not checked. That matches a “not directed at children” listing only if the store listing and content rating say the same thing. The 18+ sentence is not an age gate.

9. Partial deletion that a “all data deleted” answer would miss. The deletion receipt is kept with no expiry (hash, first confirmation time, and the fact of confirmation). The minimal consent proof lasts 365 days from the latest consent or refusal, not from deletion. Device free-use records can remain until they are older than 730 days, and safety-attempt records until they are older than 35 days. This release does not create a store subscription.

10. Speech-model host. The pages name Hugging Face as the current download host. The previous draft said the production host was still undecided. If `release-gaps.md` still has the host as undecided, the Hugging Face sentence is only the beta host.

11. Production path. The InstaBox → Bailian Beijing path is stated without the old “internal testing only” label. If the release host or the model provider is different, section 8 is wrong for the store build.

12. Controller name. The pages now name Qayvi LLC. The Play Console developer name and any “data controller” answer in the store docs need to be the same entity. There is still no postal address on the pages. Some privacy laws expect one; it is not a token in this set.

13. The pages are not store-ready while the tokens above are blank. The draft banner is intentional and this pull request does not publish them.
