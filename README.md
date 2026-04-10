MNDRThe Forgiveness ProtocolA production-grade, interactive apology interface engineered to turn difficult conversations into a sincere and modern resolution experience.Live Demo • Report Bug • Request Feature📖 IntroductionMndr is the spiritual successor to Lovr. While Lovr was designed to express affection, Mndr is built for reconciliation. It uses high-fidelity animations, soft-UI principles, and a playful evasion algorithm to facilitate apologies in the digital age.✨ Key Features🧬 Forgiveness Protocol: A simulated loading sequence designed to set a calm and sincere tone for the interaction.💨 Evasive Evasion: The "No" button dynamically repositions itself on mouseover, making refusal a playful challenge.📈 Dynamic Scale Logic: Every attempt to decline causes the "Yes" button to grow, utilizing psychological reinforcement to encourage resolution.📧 Real-time Webhooks: Integrated with EmailJS to notify the sender instantly once the apology has been accepted.📱 Responsive Glassmorphism: A fully responsive, blur-heavy interface that adapts flawlessly to mobile and desktop viewports.🛠️ Tech StackCore: HTML5, JavaScript (ES6+)Styling: Tailwind CSS 3.0 (JIT Mode)Email: EmailJS (Serverless SMTP)Typography: Dancing Script & Quicksand (Google Fonts)📐 Interaction Architecturegraph TD
    A[User Entry] --> B[https://www.sciencedirect.com/topics/materials-science/parameter-extraction](https://www.sciencedirect.com/topics/materials-science/parameter-extraction)
    B --> C[Protocol Initiation Animation]
    C --> D[Main Interaction Card]
    D --> E{Action}
    E -- Hover No --> F[Coordinate Randomizer]
    F --> G[Yes Button Scale-Up]
    E -- Click Yes --> H[EmailJS Webhook Dispatch]
    H --> I[Success Overlay & Celebration]
🚀 DeploymentClone the repositorygit clone [https://github.com/Zelvior/mndr.git](https://github.com/Zelvior/mndr.git)
Personalize the linkYou can customize the names using GET parameters:https://zelvior.github.io/mndr/?to=RecipientName&from=YourNameConfigure NotificationsUpdate the following constants in index.html:const EMAILJS_PUBLIC_KEY = "your_key";
const EMAILJS_SERVICE_ID = "your_service";
const EMAILJS_TEMPLATE_ID = "your_template";
⚖️ LicenseDistributed under the MIT License. See LICENSE for more information.
