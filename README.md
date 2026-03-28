# Job-Finder
A web agent copilot that discovers jobs, explains fit, tailors resumes, and assists students through real application workflows.




┌──────────────────────────────────────────────────────────────┐
│                        Frontend Web App                     │
│  Next.js / React                                            │
│  - Chatbox Onboarding                                       │
│  - Job Search Dashboard                                     │
│  - Resume Viewer / Editor                                   │
│  - Application Tracker                                      │
└──────────────────────────────────────────────────────────────┘
                             │
                             ▼
┌──────────────────────────────────────────────────────────────┐
│                        Backend API Layer                    │
│                    FastAPI / Next API Routes                │
│  - Auth API                                                 │
│  - Profile API                                              │
│  - Job Search API                                           │
│  - Resume API                                               │
│  - Application API                                          │
│  - Tracking API                                             │
└──────────────────────────────────────────────────────────────┘
                             │
        ┌────────────────────┼────────────────────┐
        ▼                    ▼                    ▼
┌───────────────┐   ┌──────────────────┐   ┌──────────────────┐
│ LLM Orchestrator │ │ TinyFish Agent   │   │ Workflow Engine   │
│ - chat reasoning │ │ Service          │   │ - async tasks     │
│ - profile parse  │ │ - web navigation │   │ - retries         │
│ - JD parse       │ │ - page scraping  │   │ - state machine   │
│ - resume tailor  │ │ - form filling   │   │ - scheduling      │
└───────────────┘   └──────────────────┘   └──────────────────┘
        │                    │                    │
        └────────────────────┼────────────────────┘
                             ▼
┌──────────────────────────────────────────────────────────────┐
│                        Data Layer                           │
│  PostgreSQL                                                 │
│  Redis                                                      │
│  Object Storage (S3 / Supabase Storage / Cloudinary)        │
│  Vector Store (pgvector / Pinecone / Weaviate optional)     │
└──────────────────────────────────────────────────────────────┘
                             │
                             ▼
┌──────────────────────────────────────────────────────────────┐
│                  External Platforms / Integrations          │
│  - LinkedIn / Indeed / Greenhouse / Lever / Workday         │
│  - Email notifications                                      │
│  - PDF / DOCX rendering                                     │
│  - Authentication provider                                  │
└──────────────────────────────────────────────────────────────┘
