# Delirium Management Flowchart

```mermaid
flowchart TD
    A[Hospital Admission >=18 yrs] --> B[Identify At-Risk Patients: age >=65, cognitive impairment, severe illness, surgery]
    B --> C[Implement Prevention and Screening: orientation, mobilization, sleep hygiene, hydration, nutrition]
    C --> D{Delirium Screen Positive? CAM/CAM-ICU (Features 1+2 + (3 or 4)) OR 4AT >=4}
    D -- No --> C
    D -- Yes --> E[Initial Assessment]
    E --> F[IM Physician: history, physical exam, medication review; APN: collateral history, educate family]
    F --> G{Patient age >=75 yrs?}
    G -- Yes --> G1[Refer to Geriatrics Team] --> H[Diagnostic Workup]
    G -- No --> H[Diagnostic Workup]
    H --> H1[Investigations via DELIRIUM Mnemonic: Drugs, Electrolytes, Liver/Lung, Infection, Retention, Intracranial, Uremia, Metabolic]
    H1 --> I{Neurology Referral Indicated? focal deficits, seizures, abnormal CT, delirium >48h, CNS infection, neurological history}
    I -- Yes --> I1[Consult Neurology] --> J{Psychiatry Referral Indicated?}
    I -- No --> J{Psychiatry Referral Indicated?}
    J -- Yes --> J1[Consult Psychiatry] --> K{Geriatrics Referral Indicated? age >=75, polypharmacy, frailty, cognitive impairment, sensory deficits, comorbidities}
    J -- No --> K{Geriatrics Referral Indicated?}
    K -- Yes --> K1[Consult Geriatrics] --> L[Management]
    K -- No --> L[Management]
    L --> L1[Non-Pharmacological: environment, supportive care, sleep hygiene]
    L --> L2[Pharmacological: treat underlying cause, symptom management per protocol]
    L --> L3[Involve Specialists: Neurology, Psychiatry, Geriatrics]
    L --> M[Monitor Patient: daily CAM/CAM-ICU/4AT, vitals, safety]
    M --> N{Delirium Resolved?}
    N -- No --> M
    N -- Yes --> O[Discharge Planning]
    O --> O1[Educate Patient and Family]
    O --> O2[Arrange Follow-Up: primary care, neurology, psychiatry, geriatrics]
    O --> O3[Provide Written Summary of DREAM Plan]
    O --> P[Discharge Patient]
