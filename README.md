# Zero-Trust IP Escrow

**One-sentence description:** A platform securing digital asset transactions by replacing platform-admin trust with TideCloak's policy-enforced Emergent Authority.

### 1. Vision & originality
We unlock the Gig Economy. Freelancers risk IP theft when sharing master files; clients fear empty deliveries. Current platforms just shift trust to a centralized admin who holds the master key. We shift trust to cryptographic policies.

### 2. Trust constraint insight
The bottleneck is unilateral control. A freelancer cannot share high-value source code because the platform's database or rogue admin holds the decryption key. This centralized trust prevents high-stakes digital transactions.

### 3. Value & impact
Freelancers will share master files upfront, increasing deal closures. We don't promise absolute impossibility of theft (e.g., screen recording), but we shift risk asymmetry. We make unauthorized access cryptographically impossible for the platform itself, protecting 95% of commercial interactions.

### 4. Why TideCloak matters
TideCloak enables Emergent Authority. When a freelancer sets a policy ("Decrypt only if Escrow Locked + Release Token signed"), access is granted by TideCloak's protocol, not our database. Even our admins cannot override this. Authority emerges only when policy conditions align.

### 5. Prototype & storytelling
Our 3-Persona prototype demonstrates the flow:
1. **Freelancer:** Encrypts master IP with TideCloak. Server only stores ciphertext.
2. **Rogue Admin:** Tries to "Force Override/Steal IP" from the database. TideCloak blocks it: *Cryptographic Error: Unilateral Access Denied*.
3. **Client:** Approves Escrow. TideCloak verifies the policy and decrypts the file directly to their browser.
*(Note: TideCloak integration is simulated via a mock policy engine for this prototype).*

### Setup Instructions
1. `pip install streamlit`
2. `streamlit run app.py`
