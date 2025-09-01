# 🎨 Custom Logo Instructions

## 📋 How to Add Your Custom Logo

### **Step 1: Create Your Logo**
- Design your logo in any format (PNG, SVG, JPG recommended)
- Recommended size: **200x200 pixels** or larger
- Keep file size under **1MB** for optimal loading

### **Step 2: Upload to GitHub**
1. Go to your profile repository: https://github.com/BoozeLee/BoozeLee
2. Click **"Add file"** → **"Upload files"**
3. Drag and drop your logo file
4. Name it something like `logo.png` or `logo.svg`
5. Commit the file

### **Step 3: Update the README**
Replace this line in `README.md`:
```markdown
<img src="https://via.placeholder.com/200x200/6366F1/FFFFFF?text=LOGO" alt="Custom Logo Placeholder" width="200" height="200" />
```

With your actual logo:
```markdown
<img src="https://github.com/BoozeLee/BoozeLee/blob/master/logo.png" alt="BoozeLee Logo" width="200" height="200" />
```

### **Step 4: Alternative - Use GitHub Raw URL**
For better performance, use the raw GitHub URL:
```markdown
<img src="https://raw.githubusercontent.com/BoozeLee/BoozeLee/master/logo.png" alt="BoozeLee Logo" width="200" height="200" />
```

## 🎯 Logo Design Tips

### **Recommended Styles**
- **Minimalist**: Clean, simple designs work best
- **Professional**: Reflects your AI/tech expertise
- **Scalable**: Should look good at different sizes
- **Brand Colors**: Use your profile's color scheme (#6366F1)

### **File Formats**
- **SVG**: Best for logos (scalable, small file size)
- **PNG**: Good for complex designs with transparency
- **JPG**: Use only if no transparency needed

### **Size Guidelines**
- **Profile Display**: 200x200px minimum
- **High Resolution**: 400x400px or larger for crisp display
- **Aspect Ratio**: Square (1:1) works best

## 🔧 Technical Details

### **GitHub Profile Repository**
- **Repository Name**: `BoozeLee` (must match your username exactly)
- **Visibility**: Public
- **Branch**: `master` or `main`
- **File Location**: Root directory

### **Markdown Image Syntax**
```markdown
![Alt Text](image-url)
<img src="image-url" alt="Alt Text" width="200" height="200" />
```

## 🚀 Quick Setup Commands

If you want to update the logo programmatically:

```bash
# Navigate to your profile repo
cd ~/.github

# Add your logo file
git add logo.png

# Commit and push
git commit -m "Add custom logo"
git push origin master
```

## 📱 Mobile Optimization

### **Responsive Design**
Consider adding responsive image sizing:
```markdown
<img src="your-logo-url" alt="BoozeLee Logo" width="200" height="200" style="max-width: 100%; height: auto;" />
```

### **Dark/Light Mode**
You can create different versions for different themes:
```markdown
<img src="logo-dark.png" alt="BoozeLee Logo" width="200" height="200" />
```

## 🎨 Color Palette Reference

Your profile uses these colors:
- **Primary**: #6366F1 (Indigo)
- **Success**: #00FF00 (Green)
- **Warning**: #FF6B6B (Red)
- **Info**: #00FFFF (Cyan)
- **Background**: #0D1117 (Dark)

## 📞 Need Help?

If you need assistance with:
- Logo design recommendations
- Technical implementation
- GitHub repository setup
- Markdown formatting

Feel free to reach out! Your custom logo will make your profile truly unique and professional! 🎨✨
