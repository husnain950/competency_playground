
# 🎯 Software Engineer Competency Assessment

A comprehensive, interactive web-based assessment tool for evaluating software engineering competencies across technical execution, communication, teamwork, and maturity domains.

## ✨ Features

### 🚀 **Smart Scoring System**
- **Weighted competency levels** (1-5 points per question)
- **Individual question weightages** based on importance
- **Percentage-based scoring** (0-100%)
- **Excludes non-applicable responses** from calculation

### 📊 **Progressive Competency Levels**
- **Beginner (B1-B3)**: 26% - 39%
- **Competent (C1-C3)**: 45% - 60%
- **Very Competent (VC1-VC3)**: 65% - 76%
- **Super Competent (SC1-SC3)**: 79% - 87%
- **Ridiculously Competent (RC)**: 100%

### 🎨 **Interactive UI**
- **Real-time progress tracking** with color-coded bars
- **Sticky sub-level progress** for focused feedback
- **Milestone markers** showing advancement thresholds
- **Mobile-responsive design**
- **Smooth animations** and transitions

### 📋 **Comprehensive Assessment Areas**

#### **Technical Execution** (12 Questions)
- Breadth & Depth of Experience
- Code Architecture & Project Delivery
- Mobile Development (if applicable)
- Testing, Code Management & Clean Code
- Problem Solving & Workflow Maturity

#### **Communication** (4 Questions)
- Effective Writing & Speaking
- Responsiveness & Comprehension

#### **Teamwork** (2 Questions)
- Dependability & Collaboration

#### **Maturity** (6 Questions)
- Commitment & Feedback Openness
- Initiative & Mentorship
- Continuous Learning & Self-Discipline


## 📊 How It Works

### **Scoring Logic**
```
Final Score = (Sum of weighted competency scores) / (Sum of applicable weightages) × 100
```

### **Question Weightages**
- **High Impact** (5.225): Core technical skills (Architecture, Problem Solving, etc.)
- **Medium Impact** (4.0): Important skills (Communication, Code Management, etc.)
- **Lower Impact** (3.0): Supporting skills (Writing, Testing, etc.)
- **Specialized** (2.0): Mentorship & succession planning

### **Competency Levels per Question**
- **Level 1**: Basic understanding/capability
- **Level 2**: Intermediate proficiency
- **Level 3**: Advanced competency
- **Level 4**: Expert-level mastery *(Default selection)*
- **Level 5**: Industry-recognized expertise

### **Special Responses**
- **"Not applicable to current role"**: Excluded from scoring
- **"I don't know"**: Excluded from scoring

## 🎯 Default Configuration

- **All questions pre-selected** to Level 1 (Expert competency)
- **Starting score**: ~20% (Super Competent SC1)
- **24 total questions** across 4 competency areas
- **Users adjust down/up** based on actual capabilities

## 📱 Technical Details

### **Built With**
- **React 18** (via CDN)
- **Tailwind CSS** (via CDN)
- **Vanilla JavaScript** (ES6+)
- **No build process required**

### **Browser Support**
- ✅ Chrome/Edge (Chromium)
- ✅ Firefox
- ✅ Safari
- ✅ Mobile browsers

### **File Structure**
```
competency-assessment.html     # Single standalone file
├── React components          # Embedded JavaScript
├── Tailwind CSS             # CDN-loaded styling
├── Question data            # 24 competency questions
└── Scoring logic            # Weighted percentage calculation
```

## 🔧 Customization

### **Adding New Questions**
1. Add to `competencyData` object
2. Define weightage in `weightages` object
3. Follow existing option structure

### **Modifying Competency Levels**
Update the `competencyLevels` object with new thresholds:
```javascript
"3": {
    "sub_levels": [65.0, 70.0, 76.0],
    "min_score": 76.0,
    "tooltip": "VC",
    "name": "Very Competent",
    "color": "bg-blue-500"
}
```

### **Changing Default Selections**
Modify the initialization in `useEffect`:
```javascript
defaultResponses[question.id] = 2; // Sets Level 3 as default
```

## 📈 Use Cases

### **Individual Assessment**
- **Self-evaluation** of technical and soft skills
- **Career development** planning
- **Skill gap identification**

### **Team Management**
- **Competency mapping** across team members
- **Promotion readiness** evaluation
- **Training needs** assessment

### **Hiring Process**
- **Candidate evaluation** during interviews
- **Skill verification** for role fit
- **Onboarding assessment** for new hires

### **Organizational Development**
- **Team capability** overview
- **Skills inventory** management
- **Professional development** tracking

## 🎨 Visual Highlights

- **Color-coded progress bars** that change with competency level
- **Milestone achievement** indicators
- **Sub-level progression** tracking (e.g., VC1 → VC2 → VC3)
- **Next milestone targeting** with specific point requirements
- **Responsive design** that works on all devices

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page or submit pull requests.

## 📞 Support

If you have questions or need assistance:
- Review the assessment logic in the source code
- Check browser console for any errors
- Ensure you're using a modern browser with JavaScript enabled

---

**Ready to assess your competency?** Simply open the HTML file and start your evaluation journey! 🚀