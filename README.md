**Artsoot** is a full-stack, video-based art auction platform designed to bridge the gap between artists and art buyers through an immersive, media-rich digital experience.

Artists can upload artwork images and videos, create timed auctions, and receive bids from verified buyers — while the platform manages the entire auction lifecycle from listing creation and live bidding through to final payment processing with automated commission logic built in.

**Architecture & Backend**
The platform is built on a decoupled architecture, with a Node.js/Express REST API serving as the backbone. Data is managed through MySQL using Sequelize ORM, ensuring structured, relational data handling for users, listings, bids, and transactions. Authentication is handled via JWT, providing secure, stateless session management across all API interactions. Media assets — artwork images and videos — are stored and served through AWS S3, enabling scalable, reliable cloud-based file management without burdening the core server.

**Frontend**
The client-side is a React 18 Single Page Application (SPA) built for speed and responsiveness. State management is handled by Redux with Redux Saga managing asynchronous side effects such as auction timers, bid updates, and payment flows. Users can authenticate quickly via Google and Facebook OAuth, reducing friction at onboarding. The UI is designed to be elegant and media-forward, putting artwork visuals at the center of the experience.

**Payments & Commerce**
Artsoot integrates both PayPal REST API and Stripe to support flexible payment options for buyers. The platform includes automated commission logic that calculates and splits payments between the artist and the platform upon auction completion — removing any manual reconciliation work.

**Key Highlights**
- Timed auction engine with real-time bidding
- Secure video/image uploads via AWS S3
- Dual payment gateway support (PayPal + Stripe)
- Social login via Google & Facebook OAuth
- Automated commission processing
- Fully decoupled frontend/backend architecture

Artsoot combines the excitement of live auctions with the richness of video-based art discovery — making it a compelling platform for both emerging and established artists to reach serious buyers globally.
