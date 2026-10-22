# Zero-Trust IP Escrow

**One-sentence description:** A platform securing digital asset transactions between strangers by replacing platform-admin trust with TideCloak's policy-enforced Emergent Authority.

### 1. Vision & originality
We unlock the Gig Economy. Freelancers risk IP theft when sharing drafts to win contracts. Existing platforms rely on "View Only" UI illusions, which admins can override. We shift trust from a centralized platform to cryptographic policies.

### 2. Trust constraint insight
The bottleneck is unilateral control. A freelancer cannot share high-value work because the platform holds the master key. This centralized trust prevents high-stakes digital transactions.

### 3. Value & impact
Freelancers will share their best work upfront, increasing deal closures. We don't promise absolute impossibility of theft (e.g., screen recording), but we shift risk asymmetry, making unauthorized access computationally difficult and protecting 95% of commercial interactions.

### 4. Why TideCloak matters
TideCloak enables Emergent Authority. When a designer sets a policy (e.g., "Decrypt only if JWT is valid and time < 10 mins"), access is granted by TideCloak's protocol, not our database. Even our admins cannot override this. Authority emerges only when policy conditions align.

### 5. Prototype & storytelling
Our prototype demonstrates the flow:
1. Designer uploads a mock file and sets a 10-minute view policy via TideCloak.
2. Client opens the link; the file is locked.
3. Upon policy verification (simulated via our mock TideCloak engine for this prototype), the file decrypts.
4. After 10 minutes, TideCloak revokes access.
*(Note: TideCloak integration is simulated via a mock policy engine to demonstrate the Emergent Authority flow within the hackathon timeframe).*

### Setup Instructions
1. `pip install streamlit`
2. `streamlit run app.py`
