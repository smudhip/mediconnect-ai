# 🏥 MediConnect AI: Preventing Dangerous Missed Diagnoses

[![Demo](https://img.shields.io/badge/Demo-Live-brightgreen)](https://smudhip.github.io/mediconnect-ai/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![AWS](https://img.shields.io/badge/AWS-Deployed-orange.svg)](https://aws.amazon.com)

> **Intelligent health pattern analysis that saves lives by connecting symptoms across medical specialties**

## 🚨 The Problem We Solve

**67-year-old woman almost dies from missed heart failure diagnosis**
- Doctors focus only on knee surgery for 3 months
- Dismiss leg swelling as "normal aging" 
- Ignore previous cardiac history
- Pre-surgery tests reveal severe heart failure and blocked arteries
- **Result: 3-month delay, life-threatening condition, unnecessary surgical risk**

**This happens thousands of times daily in healthcare worldwide.**

## ✨ Our Solution

**MediConnect AI** analyzes health patterns comprehensively across multiple medical conditions:

### Key Features
- **Multi-Condition Analysis**: Kidney disease, thyroid disorders, diabetes, cardiac conditions
- **Pattern Recognition**: Identifies dangerous symptom combinations
- **Risk Assessment**: Calculates risk levels with confidence scores
- **Family Communication**: Translates medical findings into understandable language
- **Interaction Detection**: Finds critical drug and condition interactions
- **Evidence-Based**: Uses medical guidelines and best practices

## 🎬 Live Demo

### Try the Demo
**🔗 [Launch Demo](https://smudhip.github.io/mediconnect-ai/)**

No installation required - works directly in your browser!

### What You'll See
- Interactive patient data input
- Real-time multi-agent analysis
- Pattern recognition results
- Risk assessment with confidence scores
- Family-friendly medical explanations
- Condition-specific warning signs

## 🏗️ Architecture

```
┌─────────────────┐
│   Web Browser   │  (GitHub Pages)
│   HTML + JS     │
└────────┬────────┘
         │ HTTPS
         ▼
┌─────────────────┐
│  API Gateway    │  (AWS)
│  REST API       │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Lambda         │  (Python 3.11)
│  Analysis Logic │
└─────────────────┘
```

**Technology Stack:**
- **Frontend**: HTML5, JavaScript (Vanilla)
- **Backend**: AWS Lambda (Python 3.11)
- **API**: AWS API Gateway (REST)
- **Hosting**: GitHub Pages
- **Infrastructure**: CloudFormation (IaC)

## 📦 What's Included

### Demo Bundle
- `agentic-medical-interface.html` - Interactive web demo
- Works offline with local fallback mode
- Connects to AWS backend when online

### Deployment Bundle
- `cloudformation-template.yaml` - Complete AWS infrastructure
- `deploy.sh` - Automated deployment script
- `lambda-function.py` - Backend analysis logic
- `cleanup.sh` - Resource cleanup script

## 🚀 Quick Start

### Option 1: Use Live Demo
Just visit: **[https://smudhip.github.io/mediconnect-ai/](https://smudhip.github.io/mediconnect-ai/)**

### Option 2: Run Locally
```bash
# Download the demo
curl -O https://raw.githubusercontent.com/smudhip/mediconnect-ai/main/index.html

# Open in browser
open index.html
```

### Option 3: Deploy Your Own
```bash
# Clone repository
git clone https://github.com/smudhip/mediconnect-ai.git
cd mediconnect-ai

# Deploy AWS backend
cd mediconnect-deployment-bundle
./deploy.sh

# Update HTML with your API endpoint
# Then host on GitHub Pages or any web server
```

## 🎯 Use Cases

### For Families
- **Elderly Care**: Monitor aging parents' health patterns
- **Chronic Conditions**: Track disease progression
- **Medical Visits**: Prepare informed questions for doctors
- **Emergency Prevention**: Early warning signs detection

### For Healthcare Providers  
- **Decision Support**: Evidence-based recommendations
- **Risk Assessment**: Surgical and treatment risk evaluation
- **Care Coordination**: Multi-specialty communication
- **Quality Improvement**: Diagnostic accuracy enhancement

## 📊 Medical Conditions Analyzed

✅ **Kidney Disease**
- Chronic kidney disease monitoring
- Medication dose adjustments
- Electrolyte management
- Dialysis considerations

✅ **Thyroid Disorders**
- Hypothyroidism/Hyperthyroidism
- Medication monitoring
- Metabolic effects
- Cardiac interactions

✅ **Diabetes**
- Blood sugar control
- Complication screening
- Diabetic nephropathy
- Cardiovascular risk

✅ **Cardiac Conditions**
- Heart failure
- Coronary artery disease
- Arrhythmias
- Surgical risk assessment

✅ **Multi-Condition Interactions**
- Kidney-thyroid interactions
- Diabetes-kidney complications
- Polypharmacy risks
- Treatment contraindications

## 💰 Cost

**Demo**: FREE (GitHub Pages hosting)

**AWS Backend** (if you deploy your own):
- Lambda: ~$0.20/month
- API Gateway: ~$0.35/month
- CloudWatch: ~$0.50/month
- **Total: ~$1/month** (Free tier eligible)

## 🔒 Security & Privacy

- ✅ HTTPS only (TLS 1.2+)
- ✅ No data storage (stateless)
- ✅ No authentication required (public demo)
- ✅ CORS enabled for web access
- ✅ CloudWatch logging for monitoring
- ⚠️ **Note**: This is a demo - not HIPAA compliant

## 📋 API Documentation

### Endpoint
```
POST https://ao8njk7pvh.execute-api.us-east-1.amazonaws.com/prod/analyze
```

### Request
```json
{
  "patient_data": {
    "medical_conditions": [
      {"condition": "Chronic Kidney Disease"}
    ],
    "medical_history": ["diabetes_history"],
    "current_symptoms": "fatigue, swelling"
  }
}
```

### Response
```json
{
  "patterns": [...],
  "alerts": [...],
  "recommendations": [...],
  "risk_level": "HIGH",
  "confidence": 92
}
```

## 🛣️ Roadmap

- [x] Multi-condition analysis
- [x] AWS serverless deployment
- [x] GitHub Pages hosting
- [ ] Mobile app
- [ ] EHR integration
- [ ] Real AI/ML models (currently rule-based)
- [ ] HIPAA compliance
- [ ] Multi-language support

## 👥 Contributing

This is a demonstration project. For production use:
1. Add authentication
2. Implement HIPAA compliance
3. Add real AI/ML models
4. Integrate with EHR systems
5. Add comprehensive testing

## 📄 License

MIT License - See [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Medical advisors for clinical guidance
- Healthcare providers for real-world insights  
- Families affected by diagnostic delays
- AWS for cloud infrastructure

## 📞 Contact

- **Demo**: [https://smudhip.github.io/mediconnect-ai/](https://smudhip.github.io/mediconnect-ai/)
- **Code**: [https://code.aws.dev/personal_projects/alias_s/smudhip/mediconnect-ai](https://code.aws.dev/personal_projects/alias_s/smudhip/mediconnect-ai)

---

**⭐ Star this repo if MediConnect AI could help save lives in healthcare!**

*Built with ❤️ to prevent dangerous missed diagnoses and empower families*
