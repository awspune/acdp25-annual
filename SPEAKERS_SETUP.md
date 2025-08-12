# Speaker Section Setup Guide

## 🎯 Overview
This guide will help you set up the speaker section with actual photos and information from the provided Google Drive and Google Sheets links.

## 📁 Google Drive Photos
**Link:** https://drive.google.com/drive/folders/14YhsrBJMO0rhEJw_pkwXKNnfGlPYu3kf

### 📸 Photo Organization (Alphabetical Order)
1. **Download all speaker photos** from the Google Drive folder
2. **Rename them alphabetically** as follows:

#### Main Speakers (6 total):
- `speaker1.jpg` - First speaker alphabetically
- `speaker2.jpg` - Second speaker alphabetically  
- `speaker3.jpg` - Third speaker alphabetically
- `speaker4.jpg` - Fourth speaker alphabetically
- `speaker5.jpg` - Fifth speaker alphabetically
- `speaker6.jpg` - Sixth speaker alphabetically

#### Co-Speakers (6 total):
- `co-speaker1.jpg` - First co-speaker alphabetically
- `co-speaker2.jpg` - Second co-speaker alphabetically
- `co-speaker3.jpg` - Third co-speaker alphabetically
- `co-speaker4.jpg` - Fourth co-speaker alphabetically
- `co-speaker5.jpg` - Fifth co-speaker alphabetically
- `co-speaker6.jpg` - Sixth co-speaker alphabetically

### 🔄 How to Organize Alphabetically:
1. **Sort by first name** (A-Z)
2. **If same first name, sort by last name** (A-Z)
3. **Assign numbers sequentially** (1, 2, 3, etc.)

## 📊 Speaker Information
**Link:** https://docs.google.com/spreadsheets/d/190pylAOQiOZ5oaMNCDNHCL4K1GzCXlzC/edit?gid=1807180763#gid=1807180763

## 📂 File Placement
1. **Create the speakers directory** (if not exists):
   ```bash
   mkdir -p assets/img/speakers
   ```

2. **Place all renamed photos** in `assets/img/speakers/`

3. **Verify file structure:**
   ```
   assets/img/speakers/
   ├── speaker1.jpg
   ├── speaker2.jpg
   ├── speaker3.jpg
   ├── speaker4.jpg
   ├── speaker5.jpg
   ├── speaker6.jpg
   ├── co-speaker1.jpg
   ├── co-speaker2.jpg
   ├── co-speaker3.jpg
   ├── co-speaker4.jpg
   ├── co-speaker5.jpg
   └── co-speaker6.jpg
   ```

## ✏️ Update HTML Content
In `index.html`, update each speaker card with:

### For Main Speakers:
```html
<img src="assets/img/speakers/speaker1.jpg" alt="[ACTUAL_NAME]" style="width: 200px; height: 200px; border-radius: 50%; object-fit: cover; box-shadow: 0 4px 20px rgba(0,0,0,0.15); transition: all 0.3s ease;">
<h4 style="margin-bottom: 8px; color: #232f3e; font-size: 1.3rem;">[ACTUAL_NAME]</h4>
<p style="color: #666; font-size: 1rem; margin-bottom: 0;">[ACTUAL_DESIGNATION]</p>
<a href="[LINKEDIN_URL]" class="linkedin-link" target="_blank" style="display: none;">LinkedIn Profile</a>
```

### For Co-Speakers:
```html
<img src="assets/img/speakers/co-speaker1.jpg" alt="[ACTUAL_NAME]" style="width: 200px; height: 200px; border-radius: 50%; object-fit: cover; box-shadow: 0 4px 20px rgba(0,0,0,0.15); transition: all 0.3s ease;">
<h4 style="margin-bottom: 8px; color: #232f3e; font-size: 1.3rem;">[ACTUAL_NAME]</h4>
<p style="color: #666; font-size: 1rem; margin-bottom: 0;">[ACTUAL_DESIGNATION]</p>
<a href="[LINKEDIN_URL]" class="linkedin-link" target="_blank" style="display: none;">LinkedIn Profile</a>
```

## 🎨 Image Requirements
- **Format:** JPG or PNG
- **Size:** Recommended 400x400px or larger (will be automatically resized to 200x200px)
- **Style:** Professional headshots with clear faces
- **Background:** Clean, professional backgrounds preferred

## 🚀 Features
- **Circular images** with hover effects
- **LinkedIn overlay** appears on hover
- **Click to open** LinkedIn profile in new tab
- **Responsive design** for all devices
- **Fallback placeholders** when images are missing

## 🧪 Testing
1. **Refresh the website** after adding photos
2. **Hover over speaker images** to see LinkedIn overlay
3. **Click LinkedIn icons** to verify profile links open
4. **Check mobile responsiveness** on different screen sizes

## 🔧 Troubleshooting
- **Images not showing?** Check file paths and names
- **LinkedIn not working?** Verify URLs in HTML
- **Layout broken?** Ensure CSS and JS files are loaded
- **404 errors?** Verify photos are in correct directory

## 📝 Notes
- **Alphabetical ordering** ensures consistent organization
- **Consistent naming** makes maintenance easier
- **Fallback placeholders** prevent broken image displays
- **All features work** even without actual photos (using placeholders)

---
**Need help?** Check the terminal for any error messages or refer to the browser console for debugging information.
