# Detailed Guide: Hosting Your Website on GitHub Pages

This guide provides comprehensive, step-by-step instructions for hosting your Mate Sri Lanka website on GitHub Pages.

## Prerequisites

- A GitHub account (create one at [github.com](https://github.com) if you don't have one)
- Git installed on your computer (download from [git-scm.com](https://git-scm.com/downloads))
- Your website files ready (HTML, CSS, JavaScript, images)

## Step 1: Prepare Your Website Files

Before uploading to GitHub, ensure your website files are properly organized:

1. Make sure your main page is named `index.html`
2. Verify all file paths are correct (CSS, JavaScript, images)
3. Test your website locally to ensure everything works

## Step 2: Create a GitHub Repository

1. Log in to your GitHub account
2. Click the "+" icon in the top-right corner and select "New repository"
3. Name your repository (e.g., "mate-sri-lanka")
4. Add a description (optional)
5. Choose "Public" visibility (required for GitHub Pages with a free account)
6. Do NOT initialize with README, .gitignore, or license (we'll add these later)
7. Click "Create repository"

## Step 3: Upload Your Website to GitHub

### Option A: Using Git Command Line (Recommended)

1. Open Terminal (Mac/Linux) or Command Prompt/Git Bash (Windows)
2. Navigate to your website folder:
   ```
   cd path/to/your/website/folder
   ```

3. Initialize a Git repository:
   ```
   git init
   ```

4. Add all your files to the repository:
   ```
   git add .
   ```

5. Commit the files:
   ```
   git commit -m "Initial website commit"
   ```

6. Link your local repository to your GitHub repository:
   ```
   git remote add origin https://github.com/yourusername/mate-sri-lanka.git
   ```
   (Replace "yourusername" with your actual GitHub username and "mate-sri-lanka" with your repository name)

7. Push your files to GitHub:
   ```
   git push -u origin main
   ```
   
   Note: If you're using an older version of Git, you might need to use `master` instead of `main`:
   ```
   git push -u origin master
   ```

8. Enter your GitHub credentials if prompted

### Option B: Using GitHub Web Interface

1. On your new repository page, click "uploading an existing file"
2. Drag and drop your website files and folders
3. Click "Commit changes"
4. Repeat if necessary (GitHub web upload has file number limitations)

## Step 4: Configure GitHub Pages

1. Go to your repository on GitHub
2. Click the "Settings" tab
3. Scroll down to the "GitHub Pages" section (or click "Pages" in the left sidebar)
4. Under "Source", select "main" branch (or "master" if that's what you used)
5. Click "Save"
6. Wait a few minutes for GitHub to build and deploy your site
7. You'll see a message saying "Your site is published at https://yourusername.github.io/mate-sri-lanka/"

## Step 5: Verify Your Website

1. Click on the URL provided in the GitHub Pages section
2. Verify that your website loads correctly
3. Test all links, images, and functionality

## Step 6: Adding a Custom Domain (Optional)

If you want to use your own domain (e.g., www.matesrilanka.com) instead of the default GitHub Pages URL:

1. Purchase a domain from a domain registrar (e.g., Namecheap, GoDaddy)
2. In your repository settings, under "GitHub Pages" > "Custom domain", enter your domain name
3. Click "Save"
4. A file named `CNAME` will be added to your repository

5. Configure your domain's DNS settings with your domain registrar:
   
   ### For an apex domain (e.g., matesrilanka.com):
   Add these A records pointing to GitHub Pages' IP addresses:
   ```
   A    @    185.199.108.153
   A    @    185.199.109.153
   A    @    185.199.110.153
   A    @    185.199.111.153
   ```

   ### For a www subdomain (e.g., www.matesrilanka.com):
   Add a CNAME record:
   ```
   CNAME    www    yourusername.github.io.
   ```

6. Wait for DNS changes to propagate (can take up to 48 hours)
7. Enable HTTPS by checking "Enforce HTTPS" in the GitHub Pages settings (available after DNS propagation)

## Step 7: Updating Your Website

When you need to make changes to your website:

### Using Git Command Line:

1. Make changes to your local files
2. Stage the changes:
   ```
   git add .
   ```
3. Commit the changes:
   ```
   git commit -m "Description of changes"
   ```
4. Push to GitHub:
   ```
   git push
   ```

### Using GitHub Web Interface:

1. Navigate to the file you want to edit
2. Click the pencil icon to edit
3. Make your changes
4. Scroll down and click "Commit changes"

GitHub Pages will automatically update your website with the new changes.

## Troubleshooting

### Website Not Publishing

- Ensure your repository is public
- Verify that your main HTML file is named `index.html`
- Check that you've selected the correct branch in GitHub Pages settings
- Wait a few minutes for changes to propagate

### Custom Domain Issues

- Verify DNS settings with your domain registrar
- Ensure the CNAME file contains only your domain name
- Wait up to 48 hours for DNS changes to propagate
- Check for typos in your domain name

### 404 Errors

- Check file paths in your HTML, CSS, and JavaScript files
- Ensure all links are relative to the repository root
- Verify that all referenced files exist in the repository

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Custom Domain Setup Guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [GitHub Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)

---

If you encounter any issues not covered in this guide, please refer to the [GitHub Pages documentation](https://docs.github.com/en/pages) or search for solutions on [Stack Overflow](https://stackoverflow.com/questions/tagged/github-pages). 