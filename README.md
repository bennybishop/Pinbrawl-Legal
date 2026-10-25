# Pinbrawl — legal information

Static English legal pages for the Android game Pinbrawl, developed by Benjamin Dehant.
Contact: benjamin.dehant@gmail.com.

## Public URLs
- https://bennybishop.github.io/Pinbrawl-Legal/
- https://bennybishop.github.io/Pinbrawl-Legal/privacy/
- https://bennybishop.github.io/Pinbrawl-Legal/data-deletion/

## Publishing
GitHub Settings → Pages → Deploy from a branch → main → /(root).
The .nojekyll file publishes plain HTML/CSS; there is no external font, JavaScript, form, analytics, or cookie dependency.
The policy includes GitHub hosting and email handling rather than claiming the website processes no data.

## Evidence and scope — 25 October 2026
The inspected Unity project integrates TinySauce 8.3.2. TinySauceBootstrap keeps its root disabled until configuration is complete and gates gameplay analytics on analytics consent. Recent APKs built by build-offline-pvp.ps1 exclude TinySauce from the isolated build copy and restore the SDK afterwards. They are local AI/offline tests.
ProgressStore writes app-local JSON saves and a recovery copy. The current interface has no player registration or Facebook Login.
SDK installation is not evidence of collection in an APK. No network audit of a future publishing build has been performed.
No credentials, tokens, package keys, player identifiers, or private project source are included in this repository.

## Confirm before a Google Play / Voodoo release
- [ ] Identify the exact APK/AAB and confirm whether it is still offline. Do not reuse an offline-only policy for an instrumented release.
- [ ] Verify the controller's full legal identity, required contact/address details and any establishment/representative details. Do not invent an address or DPO.
- [ ] Confirm target audience / Families status and age restrictions. No invented “13+” audience statement.
- [ ] List actually enabled SDKs and network endpoints. TinySauce setup also contains Adjust configuration; confirm attribution before activation rather than silently omitting an active recipient.
- [ ] Record actual fields: gameplay/session events, installation/device/ad identifiers, IP/network information, consent, diagnostics, attribution and any ads, only where evidenced.
- [ ] For each active purpose/provider, document legal basis, controller/processor roles, retention settings and international-transfer safeguards. Add them to the policy before collection.
- [ ] Test consent refusal and withdrawal. Existing analytics consent gating alone is not proof that every integrated SDK or advertising event respects the choices.
- [ ] Verify any Google Play services, backup/cloud save, account creation, multiplayer, ads, purchases, crash reporting or additional permissions in the final build.
- [ ] Align Play Console Data safety declarations, in-app policy link, consent partner list and Meta privacy/deletion URLs with the released build.
- [ ] Decide whether the Meta configuration accepts a deletion-instructions URL or requires a real callback. Static HTML is not a callback endpoint.
- [ ] Establish support-record retention and provider deletion procedures, including verification, lawful exceptions and GDPR response time limits.

## References checked
- Visual style and legal-section structure: https://github.com/bennybishop/Drone-Rush-Legal (read only).
- Google Play User Data: https://support.google.com/googleplay/android-developer/answer/10144311?hl=en
- Google Play account deletion: https://support.google.com/googleplay/android-developer/answer/13327111?hl=en
- GDPR Articles 5, 6, 12–22, 44–49: https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng
- GitHub Pages publishing: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Maintenance
Update the policy date when processing changes. Keep deletion instructions accessible without login and retain their plain email fallback.
Drone-Rush-Legal is a design reference only and has not been modified.
