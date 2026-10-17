# Chorus — Privacy Policy

**Last updated: 17 October 2026**

Chorus – All AI, One Place (`com.aihub.app`) is provided by AIHUB. Chorus is a bring-your-own-key AI client and local workspace. This policy explains data stored by the app, information sent when you use connected services, and your controls. Contact: **getaihubapp@gmail.com**.

## 1. Your local workspace

Chorus stores saved conversations and attachments, imported document text, projects, notes, prompts, assistants, selected memories, Lens cards, Mini Tools, Council results, decision records, Radar watches, settings, and usage records in the app's storage on your device. These records are not synced to an AIHUB workspace server. Different signed-in accounts have separate local records. Signing in on a new device does not transfer your connections or workspace.

Provider and search API keys are encrypted at rest using AES-GCM and a non-extractable key held in the app's device storage. Chorus decrypts a key when authenticating a request to its configured service. This protects stored keys; it does not make a compromised device safe or prevent the app from using a key.

Android automatic cloud backup and device-to-device transfer of app data are disabled. Uninstalling the app removes its local storage. Keep a manual export if you need a recoverable copy.

## 2. Account sign-in

Chorus uses Google Firebase Authentication for email/password and Google sign-in. Firebase processes the account information needed to authenticate you, including your email address, account identifier and authentication credentials. Google sign-in may provide your Google profile name and image. Firebase also processes technical information such as IP addresses and user-agent information for service operation, security and abuse prevention. Password-account email verification is required before using Chorus.

