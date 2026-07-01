# AI Sprint Project Structure Guide

## 📁 Overview

We'll create ONE parent folder `AI-Sprint` under `C:\Pinkal\Learning\AI\` with TWO subfolders:

```
C:\Pinkal\Learning\AI\
├── AISprint/                           ← NEW parent folder (groups everything)
│   ├── References/                     ← Course materials, skills, papers (NOT for GitHub)
│   └── Deliverables/                   ← Your work only (FOR GitHub)
├── github/
├── projects/
└── Teacher Repo/
```

This keeps all AI Sprint materials together and separate from your other AI learning.

### 📝 Naming Convention

**PascalCase** (no dashes, no underscores):
- ✅ `AISprint` - Clean, no build issues
- ✅ `Week1SupervisedLearning` - Readable, Windows-friendly
- ✅ `LinkedInProfile` - Professional
- ❌ `AI-Sprint` - Dashes cause build/ref issues
- ❌ `Week_1_Supervised_Learning` - Underscores verbose
- ❌ `week1supervisedlearning` - Hard to read

**Benefits:**
- No path/build errors
- Easy to read
- Windows + Git friendly
- Professional looking

---

## 🗂️ Detailed Structure

### 📚 References/ (Private - NOT for GitHub)

```
C:\Pinkal\Learning\AI\AISprint\References\
│
├── README.md                                    # Explains this is reference materials
│
├── Week1SkillsAndReferences\
│   ├── Skills\
│   │   ├── SupervisedMLThinkingSkill\           # From AI Engineering OS repo
│   │   ├── UnsupervisedMLThinkingSkill\
│   │   └── AgenticSystemDesignSkill\
│   │
│   └── SessionNotes\
│       ├── SaturdaySessionNotes.md              # Your notes from session
│       ├── SundaySessionNotes.md
│       └── Week1DeliverablesOriginal.docx       # Original PDF/docs from instructor
│
├── Week2SkillsAndReferences\
│   ├── Skills\
│   │   ├── LinkedInProfileOptimizerSkill\
│   │   ├── LinkedInPostGeneratorSkill\
│   │   └── HumanizerSkill\
│   │
│   └── SessionNotes\
│       └── Week2DeliverablesOriginal.docx
│
├── Week3SkillsAndReferences\
│   └── SessionNotes\
│       └── Week3DeliverablesOriginal.docx
│
├── Week4SkillsAndReferences\
│   └── SessionNotes\
│
├── Week5Part1References\
│   ├── Papers\
│   │   ├── GenerativeAgents.pdf                 # Research papers for memory system
│   │   ├── MemGPT.pdf
│   │   ├── MemoryNetworks.pdf
│   │   ├── AttentionIsAllYouNeed.pdf
│   │   ├── RAGPaper.pdf
│   │   └── RETROPaper.pdf
│   │
│   └── EngineeringHandbook.pdf                  # Week 5.1 deliverables handbook
│
├── Week5Part2References\
│   └── CareerPositioningHandbook.pdf            # Week 5.2 deliverables handbook
│
├── CommonResources\
│   ├── DownloadedSkills\
│   │   └── SkillsPackageAll.zip                 # From Google Drive
│   │
│   ├── GitHubRepos\
│   │   ├── AIEngineeringOS\                     # Clone of GitHub repo
│   │   └── LiteracyFrameworks\                  # Clone of GitHub repo
│   │
│   └── ExternalLinks.md                         # All external resources with links
│
└── .gitignore                                    # Ignore everything (this folder NOT a repo)
```

---

### 🎯 Deliverables/ (Public - FOR GitHub)

