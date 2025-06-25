# Website Deployment Guide for AI Mobility Research Lab

This guide provides step-by-step instructions for deploying the Urban Truck Characterization website to the AI Mobility Research Lab GitHub organization.

## 🚀 Quick Deployment Steps

### 1. Create Repository in AI-Mobility-Research-Lab Organization

1. **Go to GitHub**: Navigate to https://github.com/AI-Mobility-Research-Lab
2. **Create New Repository**:
   - Click "New" to create a new repository
   - Repository name: `gsv-truck-characterization` (or your preferred name)
   - Description: `Urban Truck Characterization using Google Street View Imagery - Research Website`
   - Set as **Public** repository
   - Initialize with README: **No** (we'll push our existing files)

### 2. Push Website Files to Organization Repository

```bash
# Navigate to your current project directory
cd /path/to/your/gsv_truck_part_a

# Initialize git repository if not already done
git init

# Add the new organization repository as remote origin
git remote add origin https://github.com/AI-Mobility-Research-Lab/gsv-truck-characterization.git

# Add all website files
git add index.html README.md .nojekyll DEPLOYMENT_GUIDE.md
git add *.png *.pdf  # Add all images and PDF

# Commit the files
git commit -m "Initial website deployment for Urban Truck Characterization research"

# Push to main branch
git push -u origin main
```

### 3. Enable GitHub Pages

1. **Go to Repository Settings**:
   - Navigate to `https://github.com/AI-Mobility-Research-Lab/gsv-truck-characterization`
   - Click **Settings** tab

2. **Configure Pages**:
   - Scroll down to **Pages** section (left sidebar)
   - Under **Source**, select "Deploy from a branch"
   - Choose **main** branch
   - Select **/ (root)** folder
   - Click **Save**

3. **Wait for Deployment**:
   - GitHub will automatically build and deploy your website
   - This typically takes 1-5 minutes
   - You'll see a green checkmark when deployment is successful

### 4. Access Your Website

Your website will be available at:
```
https://ai-mobility-research-lab.github.io/gsv-truck-characterization/
```

## 🔧 Advanced Configuration

### Custom Domain Setup (Optional)

If you want to use a custom domain like `truck-research.ai-mobility.org`:

1. **Add CNAME File**:
   ```bash
   echo "truck-research.ai-mobility.org" > CNAME
   git add CNAME
   git commit -m "Add custom domain configuration"
   git push
   ```

2. **Configure DNS**:
   - Add a CNAME record in your DNS settings
   - Point your subdomain to `ai-mobility-research-lab.github.io`

3. **Update GitHub Settings**:
   - Go to repository Settings > Pages
   - Enter your custom domain in the "Custom domain" field
   - Enable "Enforce HTTPS"

### File Organization

Ensure your repository has this structure:
```
gsv-truck-characterization/
├── index.html                              # Main website
├── README.md                               # Project documentation
├── DEPLOYMENT_GUIDE.md                     # This file
├── .nojekyll                               # Prevents Jekyll processing
├── CNAME                                   # Custom domain (if used)
├── elsarticle-template-num.pdf             # Research paper
├── graphic_abstract.png                    # Abstract figure
├── overall_architecture.png                # Architecture diagram
├── class_distribution_horizontal.png       # Results figures
├── confusion_matrix_normalized.png
├── classification_metrics_efficientnet_f1_plot.png
├── model_improvement_comparison.png
├── Strip_image_depthAnything_.png
├── truckpm25.png
├── Individual Four Perspectives_Montage.png
├── Merged Four Perspectives Annotated Image.png
└── other image files...
```

## 🔍 Troubleshooting

### Common Issues and Solutions

1. **Website Not Loading**:
   - Check that `index.html` is in the root directory
   - Ensure GitHub Pages is enabled in repository settings
   - Wait 5-10 minutes for initial deployment

2. **Images Not Displaying**:
   - Verify image file names match exactly (case-sensitive)
   - Check that images are committed and pushed to the repository
   - Use relative paths (e.g., `./image.png` not absolute paths)

3. **Custom Domain Issues**:
   - Verify DNS settings are correct
   - Check that CNAME file contains only the domain name
   - Wait for DNS propagation (can take up to 24 hours)

4. **SSL Certificate Issues**:
   - GitHub automatically provides SSL for `.github.io` domains
   - For custom domains, it may take a few hours to provision

### Verification Steps

To verify your deployment:

1. **Check Repository**:
   - All files are present in the GitHub repository
   - Latest commit shows your website files

2. **Test Website**:
   - Visit the GitHub Pages URL
   - Check all sections load correctly
   - Verify images display properly
   - Test download links for PDF

3. **Mobile Testing**:
   - Test website on mobile devices
   - Ensure responsive design works correctly

## 🔄 Updating the Website

To update the website after initial deployment:

```bash
# Make your changes to index.html or other files
# Then commit and push the changes

git add .
git commit -m "Update research findings and add new results"
git push

# GitHub Pages will automatically rebuild and deploy
# Changes typically appear within 1-2 minutes
```

## 📊 Analytics and Monitoring

Consider adding:
- **Google Analytics** for visitor tracking
- **GitHub repository insights** to monitor traffic
- **Social media preview optimization** using Open Graph tags (already included)

## 🛡️ Security and Best Practices

- Keep the repository **public** for GitHub Pages to work with the free plan
- Use **relative paths** for all links and images
- Include **meta tags** for SEO (already included in template)
- Add **structured data** for better search engine understanding

## 📞 Support

For additional help:
- **GitHub Pages Documentation**: https://docs.github.com/en/pages
- **AI Mobility Research Lab**: Contact repository administrators
- **Technical Issues**: Create an issue in the repository

---

*This deployment guide ensures your research website is properly hosted and accessible to the academic community and general public.* 