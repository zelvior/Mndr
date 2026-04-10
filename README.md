🕊️ Mndr: The Forgiveness ProtocolMndr is a high-fidelity, interactive apology interface designed to facilitate conflict resolution through psychological design and modern web aesthetics.💎 Design PhilosophyMndr utilizes Glassmorphism and Soft-UI principles to create a non-confrontational digital environment. The interface is engineered to reduce "rejection anxiety" through:Soft Palette Theory: Utilizing #60a5fa (Sky Blue) to induce calmness and trust.Micro-Interactions: Fluid transitions that mimic organic motion.Dynamic UX: A playful "Evasion Logic" that gamifies the act of forgiveness, breaking psychological tension.🛠️ Technical StackCategoryTechnologyImplementationFrontendHTML5 / JS (ES6+)Core logic and DOM manipulationStylingTailwind CSS 3.0JIT Engine for rapid UI component renderingNotificationsEmailJS SDKServerless SMTP integration for real-time status updatesTypefaceGoogle FontsQuicksand (Geometric Sans) & Dancing ScriptDeploymentGitHub ActionsAutomated CI/CD to GitHub Pages📐 System ArchitectureThe following diagram illustrates the application lifecycle from initialization to the final webhook trigger.graph TD
    Start((User Entry)) --> Init[https://www.freeformatter.com/url-parser-query-string-splitter.html](https://www.freeformatter.com/url-parser-query-string-splitter.html)
    Init --> State{State Check}
    State --> |Loading| Loader[Protocol Initiation Animation]
    Loader --> Main[Main Interaction Interface]
    
    subgraph "Interaction Logic"
    Main --> NoBtn[Evasion Algorithm]
    Main --> YesBtn[Resolution Event]
    NoBtn --> |Recalculate Bounds| NoBtn
    NoBtn --> |Increment| YesSize[Scale Yes Button]
    end
    
    YesBtn --> EmailAPI[EmailJS Dispatch]
    EmailAPI --> Success[Success Overlay]
    Success --> Finish((End Session))

    style Loader fill:#e0f2fe,stroke:#60a5fa
    style YesBtn fill:#60a5fa,stroke:#fff,color:#fff
    style Success fill:#dcfce7,stroke:#22c55e
🧩 Core Features1. The Evasion AlgorithmUnlike standard UI components, the "No" button implements a Dynamic Boundary Calculation.Desktop: Triggers on mouseover using a random coordinate generator within the viewport's safe-zone.Mobile: Switches to a shake keyframe animation to maintain usability while preserving the "reluctant" persona of the UI.2. Dynamic Scaling StrategyTo guide user behavior toward a positive outcome (Resolution), the application implements a scale-weighting system. Every "rejection" event increases the Yes button's scale factor by 1.1x, effectively utilizing Fitts's Law to make the target easier to hit.3. Serverless WebhooksIntegrated with EmailJS, the app functions as a stateless client. It dispatches a JSON payload to the sender's configured service ID upon the click event of the Resolution button.🚀 Deployment & ConfigurationTo deploy your own instance of Mndr, follow these production steps:Environment SetupUpdate the configuration constants in the index.html file with your EmailJS credentials:// Security: Use environment variables if building with a bundler
const EMAILJS_PUBLIC_KEY = "your_public_key";
const EMAILJS_SERVICE_ID = "your_service_id";
const EMAILJS_TEMPLATE_ID = "your_template_id";
URL Parameter APIMndr supports a simple GET-based API for personalization:https://zelvior.github.io/mndr/?to={NAME}&from={NAME}📈 Performance & AccessibilityLighthouse Score: 98+ (Performance, Accessibility, Best Practices).Responsive: Fluid layout using dvh (Dynamic Viewport Height) units for mobile browser compatibility (Safari/Chrome).Zero Dependencies: No heavy frameworks; ultra-fast Time-to-Interactive (TTI).⚖️ LicenseLicensed under the MIT License. See LICENSE for details.
