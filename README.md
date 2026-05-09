# Scyther Formal Verification Model-- Authchain_V2X: Verification-Driven Trust and Blockchain-Assisted Authentication for Secure V2X Networks

This repository contains the SPDL implementation and formal verification artefacts for the proposed **AuthChain-V2X** authentication and key agreement protocol designed for secure Vehicle-to-Everything (V2X) communication environments.

The protocol integrates blockchain-assisted session establishment, mutual authentication, ephemeral exchange, and session-key protected communication. Formal verification is performed using the **Scyther** security protocol verification tool under the Dolev–Yao adversarial model.

---

## Repository Contents

| File / Folder | Description |
|---|---|
| `AuthChain_V2X.spdl` | Main SPDL implementation of the protocol |
| `settings/scyther_settings.txt/` | Scyther settings to run the protocol |
| `results/scyther_output.txt` | Raw Scyther verification results |
| `results/verification_summary.txt` | Summary of verified security claims |
| `settings/scyther_settings.jpg/` | Screenshots of Scyther settings |
| `results/V2X output.jpg/` | Screenshots of Scyther verification output |
| `figures/conceptual_workflow.jpg` | Conceptual workflow of the protocol |

---

## Protocol Overview

The proposed protocol consists of three participating entities:

- **X1** : V2X Node 1
- **X2** : V2X Node 2
- **BC** : Blockchain-assisted coordination service

The protocol operates in the following phases:

1. Blockchain-assisted authentication
2. Secure session key establishment
3. Ephemeral parameter exchange
4. Mutual confirmation and synchronisation
5. Session-key protected communication

---

## Verified Security Properties

The following security properties are verified using Scyther:

- Aliveness
- Weak Agreement
- Non-injective Agreement
- Non-injective Synchronisation
- Running and Commit Claims
- Session Key Secrecy

---

## Verification Tool

Formal verification was conducted using:

- **Tool:** Scyther
- **Model:** Dolev–Yao adversary model

Official Scyther website:

https://people.cispa.io/cas.cremers/scyther/

---

## Running the Verification

### Step 1: Install Scyther

Download and install Scyther from the official website.

### Step 2: Open the Protocol File

Open the following file inside Scyther:

```text
AuthChain_V2X.spdl
```

### Step 3: Execute Verification

Run protocol verification using the suggested Scyther settings.

---

## Expected Verification Outcome

The protocol successfully verifies:

- Mutual authentication
- Synchronisation
- Agreement properties
- Session-key confidentiality

without any attack traces under the analysed threat model.

---

## License

This repository is shared for academic and research purposes.
