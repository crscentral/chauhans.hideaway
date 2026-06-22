# Deploying The Chauhans Hideaway Website to GitHub Pages

## Step 1: Create a GitHub Account
If you don't have one, go to https://github.com and sign up for free.

## Step 2: Create a New Repository
1. Click the **+** icon (top right) → **New repository**
2. Name it exactly: `chauhanshideaway.com` (or any name you prefer)
3. Set it to **Public**
4. Click **Create repository**

## Step 3: Upload the Website File
1. On the new repository page, click **uploading an existing file**
2. Drag and drop `index.html` from your computer
3. Scroll down, add a commit message like "Initial website upload"
4. Click **Commit changes**

## Step 4: Enable GitHub Pages
1. Go to your repository **Settings** (top tab)
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Choose branch: `main`, folder: `/ (root)`
5. Click **Save**

## Step 5: Access Your Website
After 1–2 minutes, your site will be live at:
`https://YOUR-GITHUB-USERNAME.github.io/REPOSITORY-NAME/`

---

## Using a Custom Domain (chauhanshideaway.com)

### In GitHub Pages settings:
1. Under **Custom domain**, type: `chauhanshideaway.com`
2. Click **Save**
3. Enable **Enforce HTTPS** (checkbox)

### At your domain registrar (where you bought chauhanshideaway.com):
Add these DNS records:

**A Records** (point to GitHub's servers):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME Record:**
```
www → YOUR-GITHUB-USERNAME.github.io
```

DNS changes take 24–48 hours to propagate.

---

## Updating the Website Later
1. Make changes to `index.html` on your computer
2. Go to your GitHub repository
3. Click on `index.html` → click the **pencil edit icon**
4. Or simply drag the new file to upload (overwrite)

---

## Connecting Enquiry Form to Email
The enquiry form uses `mailto:` which opens the visitor's email client. 
For a proper server-side form (so visitors don't need email app), consider:
- **Formspree** (free): Replace the submit function with a Formspree endpoint
- **Netlify Forms**: Host on Netlify instead for built-in form handling

---

*Need help? Contact your web developer or reach out to GitHub Support.*
