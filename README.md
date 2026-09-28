# Hi, I'm Ivan

Frontend Developer with 5 years of experience building web and mobile applications (telemedicine, govtech, fintech, social). Focused on real-time systems (WebSocket, WebRTC), rendering performance, feature-sliced architecture and testability. Currently moving toward LLM pipelines, AI automation and end-to-end product engineering.

### Core Tech Stack
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) ![Next.js](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white) ![React Native](https://img.shields.io/badge/react%20native-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![Expo](https://img.shields.io/badge/expo-1C1E24?style=for-the-badge&logo=expo&logoColor=white) ![Redux](https://img.shields.io/badge/redux-%23593d88.svg?style=for-the-badge&logo=redux&logoColor=white) ![Zustand](https://img.shields.io/badge/zustand-433E38?style=for-the-badge)

### Styling & UI
![SCSS](https://img.shields.io/badge/SCSS-hotpink?style=for-the-badge&logo=SASS&logoColor=white) ![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white) ![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)

### Instruments & Technologies
![Zod](https://img.shields.io/badge/zod-%233068b7.svg?style=for-the-badge&logo=zod&logoColor=white) ![WebRTC](https://img.shields.io/badge/WebRTC-black?style=for-the-badge&logo=webrtc&logoColor=white) ![WebSocket](https://img.shields.io/badge/WebSocket-red?style=for-the-badge&logo=socketdotio&logoColor=white) ![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white) ![Jest](https://img.shields.io/badge/-jest-%23C21325?style=for-the-badge&logo=jest&logoColor=white) ![Cypress](https://img.shields.io/badge/-cypress-%23E5E5E5?style=for-the-badge&logo=cypress&logoColor=058a5e) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

---

### Key Achievements (Work Experience)

**Telemedicine platform (Nov 2024 - present)** - sole owner of the real-time layer in a three-person frontend team

* **WebRTC calling**: Built 1:1 calls from scratch on native `RTCPeerConnection` with no SDK: custom WebSocket signalling, SDP/ICE serialisation, a deferred ICE-candidate queue that eliminated negotiation races, TURN config refreshed at runtime.
* **Call reliability**: Cut dropped calls by 15% by tracing failures to public relay infrastructure, making the case for dedicated TURN, and rebuilding the connection flow around backend-issued credentials and ICE restart.
* **WS architecture**: Re-architected a 2,000-line WebSocket monolith into 13 feature-sliced modules with a hard boundary between socket transport and state mutation. New message types now ship from established handler/sender patterns.
* **Performance**: Reduced chat re-renders by ~60% (React Profiler baseline): granular Zustand selectors, splice-based updates preserving referential equality, `react-window` virtualisation, portal-rendered context menus, memoised rich-text editor. Conversations of 3,000+ messages scroll smoothly with full history kept.
* **Testing**: Took the codebase from zero to 146 Jest unit tests and 54 Cypress E2E tests; built a mock WebSocket server that made reconnect, delivery and presence scenarios deterministic.
* **Security**: Implemented client-side AES-256-GCM encryption on the native Web Crypto API with per-conversation symmetric keys for medical message data.
* **UI Kit**: Consolidated 30+ legacy components into a shared UI Kit adopted by the messaging team.

**Product studio, sole frontend engineer (Mar 2023 - Nov 2024)**

* Delivered 5 products end to end: 80+ screens and 130+ reusable components in React, Next.js and React Native across govtech, fintech and social.
* Built an applicant-facing portal with multi-step building permit flows and full i18next localisation; fintech dashboards with investment package browsing, booking and onboarding; a React Native / Expo dating app MVP with gesture-driven navigation and swipe interactions.
* Improved LCP/FCP on key routes via code splitting and lazy loading (verified in Lighthouse); wrote 50+ Jest tests across forms, onboarding and state.

**Orthodontic aligner manufacturer (Aug 2021 - Jan 2023)**

* Built an internal SPA for partner orthodontists (case submission, photo upload, support messaging, loyalty points); 3,000+ clinical cases went through it.
* Delivered 30+ marketing landing pages and ran A/B tests in Yandex.Metrica and Vercel Analytics, cutting time to conversion on a key page by 12%.

---

### Portfolio Highlights (Freelance and pet projects)

* **[feiary.ru - Custom leather goods ordering platform](https://feiary.ru)**
    * **Role:** Frontend / Product Engineer (team of 3).
    * **Tech Stack:** Next.js, TypeScript, Canvas API.
    * **Key Contributions:** Owned the order submission pipeline, site structure and codebase organisation. Restructured the order handler into focused modules (validation, email, error handling, request parsing), cutting it to half the lines. Built a canvas-based drag-and-drop design configurator where customers upload artwork and preview it on leather products before ordering. Implemented a bilingual (RU/EN) order flow with drag-and-drop upload and specific error messages per failure type. Added SEO coverage: metadata, sitemap, correct routing.

* **[Valentin Diakonov - Art Critic Portfolio (yick.art)](https://yick.art/en)**
    * **Role:** Frontend / Product Engineer.
    * **Tech Stack:** Next.js, TypeScript, Sanity.io, GraphQL.
    * **Key Contributions:** Built end to end: briefed the designer, defined features, built the frontend, managed the CMS, handled deployments. Alphabetical artist navigator, bilingual (RU/EN) article system, per-device image optimisation, page-level caching, full SEO coverage (titles, descriptions, sitemap, hreflang).

* **[Incredibly Cool Game (Vampire Survivors Clone)](https://github.com/orange1072/incredibly-cool-game)**
    * **Role:** Engine Developer / Frontend Architect.
    * **Tech Stack:** TypeScript, OOP, Redux Toolkit (RTK Query), Canvas API.
    * **Engine Architecture:** Designed a custom **[modular game engine](https://github.com/orange1072/incredibly-cool-game/tree/dev/packages/client/src/engine)** on mixins: game mechanics and entities (player, enemies, projectiles) are composed from independent modules (collisions, health, AI behaviours, spawning, camera).
    * **Rendering System:** Canvas API renderer from scratch: world-rendering pipeline, camera (follow/zoom), optimised sprite rendering for high-density mob scenes.
    * **State Management & UI:** Custom [adapter](https://github.com/orange1072/incredibly-cool-game/tree/dev/packages/client/src/engine/adapters) syncing engine state with the React UI; [game states](https://github.com/orange1072/incredibly-cool-game/tree/dev/packages/client/src/store/slices/game); forum API via RTK Query [createApi](https://github.com/orange1072/incredibly-cool-game/tree/dev/packages/client/src/api).

* **[Messenger Framework & Chat App](https://ws-chat-advance.netlify.app/)** - [source](https://github.com/zknone/ws-chat-advance)
    * **Role:** Frontend Engineer.
    * **Tech Stack:** TypeScript, OOP, Handlebars, Vite, Mocha/Chai.
    * **Highlights:** Custom SPA framework from scratch (Router, Store, block-based component system), private routing, persistent sessions, real-time messaging via WebSocket, strict ESLint/Stylelint, unit tests for core framework modules.
---