```
C:\Pinkal\Learning\AI\AISprint\Deliverables\
│
├── .gitignore                                   # Ignore large files, private data
├── README.md                                    # Main project README
│
├── PlanningAndTracking\
│   ├── MyActionPlan.md                         # Your 2-day plan
│   ├── MyProgressTracker.csv                   # Track completion
│   ├── AISprintSummary.md                      # Full reference guide
│   ├── QuickReference.md                       # Table format
│   └── FolderStructureSetup.md                 # This guide
│
├── Templates\                                   # Reusable templates
│   ├── SystemAuditTemplate.md
│   ├── OfferDocumentTemplate.md
│   ├── MasterDocTemplate.md
│   └── ResearchTrackingTemplate.md
│
├── Week1SupervisedUnsupervisedLearning\
│   ├── README.md                               # Week 1 overview and status
│   │
│   ├── Algorithms/
│   │   ├── Logistic_Regression_Analysis.docx   # COPY FROM: my Delivered/week 1/
│   │   ├── Decision_Trees_Analysis.docx        # COPY FROM: my Delivered/week 1/
│   │   ├── XGBoost_Analysis.docx              # COPY FROM: my Delivered/week 1/
│   │   └── [Algorithm_4]_Analysis.md          # Your 4th algorithm (when done)
│   │
│   ├── Thinking_and_Reflection/
│   │   ├── What_I_Think.md                    # COPY FROM: my Delivered/week 1/
│   │   └── Self_Talk.txt                      # COPY FROM: my Delivered/week 1/
│   │
│   ├── Videos/
│   │   ├── Saturday_Loom_Link.md              # Link to video (not the file itself)
│   │   └── Sunday_Loom_Link.md                # Link to video
│   │
│   ├── Content_Extraction/
│   │   ├── Raw_Insights_30-40.md              # When completed
│   │   └── Selected_Content_10-20.md          # When completed
│   │
│   └── Voice_Transcript/
│       ├── Voice_Recording_Link.md             # Link to audio file
│       └── Assembly_AI_Transcript.txt          # The transcript text
│
├── Week_2_Ship_in_Public/
│   ├── README.md                               # Week 2 overview
│   │
│   ├── Master_Doc.md                          # COPY FROM: week Deliverables/Templates/
│   │                                          # (Your daily content engine - IMPORTANT!)
│   │
│   ├── LinkedIn_Profile/
│   │   ├── Before_Profile.png                 # COPY FROM: my Delivered/week 2/
│   │   ├── After_Profile.png                  # COPY FROM: my Delivered/week 2/
│   │   └── Profile_Changes_Log.md             # Document what changed
│   │
│   ├── LinkedIn_Posts/
│   │   ├── Post_1_[Date]_[Topic].md          # Your Week 3 posts (already done)
│   │   ├── Post_2_[Date]_[Topic].md
│   │   ├── Post_3_[Date]_[Topic].md
│   │   ├── Post_4_[Date]_[Topic].md
│   │   └── Post_5_[Date]_[Topic].md
│   │
│   ├── LinkedIn_Comments/
│   │   └── Comments_Log_Week_2.md             # Track your comments
│   │
│   └── Dev_to_Articles/
│       ├── Article_1_[Title]/
│       │   ├── article.md                     # Article content
│       │   └── published_link.md              # Link to published
│       └── Article_2_[Title]/
│           └── article.md
│
├── Week_3_Outreach_and_Audits/
│   ├── README.md
│   │
│   ├── Offer_Document/
│   │   └── My_Offer_Document.md               # COPY FROM: week Deliverables/Templates/
│   │
│   ├── Domain_Research/
│   │   ├── Companies_Research.xlsx            # 20 companies spreadsheet
│   │   ├── Domain_Primer.md                   # Domain knowledge write-up
│   │   └── Workflow_Maps/
│   │       ├── Workflow_1_[Process].md
│   │       ├── Workflow_2_[Process].md
│   │       └── Workflow_3_[Process].md
│   │
│   ├── System_Audits/
│   │   ├── [Company_1]_[Process]_Audit.md    # 15 audits total
│   │   ├── [Company_2]_[Process]_Audit.md
│   │   └── ... (15 total)
│   │
│   ├── Outreach_Campaign/
│   │   ├── Outreach_Messages_Template.md     # Your message templates
│   │   ├── Sent_Messages_Log.csv             # Track who you contacted
│   │   └── Responses_Tracking.md             # Track responses
│   │
│   ├── LinkedIn_Posts/
│   │   └── [5 posts - same format as Week 2]
│   │
│   ├── LinkedIn_Comments/
│   │   └── Comments_Log_Week_3.md
│   │
│   └── Dev_to_Articles/
│       └── [2 articles]
│
├── Week_4_Consistent_Engagement/
│   ├── README.md
│   ├── LinkedIn_Posts/
│   ├── LinkedIn_Comments/
│   └── Dev_to_Articles/
│
├── Week5Part1MemorySystemProject\
│   ├── README.md                              # Project overview
│   │
│   ├── Reconstruction\
│   │   ├── ProblemReconstruction.pdf
│   │   ├── HistoricalTimeline.pdf
│   │   ├── FailureAnalysis.md
│   │   └── FirstPrinciples.md
│   │
│   ├── Research\
│   │   ├── ResearchLandscape.md
│   │   ├── DesignBacklog.md
│   │   ├── Week1\
│   │   │   ├── ComponentScan.md
│   │   │   ├── IdeaEvaluationMatrix.md
│   │   │   ├── DesignOpportunities.pdf
│   │   │   └── ChallengeNotes.md
│   │   └── ReadingNotes\
│   │       ├── GenerativeAgentsNotes.md
│   │       └── [Paper]Notes.md
│   │
│   ├── Design\
│   │   ├── SystemDesign.pdf
│   │   ├── Architecture.pdf
│   │   ├── DataFlow.pdf
│   │   ├── DataModel.md
│   │   ├── APIContracts.md
│   │   ├── ThreatModel.md
│   │   ├── DecisionRecords\
│   │   └── SprintPlan.md
│   │
│   ├── Experiments\
│   │   ├── NaiveBaseline\
│   │   │   ├── src\
│   │   │   └── README.md
│   │   ├── BaselineProtocol.md
│   │   ├── BaselineResults.csv
│   │   ├── ProductiveFailureReport.pdf
│   │   └── ErrorExamples.jsonl
│   │
│   ├── Implementation\
│   │   ├── src\
│   │   │   ├── memory\
│   │   │   ├── retrieval\
│   │   │   └── context\
│   │   ├── tests\
│   │   ├── README.md
│   │   └── requirements.txt
│   │
│   ├── Verification\
│   │   ├── TestPlan.md
│   │   ├── TestResults\
│   │   └── EvaluationDatasets\
│   │
│   ├── Transfer\
│   │   └── TransferStudy.md
│   │
│   ├── Journal\
│   │   ├── DailyLogs\
│   │   │   ├── 2026-07-01.md
│   │   │   └── [date].md
│   │   └── Retrospective.md
│   │
│   └── Genesis\
│       ├── Done.html
│       ├── Plan.md
│       ├── ImplementationNotes.html
│       ├── ContextGraph\
│       ├── Loops\
│       ├── Checkpoints\
│       ├── Wiki\
│       └── Decisions\
│
└── Week5Part2CareerPositioning\
    ├── README.md
    ├── CareerPositioning.pdf
    ├── TargetMarket.md
    ├── MarketResearch.pdf
    ├── OutreachCampaign.md
    ├── DomainPrimer.pdf
    └── Positioning.md
```

