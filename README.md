# SnappFeed Privacy and Support Website

This repository contains a cross-platform privacy policy and support page for the SnappFeed iOS and Android applications.

## Included files

- `index.html` — public Privacy Policy page
- `support.html` — public Support page
- `privacy-policy.md` — editable Markdown copy
- `README.md` — deployment instructions

## Recommended GitHub Pages setup

### Option A — Clean root URL

If your GitHub username is exactly `snappfeed`, create a public repository named:

`snappfeed.github.io`

The published website will normally be:

`https://snappfeed.github.io/`

The support URL will be:

`https://snappfeed.github.io/support.html`

### Option B — Project repository

Create a public repository named:

`snappfeed-privacy`

The published website will normally be:

`https://YOUR_GITHUB_USERNAME.github.io/snappfeed-privacy/`

The support URL will be:

`https://YOUR_GITHUB_USERNAME.github.io/snappfeed-privacy/support.html`

## Publish from the GitHub website

1. Open the target repository.
2. Select **Add file → Upload files**.
3. Upload:
   - `index.html`
   - `support.html`
   - `privacy-policy.md`
   - `README.md`
4. Commit the files to the `main` branch.
5. Open **Settings** in the repository.
6. In the left sidebar, open **Pages** under **Code and automation**.
7. Under **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/(root)**
8. Select **Save**.
9. Wait for GitHub Pages to finish deployment.
10. Open the final URL in an incognito/private window and confirm:
    - the page opens without signing in;
    - the Privacy Policy is visible;
    - the Support link works;
    - the email link works;
    - the website uses HTTPS.

## Publish using Git

After creating an empty repository, run from this folder:

```bash
git init
git add index.html support.html privacy-policy.md README.md
git commit -m "Add SnappFeed privacy policy and support pages"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

Then enable GitHub Pages in **Settings → Pages**.

## Store-console URLs

Use the Privacy Policy URL in both:

- App Store Connect → App Privacy → Privacy Policy URL
- Google Play Console → App content → Privacy policy

Use the Support URL in:

- App Store Connect → App version → Support URL
- Google Play listing or app support contact fields where relevant

Add the Privacy Policy link inside the SnappFeed app as well.

## Before publishing

Confirm that these statements match the submitted iOS and Android builds:

- no user accounts;
- no SnappFeed backend storage;
- no advertising SDK;
- no analytics SDK;
- no crash-reporting SDK added by the app;
- no remote photo upload;
- no public content sharing;
- no background location;
- Google Maps is the principal online service.

Update the policy before or when any of these practices change.

## Important

The Privacy Policy does not replace:

- Apple App Privacy answers in App Store Connect;
- Google Play Data safety answers;
- permission disclosures shown inside the app;
- any legally required consent or notice.

Third-party SDK behavior must be included in the store disclosures.
