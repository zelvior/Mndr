🕊️ Mndr — The Forgiveness ProtocolMndr is a lightweight, interactive "Apology-as-a-Service" web application. Built to follow the design language of its predecessor Lovr, it transforms the difficult act of saying "I'm sorry" into a sincere, engaging, and modern digital experience.🔗 Live DemoExperience the application here:👉 https://zelvior.github.io/mndrPersonalize your apology:Add parameters to the URL to customize the names:https://zelvior.github.io/mndr/?to=Bestie&from=Zelvior📸 OverviewMndr uses a glassmorphism UI, fluid animations, and a playful "No" button logic to ease the tension during an apology. Once the recipient clicks "Yes," an automated confirmation is sent to the sender via EmailJS.Key FeaturesDynamic Personalization: Pass names via URL parameters (?to=Name&from=Name).Forgiveness Protocol: A simulated "scanning" state to build anticipation and sincerity.Evasive "No" Button: A playful mechanism where the "No" button escapes the cursor on desktop (and shakes on mobile).Persistent Growth: The "Yes" button grows larger every time the "No" button is interacted with.Instant Notification: Real-time email alerts via EmailJS when the apology is accepted.🛠️ Tech Stack & Architecturegraph TD
    A[User Opens URL] --> B{URL Params?}
    B -- Yes --> C[Display Custom Names]
    B -- No --> D[Display Default Names]
    C --> E[Forgiveness Protocol Init]
    D --> E
    E --> F[Main Apology Card]
    F --> G{Decision}
    G -- Hover/Click No --> H[Button Escapes / Yes Grows]
    G -- Click Yes --> I[Trigger EmailJS API]
    I --> J[Success Celebration Card]
    J --> K[Confetti & Sparkles]
ComponentTechnologyRoleStylingTailwind CSSUtility-first responsive designTypographyGoogle FontsDancing Script & QuicksandLogicVanilla JavaScriptState management & DOM manipulationBackendEmailJSServerless email deliveryEffectsCSS KeyframesFloating elements & Glassmorphism🚀 Getting Started1. InstallationClone the repository to your local machine:git clone [https://github.com/zelvior/mndr.git](https://github.com/zelvior/mndr.git)
cd mndr
2. ConfigurationOpen index.html and update the EmailJS credentials with your own to receive notifications:const EMAILJS_PUBLIC_KEY = "YOUR_PUBLIC_KEY";
const EMAILJS_SERVICE_ID = "YOUR_SERVICE_ID";
const EMAILJS_TEMPLATE_ID = "YOUR_TEMPLATE_ID";
3. DeploymentThis project is ready for GitHub Pages. Simply go to your Repository Settings > Pages and select the main branch to host your own version.📊 Interaction FlowUser ActionUI ResponseOutcomePage LoadBlue Progress BarCalms the user and sets the stageHover "No"Button jumps to random X/YSoftens the tension with humorClick "No"Message cycles (e.g., "Think again! 🥺")Emotional appeal for a second chanceClick "Yes"Celebration animationFull resolution and psychological closure📜 LicenseDistributed under the MIT License.
