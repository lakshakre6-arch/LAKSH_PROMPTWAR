# BlindSpot AI 🧠👁️
> **“Before you decide, see what you might be missing.”**

**BlindSpot AI** is a decision reflection platform built for the hackathon problem statement **“The Blind Spot.”**

---

## 🎯 The Core Problem

People often make major life, career, and financial decisions using only the immediate information in front of them — overlooking unexamined assumptions, competing priorities, second-order risks, and alternative perspectives.

BlindSpot AI illuminates what is hidden without ever nudging, judging, or making the decision for the user.

### 🛡️ Strictly Enforced Neutrality Principle
BlindSpot AI **NEVER** makes the decision for the user. It will never say:
- ❌ *"You should choose X"*
- ❌ *"You should accept this"*
- ❌ *"You should reject this"*
- ❌ *"Do this / Don't do this"*
- ❌ *"Yes, this is the right decision"*

Instead, it functions as an objective, multi-angle analytical mirror that helps users think more deeply and stress-test their own reasoning.

---

## ✨ Features & Architecture

### 1. Landing Page
- Modern dark-mode interface with ambient gradient lighting and glassmorphism.
- Core Problem statement badge and value proposition.
- 4 Feature pillars:
  1. **Uncover Blind Spots**: Find factors you may have overlooked.
  2. **Challenge Assumptions**: Identify beliefs that may need verification.
  3. **See Conflicts**: Discover where your priorities may compete.
  4. **Think Differently**: Explore alternative perspectives.
- Quick 1-click Preset Scenarios for hackathon judging demos.

### 2. Decision Canvas (Input Form)
Structured 5-dimensional input form:
1. *What decision are you considering?*
2. *Describe your situation* (context & constraints)
3. *What matters most to you?* (values & declared priorities)
4. *What are you currently thinking?* (current leaning & rationale)
5. *What concerns you?* (doubts & perceived risks)

### 3. Multi-Stage AI Reasoning Animation
- Smooth animated progression tracking 5 analytical phases:
  - 🔄 *Understanding your situation*
  - 🔄 *Mapping your priorities*
  - 🔄 *Finding overlooked factors*
  - 🔄 *Challenging assumptions*
  - 🔄 *Exploring alternative perspectives*

### 4. Comprehensive 9-Section Analysis Dashboard
1. **Decision Snapshot**: Neutral, concise summary of the dilemma without outcome bias.
2. **Factors You Already Considered**: Categorized cards of factors declared by the user.
3. **Potential Blind Spots (Main Feature)**: Identified overlooked factors with **HIGH / MEDIUM / LOW** severity badges and mitigation guidance.
4. **Hidden Assumptions**: Unverified beliefs separated from facts, with "Why Question It" critique.
5. **Possible Conflicts**: Direct visual mapping of where user's priorities compete with each other.
6. **Questions Worth Asking**: Practical due-diligence questions with interactive exploration checkboxes.
7. **Alternative Perspectives**: 2–4 distinct strategic lenses (e.g. Career Acceleration, Academic Foundation, Risk Mitigation).
8. **Blind Spot Coverage**: Multidimensional completeness audit across 8 key life dimensions (Financial, Time, Well-being, Opportunity Cost, etc.) with Considered/Partially Considered/Unclear statuses.
9. **⚡ Challenge My Thinking**: Large interactive button that launches a dedicated contrarian critique:
   - *What might you be assuming?*
   - *What could someone who disagrees say?*
   - *What evidence would change your thinking?*
   - *What are you possibly underestimating?*

### 5. Dual-Engine Intelligence: Live Gemini + Seamless Demo Mode
- **Live Google Gemini Engine**: Direct integration with Gemini 2.0 / 1.5 Flash models via secure backend proxy.
- **Configurable API Key Modal**: Enter or remove a custom Gemini API key anytime right from the navbar.
- **Dynamic Fallback / Demo Mode**: If no API key is provided or the network is offline, an intelligent contextual fallback engine generates realistic, scenario-tailored analysis so the application never breaks during a live hackathon pitch!

---

## 🚀 Running Locally

### Prerequisites
- Node.js (v18+ or v20+)
- npm

### 1. Start Both Frontend and Backend
```bash
# In the project directory:
npm run dev
```
- **Frontend (Vite HMR)**: `http://localhost:5173`
- **Backend API**: `http://localhost:3001`

### 2. Or Run Standalone Express Server
```bash
# Serves the compiled production frontend and API together:
npm start
```
- **Unified App**: `http://localhost:3001`

### 3. (Optional) Provide Gemini API Key
You can provide your key in three ways:
1. Via `.env` file: `GEMINI_API_KEY=your_key_here`
2. Directly in the web interface by clicking **"Configure Gemini Key"** in the top navbar.
3. Or test in **Demo Mode** without any key needed!

---

## 🛠️ Tech Stack
- **Frontend**: React 18, Vite, Tailwind CSS, Lucide Icons
- **Backend**: Node.js, Express, CORS, Dotenv
- **AI Integration**: Google Gemini Flash API (`gemini-2.0-flash` / `gemini-1.5-flash`)
