┌─────────────┐   ┌─────────────┐   ┌─────────────┐   ┌─────────────┐
│  Image      │ → │ Preprocess  │ → │ YOLOv8      │ → │ Firebase    │
│  Capture    │   │ (Resize/    │   │ Detection   │   │ (Store      │
│  (Field)    │   │ Augment)    │   │ (mAP75.2%)  │   │ Results)    │
└─────────────┘   └─────────────┘   └─────────────┘   └──────┬──────┘
                                                             ↓
┌─────────────┐   ┌─────────────┐   ┌─────────────────────┐
│  Streamlit  │ ← │ Severity    │ ← │ Farmer Feedback     │
│  UI         │   │ Analysis    │   │ (Improve Model)     │
│  (Real-time)│   │ (Moderate/  │   │                     │
└─────────────┘   │ Severe)     │   └─────────────────────┘
                  └─────────────┘