See [Firebase's privacy information](https://firebase.google.com/support/privacy) and [Google's Privacy Policy](https://policies.google.com/privacy). AIHUB does not receive your Google account password.

## 3. AI, search and connected endpoints

When you send an AI request, Chorus sends the content needed for that task directly to your selected provider or configured gateway. This can include prompts, conversation context, images, document text, instructions, selected memories, source material and workspace records you choose to process. Council sends a question to two selected members and their answers to the reviewer. Remember Why's optional AI action sends the records within the displayed scope to the model you select.

Optional web search sends the query to your configured search service; selected results may be included in the AI context. Connection tests and model discovery contact the configured endpoint. Providers and gateways receive network information such as your IP address as part of a request. Their retention, training, billing and deletion practices are governed by their own policies and your agreement with them. A custom gateway may route your content to further providers. Check whom you connect and avoid sending information you do not want that service to process.

Provider presets use HTTPS. Chorus also permits a user-configured HTTP endpoint for local or network servers. HTTP traffic, including content and credentials for that connection, is not encrypted in transit. Use HTTPS for remote connections.

## 4. Files, photos, camera and voice

You choose which files or images to import or share into Chorus. Document text is extracted locally. Importing content does not itself send the document to an AI provider; using it in an AI action sends the relevant text or image to the selected endpoint.

Chorus Lens uses bundled Google ML Kit Latin-script text recognition on Android. Image recognition runs on the device. ML Kit can collect SDK diagnostic and usage metadata, including device/app information, installation identifiers, performance information, feature events, configuration and input/output sizes. These are distinct from uploading the photo for cloud AI. See [ML Kit's Android data disclosure](https://developers.google.com/ml-kit/android-data-disclosure).

Microphone permission is requested when you use voice input. Recorded audio is sent to a connected Groq or OpenAI transcription endpoint and the transcript becomes a draft you can review. Chorus does not keep a voice recording as part of the chat history. Sending the draft then sends the text to your chosen chat model. Listening to replies uses your device's text-to-speech engine; that engine's voices and network processing depend on your device settings and its provider.

Camera and photo/file access support the items you explicitly capture or select. Declining microphone or camera access leaves typing and other import methods available.

## 5. Radar, notifications and the widget

Personal Radar requests public HTTPS pages you choose and stores local text snapshots and change excerpts. Android can repeat these requests in the background while a watch is enabled, subject to system conditions. The source website receives the request and ordinary network information. Radar does not send your AI keys to the watched website. Pause or remove watches to stop their checks; signing out suspends this account's Android checks.

Notifications are optional and show a generic prompt to review source changes. The home-screen widget uses local appearance settings and opens chat or voice; it does not itself send a conversation to an AI provider.

## 6. Private chats and retained records

Private chats are not saved to normal conversation history and do not use saved memories as automatic chat context. Content you submit still reaches the selected provider, which has its own retention policy. Private mode does not make provider traffic anonymous.

Saved source quotes in Lens and Remember Why are retained copies. Removing an original chat or note does not automatically remove a quote already saved in another record. Delete the saved record or retained quote as well when you want to remove that copy.

## 7. Safety reports, exports, backups and support

In versions offering **Report AI Content**, you can send selected AI content and an optional comment to AIHUB for safety review without leaving Chorus. Before submitting, you can inspect and edit the excerpt, choose a reason and remove personal or secret details. Known API-key patterns are redacted, but this is not a guarantee that every secret will be detected. Only the report form, your Chorus account identifier, screen name, model identifier when available, app version, request identifier and server submission time are sent to AIHUB through Google Cloud Firestore over HTTPS. The app does not automatically attach other conversations, stored connection keys or files. Private-chat content is included only if you explicitly report the selected excerpt.

Reports are stored for developer review, abuse prevention and response to the reported safety issue. Project administrators can review them; other Chorus users cannot read your reports. A success receipt appears only after the receiving server confirms delivery. Reports are not an emergency response service. Submitted reports are retained until your account is deleted or the developer removes them when they are no longer needed for safety review. Account deletion in versions with reporting removes reports before deleting the authentication account and local workspace. If you use an older app version or email us to request deletion, we remove reports associated with the verified account as part of that request.


Exports and backups are files you control. Backups exclude provider/search API keys but contain readable, unencrypted workspace text. They are not a complete archive of all binary attachments. Anyone you share an exported file with may be able to read it. Calendar, CSV, tool and Council exports may likewise contain your content. Review files before sharing them and store them securely.

Support or bug-report messages are sent only when you choose to send them using your email app or another external service. A prefilled report may contain app/platform information and recent provider/model error details. Review it before sending. If you contact AIHUB, we process the information you send to answer your request, troubleshoot or handle account deletion; do not send passwords or API keys. We keep support correspondence only as needed for those purposes and any applicable obligations.

Chorus does not sell your conversations. Authentication and ML Kit technical data processing described above still apply; there is no separate AIHUB conversation-analytics service.

### Sponsored responses in ad-enabled builds

The published build 99 (1.0.9) contains no advertising SDK. Build 100 offers optional **Sponsored Responses** using Google AdMob. From build 101, sponsored cards support free app use and there is no app-wide ad on/off switch. This section applies when you use a build with that feature. An ad card is separate from the AI answer; Chorus does not send your prompts, conversations, attachments, saved memories, provider/search API keys or Chorus account ID to AdMob to choose ads. Ads are not included in AI conversation context, exports or saved answers. Private Chat does not display these cards.

Google's Mobile Ads SDK may process IP addresses (which can indicate approximate location), device and advertising identifiers, diagnostics, and ad interaction information for advertising, measurement, security and fraud prevention. This processing involves Google and the advertising technology providers disclosed in the consent interface. Chorus does not request precise device location for ads. The app requests non-personalized ads; that setting does not mean that no device information is processed. See [Google's advertising privacy information](https://policies.google.com/technologies/ads) and [the Mobile Ads SDK data disclosure](https://developers.google.com/admob/android/privacy/play-data-disclosure).

Where applicable, Google's consent message appears before ads can be requested. In ad-enabled builds, use **Settings → Sponsored Responses → Ad Privacy Options** to manage or withdraw consent where Google provides that form. Build 100 also provides a **Show Sponsored Cards** switch; build 101 and later do not. Required consent and privacy choices remain available. Withdrawing consent does not reverse information already processed by Google. Android's advertising ID settings provide additional device controls. Deleting your Chorus account does not erase advertising records retained by Google under its own policies.

## 8. Deletion and your choices

You can delete saved items in the app, remove provider connections, pause Radar, revoke device permissions and revoke API keys in your provider's dashboard. Export anything you want to keep before deletion.

To delete your Chorus account, open **Settings → Account → Delete Account and All Data**, follow the confirmation and re-authentication steps, and complete deletion. This removes the Firebase account and that account's local workspace from the device performing deletion. Versions with in-app reporting first remove the account's submitted reports. If report cleanup fails, the app preserves the account and local workspace and asks you to retry or contact support; some reports may already have been removed. Signing in on another device does not remotely wipe that device's local files. Uninstall Chorus there or remove its local app data as well.

You can also request account deletion by emailing **getaihubapp@gmail.com** from the account address, as explained on the [account deletion page](https://subhashns1988-svg.github.io/aihub-legal/delete-account.html). We may verify ownership to protect the account. AIHUB cannot remotely retrieve local records or erase files you exported, other recipients' copies, or data retained by your selected providers; contact those services for their deletion controls. Google may retain technical records according to its applicable policies and obligations.

## 9. Children and policy updates

Chorus is not directed at children under 13 and AIHUB does not knowingly collect their personal information. Provider age requirements also apply.

When this policy changes, we update the date and publish the revised policy here. Contact **getaihubapp@gmail.com** with privacy questions or requests.
