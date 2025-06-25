# Urban Truck Characterization using Google Street View Imagery

🚛 **Exploring Drive-by Sensing and Deep Learning for Urban Truck Characterization**

[![Website](https://img.shields.io/badge/Website-Live-brightgreen)](https://ai-mobility-research-lab.github.io/gsv-truck-characterization/)
[![Paper](https://img.shields.io/badge/Paper-PDF-red)](./elsarticle-template-num.pdf)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue)](https://github.com/AI-Mobility-Research-Lab)

## 🎯 Project Overview

This research introduces an innovative approach to urban truck monitoring through drive-by sensing technology and deep learning. Using Google Street View imagery, we developed a comprehensive framework for large-scale urban freight monitoring that significantly improves the spatial resolution of data collection over traditional traffic monitoring methods.

### 🔬 Key Innovations

- **Drive-by Sensing Integration**: First study to pioneer drive-by sensing and deep learning for urban truck distribution analysis at scale
- **DepthAnything Enhancement**: Novel integration of DepthAnything with YOLO for improved object detection accuracy
- **AI-Assisted Data Augmentation**: Semi-automated approach using Claude-3.7-sonnet boosting specialty services truck recall from 17% to 50%
- **Environmental Impact Assessment**: Correlation analysis showing trucks contribute ~16% to PM2.5 emissions in studied Manhattan areas

## 📊 Dataset & Results

- **22,589** panoramic Google Street View images
- **10,000** manually annotated images across 6 vehicle categories
- **10 detailed truck categories** for fine-grained classification
- **Manhattan case study** with environmental correlation analysis

## 🛠️ Methodology

Our framework consists of several integrated components:

1. **Data Collection**: Google Street View panoramic imagery processing
2. **Object Detection**: Customized YOLO model for truck detection
3. **Depth Filtering**: DepthAnything integration for spatial accuracy
4. **Fine-grained Classification**: EfficientNet for detailed truck categorization
5. **Environmental Analysis**: Correlation with NYC air quality data

## 🏗️ Website Deployment Instructions

### Hosting on AI Mobility Research Lab GitHub Pages

This website is designed to be hosted on the AI Mobility Research Lab GitHub organization page. Follow these steps:

#### Step 1: Repository Setup
```bash
# Clone this repository to the AI-Mobility-Research-Lab organization
git clone https://github.com/AI-Mobility-Research-Lab/gsv-truck-characterization.git
cd gsv-truck-characterization
```

#### Step 2: Enable GitHub Pages
1. Go to the repository settings on GitHub
2. Navigate to **Pages** section
3. Under **Source**, select "Deploy from a branch"
4. Choose **main branch** and **/ (root)** folder
5. Click **Save**

#### Step 3: Configure Custom Domain (Optional)
If you want to use a custom domain:
1. Add a `CNAME` file with your domain name
2. Configure DNS settings with your domain provider
3. Update GitHub Pages settings to use the custom domain

#### Step 4: Website URL
Your website will be available at:
- Default: `https://ai-mobility-research-lab.github.io/gsv-truck-characterization/`
- Custom domain: `https://your-custom-domain.com` (if configured)

### Local Development

To run the website locally for development:

```bash
# Simple HTTP server using Python
python -m http.server 8000

# Or using Node.js
npx http-server

# Then visit http://localhost:8000
```

## 📁 Repository Structure

```
gsv-truck-characterization/
├── index.html                          # Main website file
├── README.md                           # This file
├── elsarticle-template-num.pdf         # Research paper PDF
├── images/                             # All visualization assets
│   ├── overall_architecture.png
│   ├── class_distribution_horizontal.png
│   ├── confusion_matrix_normalized.png
│   ├── classification_metrics_efficientnet_f1_plot.png
│   ├── model_improvement_comparison.png
│   ├── Strip_image_depthAnything_.png
│   ├── truckpm25.png
│   ├── Individual Four Perspectives_Montage.png
│   ├── Merged Four Perspectives Annotated Image.png
│   └── graphic_abstract.png
└── assets/                             # Additional assets (if needed)
```

## 🎨 Website Features

- **Responsive Design**: Mobile-friendly layout with Bootstrap 5
- **Modern UI**: Clean, professional academic website design
- **Interactive Navigation**: Smooth scrolling and fixed navigation
- **Image Gallery**: Showcases research results and methodology
- **Download Section**: Direct access to paper and supplementary materials
- **Citation Generator**: Ready-to-use BibTeX citation
- **SEO Optimized**: Meta tags for better search engine visibility


## 👥 Authors

- **Bo Shang** - Graduate Research Assistant, The City College of New York, CUNY
- **Yiqiao Li** - Assistant Professor (Corresponding Author), The City College of New York, CUNY
- **Blanche Horbach** - Master's Candidate, The City College of New York, CUNY  
- **Kevin Villon** - Research Assistant, The City College of New York, CUNY

## 📧 Contact

For questions about this research:
- **Yiqiao Li** (Corresponding Author): [yli4@ccny.cuny.edu](mailto:yli4@ccny.cuny.edu)
- **Bo Shang**: [bshang@ccny.cuny.edu](mailto:bshang@ccny.cuny.edu)

## 🏢 Affiliation

**AI Mobility Research Lab**  
The City College of New York, CUNY  
160 Convent Avenue  
New York, NY 10031, USA

## 📋 Keywords

Deep Learning • Object Detection • Urban Freight Data • Google Street View • Large-Scale Data Collection • Correlation Analysis • Emission Data • DepthAnything • Drive-by Sensing • Urban Transportation

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*This website template is designed for academic research presentation and can be easily customized for similar projects.* 
