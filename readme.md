# Delirium Management Flowchart

This is the DREAM protocol decision-making tree in Mermaid.

```mermaid
flowchart TD
    A[Hospital Admission (≥18 yrs)] --> B[Identify At-Risk Patients<br/>(≥65, cognitive impairment, severe illness, surgery)]
    B --> C[Implement Prevention & Screening<br/>(orientation, mobilization, sleep hygiene, hydration, nutrition)]
    C --> D{Delirium Screen Positive?<br/>CAM/CAM-ICU: Features 1+2 + (3 or 4)<br/>4AT ≥4}
    D -- No --> C
    D -- Yes --> E[Initial Assessment]
    E --> F[IM Physician: Hx, PE, Med Review<br/>APN: Collateral Hx, Educate Family]
    F --> G{Patient ≥75 yrs?}
    G -- Yes --> G1[Refer to Geriatrics Team] --> H[Diagnostic Workup]
    G -- No --> H[Diagnostic Workup]
    H --> H1[Investigations via DELIRIUM Mnemonic<br/>Drugs, Electrolytes, Liver/Lung, Infection, Retention, Intracranial, Uremia, Metabolic]
    H1 --> I{Neurology Referral Indicated?<br/>(Focal deficits, seizures, abnormal CT, delirium >48h, CNS infection, neuro history)}
    I -- Yes --> I1[Consult Neurology] --> J{Psychiatry Referral Indicated?}
    I -- No --> J{Psychiatry Referral Indicated?}
    J -- Yes --> J1[Consult Psychiatry] --> K{Geriatrics Referral Indicated?<br/>(≥75 yrs, polypharmacy, frailty, CI, sensory deficits, comorbidities)}
    J -- No --> K{Geriatrics Referral Indicated?}
    K -- Yes --> K1[Consult Geriatrics] --> L[Management]
    K -- No --> L[Management]
    L --> L1[Non-Pharmacological:<br/>Environment, Supportive care, Sleep hygiene]
    L --> L2[Pharmacological:<br/>Treat underlying cause, Symptom management per protocol]
    L --> L3[Involve Specialists: Neurology, Psychiatry, Geriatrics]
    L --> M[Monitor Patient<br/>Daily CAM/CAM-ICU/4AT, vitals, safety]
    M --> N{Delirium Resolved?}
    N -- No --> M
    N -- Yes --> O[Discharge Planning]
    O --> O1[Educate Patient & Family<br/>(Appendix D)]
    O --> O2[Arrange Follow-Up:<br/>Primary Care, Neurology, Psychiatry, Geriatrics]
    O --> O3[Provide Written Summary of DREAM Plan]
    O --> P[Discharge Patient]