---

## 📋 File Mapping - What Gets Copied Where

### From Current Locations → New Deliverables Folder

| Current Location | New Location | Notes |
|------------------|--------------|-------|
| **my Delivered/week 1/** | | |
| `Logistic Regression.docx` | `Week1.../Algorithms/LogisticRegressionAnalysis.docx` | Algorithm work |
| `Decision Trees.docx` | `Week1.../Algorithms/DecisionTreesAnalysis.docx` | Algorithm work |
| `XGBoost.docx` | `Week1.../Algorithms/XGBoostAnalysis.docx` | Algorithm work |
| `What I think.md` | `Week1.../ThinkingAndReflection/WhatIThink.md` | Reflection |
| `self talk.txt` | `Week1.../ThinkingAndReflection/SelfTalk.txt` | Reflection |
| **my Delivered/week 2/** | | |
| `BeforeLinkedIn.png` | `Week2.../LinkedInProfile/BeforeProfile.png` | Profile work |
| `afterLinkedin.png` | `Week2.../LinkedInProfile/AfterProfile.png` | Profile work |
| **week Deliverables/** (all .md files I created) | | |
| `README.md` | `PlanningAndTracking/` + keep as root README | Main guide |
| `My_Action_Plan.md` | `PlanningAndTracking/MyActionPlan.md` | Your plan |
| `My_Progress_Tracker.csv` | `PlanningAndTracking/MyProgressTracker.csv` | Tracker |
| `AI_Sprint_Deliverables_Summary.md` | `PlanningAndTracking/AISprintSummary.md` | Reference |
| `Quick_Reference_Deliverables.md` | `PlanningAndTracking/QuickReference.md` | Quick ref |
| **week Deliverables/Templates/** | | |
| All template files | `Templates/` (root level) | Reusable templates |

---

## 🔒 .gitignore for Deliverables Repo

Create `.gitignore` in `AISprint\Deliverables\`:

```gitignore
# Large media files (link to cloud storage instead)
*.mp4
*.avi
*.mov
*.mp3
*.wav
*.m4a

# Large documents
*.zip
*.rar
*.7z

# Private/sensitive information
*_private.*
*_confidential.*
.env
secrets/
api_keys/

# Temporary files
*.tmp
*~
.DS_Store
Thumbs.db

# IDE files
.vscode/
.idea/
*.swp
*.swo

# Python
__pycache__/
*.pyc
*.pyo
*.pyd
.Python
env/
venv/
*.egg-info/

# Node
node_modules/
npm-debug.log

# OS
.DS_Store
desktop.ini

# Keep these files/folders
!.gitignore
!README.md
```

---

## 📝 Week-level README Template

Each week folder should have a README.md:

```markdown
# Week X - [Week Title]

## Status
- ✅ Completed: [List what's done]
- 🚧 In Progress: [List what you're working on]
- ⏸️ Pending: [List what's not started]

## Deliverables
1. **[Deliverable 1]** - Status: ✅/🚧/⏸️
   - Location: [Folder/file]
   - Notes: [Any relevant notes]

2. **[Deliverable 2]** - Status: ✅/🚧/⏸️
   - Location: [Folder/file]

## Key Learnings
- 
- 

## Links
- Week X original deliverables doc: [in References folder]
- Related skills: [in References folder]

## Submission
- Submitted: [Date]
- Form link: [If applicable]
- Feedback: [When received]
```

---

## 🚀 Implementation Steps

Once you approve this structure, here's what I'll do:

1. **Create folder structure** for both References and Deliverables
2. **Copy files** from existing locations to new structure
3. **Create README files** for each week folder
4. **Create .gitignore** for deliverables repo
5. **Create reference guide** in References folder
6. **Generate PowerShell script** for you to verify everything

After verification, you can:
- Initialize git in `AISprint\Deliverables\`
- Push to GitHub
- Delete/archive the old scattered folders

---

## ❓ Questions to Confirm

1. **Week 3 posts/comments** - You mentioned they're already done. Where are they currently? Should I create placeholder files for them?

2. **Video files** - Since they're large, should I:
   - Create `.md` files with links to where they're stored (YouTube/Loom)?
   - Or keep them locally but exclude from git?

3. **Skills from repo** - Should I:
   - Clone the GitHub repos into References folder?
   - Or just create link files pointing to them?

4. **File naming** - For your algorithm docs, keep as `.docx` or convert/copy as `.md`?

---

**Review this structure and let me know if you want any changes before I create it!**

## 📂 Final Folder Tree Summary

After creation, your `C:\Pinkal\Learning\AI\` will look like:

```
C:\Pinkal\Learning\AI\
│
├── AISprint\                           ← Everything cohort-related here
│   │
│   ├── References\                     ← Private learning materials
│   │   ├── Week1SkillsAndReferences\
│   │   ├── Week2SkillsAndReferences\
│   │   ├── Week3SkillsAndReferences\
│   │   ├── Week4SkillsAndReferences\
│   │   ├── Week5Part1References\
│   │   ├── Week5Part2References\
│   │   ├── CommonResources\
│   │   └── README.md
│   │
│   └── Deliverables\                   ← Git repo for GitHub
│       ├── .git\
│       ├── .gitignore
│       ├── README.md
│       ├── PlanningAndTracking\
│       ├── Templates\
│       ├── Week1SupervisedUnsupervisedLearning\
│       ├── Week2ShipInPublic\
│       ├── Week3OutreachAndAudits\
│       ├── Week4ConsistentEngagement\
│       ├── Week5Part1MemorySystemProject\
│       └── Week5Part2CareerPositioning\
│
├── github\                             ← Your other work
├── projects\
└── Teacher Repo\
```

**Benefits:**
- ✅ All AI-Sprint materials grouped together
- ✅ Clean separation of references vs deliverables
- ✅ Easy to push Deliverables to GitHub (one repo)
- ✅ References stay private and local
- ✅ Doesn't mix with your other AI learning

