# 🤖 AI-Assisted Web Development Course Guide (Taglish)

> **Modern web development gamit ang AI tools (Claude Code CLI / OpenCode CLI), Laravel, Next.js, at MySQL.**
> Matuto kang bumuo ng full-stack applications nang mas mabilis at mas efficient sa tulong ng AI coding assistants.
> Lahat ng lessons ay Taglish — halo ng Tagalog at English para swak sa Pinoy developers.

---

## 📦 COURSE OVERVIEW

| Phase | Focus Area | Total Lessons |
|-------|------------|---------------|
| Phase 0 | AI Coding Tools Setup & Mindset | 6 |
| Phase 1 | MySQL Database Design & Management | 7 |
| Phase 2 | Laravel Backend Development | 10 |
| Phase 3 | Next.js Frontend Development | 9 |
| Phase 4 | API Integration & Full-Stack Communication | 6 |
| Phase 5 | Authentication, Authorization & Security | 7 |
| Phase 6 | Testing, Debugging & Performance | 6 |
| Phase 7 | Deployment, DevOps & Maintenance | 5 |
| Phase 8 | Capstone Projects | 4 |

---

## 🤖 PHASE 0: AI CODING TOOLS SETUP & MINDSET
*Dito mo matututunan paano gamitin ang AI bilang coding partner mo — hindi ka papalitan, pero papabilisin ka.*

### Lesson 0.1 – Introduction to AI-Assisted Development
- Ano ang AI coding assistants? (Claude Code CLI, OpenCode CLI, GitHub Copilot, Cursor)
- Paano naiiba ang AI-assisted development sa traditional coding
- Mindset shift: AI bilang "pair programmer" mo, hindi "magic button"
- **Taglish:** "Si AI ay parang senior dev na laging available mag-suggest at mag-review ng code mo — pero ikaw pa rin ang may final say."

### Lesson 0.2 – Setting Up Claude Code CLI
- Installing Claude Code CLI (npm install, authentication)
- System requirements at API keys
- Basic commands: `claude`, `claude "prompt"`, interactive mode
- Configuring Claude Code (`.claude` settings)
- **Taglish:** "I-install mo lang via npm, mag-login gamit ang Anthropic account mo, at handa ka nang mag-prompt."

### Lesson 0.3 – Setting Up OpenCode CLI (Alternative)
- What is OpenCode CLI? Open-source alternative
- Installation at setup
- Pagkukumpara kay Claude Code CLI (features, pricing, performance)
- When to use which tool
- **Taglish:** "Kung open-source ang trip mo, OpenCode CLI ang option. Halos pareho ng workflow pero community-driven."

### Lesson 0.4 – Effective Prompt Engineering for Coding
- Paano magsulat ng malinaw na prompts para sa AI
- Context setting: anong tech stack, anong goal, anong constraints
- Iterative prompting: refine, clarify, at iwasan ang vague instructions
- Examples: "Create a Laravel controller that..." vs "Gawa ka ng controller"
- **Taglish:** "Mas specific ang prompt mo, mas accurate ang output ng AI. Sabihin mo: 'Gamit ang Laravel 11, gumawa ka ng UserController na may CRUD operations, PDO prepared statements, at validation.'"

### Lesson 0.5 – AI-Assisted Workflow Best Practices
- Prompt → Review → Test → Refactor cycle
- Paano i-verify ang AI-generated code (huwag bulag na pagkatiwalaan)
- Using AI for debugging at error explanation
- Documenting AI-assisted code
- **Taglish:** "AI ang magsusulat ng unang draft, pero ikaw ang mag-iisip kung tama ba 'yun. Laging may human review."

### Lesson 0.6 – Local Dev Environment Setup (Laravel + Next.js + MySQL)
- Installing PHP, Composer, Node.js, npm
- Setting up Laravel project (`composer create-project laravel/laravel`)
- Setting up Next.js project (`npx create-next-app@latest`)
- MySQL installation (XAMPP/Laragon o Docker)
- Project structure overview para sa full-stack app
- **Taglish:** "Magkahiwalay ang backend (Laravel sa port 8000) at frontend (Next.js sa port 3000) — ganito ang modern full-stack setup."

---

## 🗄️ PHASE 1: MYSQL DATABASE DESIGN & MANAGEMENT
*Ang database ang puso ng application — dito naka-store lahat ng data mo.*

### Lesson 1.1 – Database Fundamentals with MySQL
- Relational database concepts (tables, rows, columns)
- MySQL installation at setup (XAMPP/Laragon)
- phpMyAdmin at MySQL CLI basics
- Creating your first database at table
- **Taglish:** "Ang MySQL database ay parang filing cabinet — may folders (tables), may documents (rows), at may fields (columns)."

### Lesson 1.2 – SQL Fundamentals (DDL & DML)
- Data Types: INT, VARCHAR, TEXT, DATE, DATETIME, DECIMAL, BOOLEAN
- CREATE TABLE, ALTER TABLE, DROP TABLE
- INSERT, SELECT, UPDATE, DELETE
- WHERE, ORDER BY, LIMIT, DISTINCT
- **Taglish:** "`SELECT * FROM users WHERE age > 18 ORDER BY name;` — eto na ang basic query structure na magagamit mo araw-araw."

### Lesson 1.3 – Advanced SQL Queries (Prompting AI)
- JOINs: INNER, LEFT, RIGHT (with AI-generated examples)
- GROUP BY at aggregate functions (COUNT, SUM, AVG, MAX, MIN)
- Subqueries at derived tables
- Using AI to generate complex queries: "Gumawa ka ng SQL query na magdi-display ng total orders per customer..."
- **Taglish:** "Kapag nahihirapan ka sa complex JOIN, i-describe mo lang kay AI ang gusto mong output — siya na gagawa ng query."

### Lesson 1.4 – Database Design & Normalization
- Entity-Relationship Diagrams (ERD) — generating gamit ang AI
- Normalization: 1NF, 2NF, 3NF
- Pag-design ng schema para sa e-commerce, blog, o task management app
- Using AI to suggest optimal table structures
- **Taglish:** "Sabihin mo kay AI: 'I-design mo ang database schema para sa isang e-commerce app na may users, products, orders, at reviews.'"

### Lesson 1.5 – Indexes, Constraints & Performance
- Primary keys, foreign keys, unique constraints
- Indexes: bakit kailangan? (B-tree indexes)
- Query optimization basics: EXPLAIN statement
- Using AI to suggest indexes base sa queries mo
- **Taglish:** "Ang index parang table of contents ng libro — kung wala, isa-isang babasahin ni MySQL bawat pahina (row)."

### Lesson 1.6 – Database Migrations with Laravel
- What are migrations? Version control for database schema
- Creating migrations: `php artisan make:migration`
- Schema builder: `$table->string()`, `$table->foreignId()`, etc.
- Running at rolling back migrations
- Using AI to generate migration files: "Gumawa ka ng Laravel migration para sa products table..."
- **Taglish:** "Sa Laravel, hindi ka direktang gumagawa ng table sa phpMyAdmin — migration files ang gamit para version-controlled ang schema."

### Lesson 1.7 – Seeding & Factories (AI-Assisted)
- Database seeders: paano mag-populate ng test data
- Laravel Factories: generating realistic fake data
- Using AI to generate seeders: "Gumawa ka ng seeder na magpo-produce ng 50 fake users..."
- **Taglish:** "Kapag nagde-develop, kailangan mo ng dummy data — si AI na bahalang gumawa ng realistic names, emails, at iba pa."

---

## 🐘 PHASE 2: LARAVEL BACKEND DEVELOPMENT
*Ang Laravel ang isa sa pinakasikat na PHP framework — dito mo bubuuin ang backend logic at API.*

### Lesson 2.1 – Laravel Fundamentals at AI Pair Programming
- Laravel project structure overview
- Artisan CLI: `php artisan` commands
- Routes: `web.php` vs `api.php`
- Basic Controller: `php artisan make:controller`
- Using AI to scaffold controllers at routes
- **Taglish:** "Sabihin mo kay AI: 'Gumawa ka ng API routes at Controller para sa Product CRUD sa Laravel 11.' Instant scaffolding."

### Lesson 2.2 – Eloquent ORM: Models & Relationships
- Eloquent models: `php artisan make:model`
- Basic CRUD with Eloquent
- Relationships: hasMany, belongsTo, belongsToMany, hasOne
- Eager loading vs lazy loading (N+1 problem)
- Using AI to generate models with relationships
- **Taglish:** "Ang Eloquent ay para kang may personal assistant na nagsasalin ng SQL queries to PHP objects — mas readable at secure."

### Lesson 2.3 – Form Requests & Validation (AI-Generated)
- Creating Form Requests: `php artisan make:request`
- Validation rules: required, email, unique, min, max, etc.
- Custom error messages (Tagalog puwede!)
- Using AI to generate validation rules: "Gumawa ka ng StoreUserRequest na may validation para sa name, email, password..."
- **Taglish:** "Ang validation ay huwag na huwag pagkakatiwalaan ang user input — si AI na bahalang mag-generate ng kumpletong rules."

### Lesson 2.4 – API Resources & Transformations
- API Resources: `php artisan make:resource`
- Transforming model data to JSON consistently
- Pagination with API Resources
- Using AI to generate Resource classes
- **Taglish:** "Ang API Resource ay nagfo-format ng JSON response mo — consistent ang structure, kahit iba-iba ang data."

### Lesson 2.5 – Middleware & Request Lifecycle
- What is Middleware? Request → Middleware → Controller
- Built-in middleware: auth, throttle, cors
- Creating custom middleware: `php artisan make:middleware`
- Using AI to create middleware: "Gumawa ka ng middleware na magla-log ng lahat ng API requests..."
- **Taglish:** "Middleware ay parang checkpoints — bago makarating ang request sa controller, dumadaan muna sa mga filters."

### Lesson 2.6 – File Uploads & Storage (AI-Assisted)
- Handling file uploads in Laravel
- Storage facade: local, public, S3
- Image intervention/optimization
- Using AI to generate file upload logic
- **Taglish:** "Kapag mag-a-upload ng image, huwag i-store sa database ang file mismo — ang path lang, ang file sa storage."

### Lesson 2.7 – Queues, Jobs & Background Processing
- What are queues? Offloading slow tasks
- Creating Jobs: `php artisan make:job`
- Dispatching jobs, failed jobs handling
- Using AI to create queued jobs (e.g., sending email, generating reports)
- **Taglish:** "Kapag may task na mabagal (e.g., mag-email sa 1000 users), ilagay sa queue para hindi maghintay si user."

### Lesson 2.8 – Caching & Performance Optimization
- Laravel Cache: Redis, Memcached, file
- Caching queries, views, at config
- Rate limiting APIs
- Using AI to suggest caching strategies
- **Taglish:** "Kung paulit-ulit ang query na hindi nagbabago, i-cache mo — instant load sa susunod."

### Lesson 2.9 – Error Handling & Logging
- Exception handling in Laravel
- Custom exceptions
- Logging: channels (single, daily, slack), levels (debug, info, error)
- Using AI to generate try-catch blocks at logging
- **Taglish:** "Kapag may error, dapat naka-log — para kapag nagreklamo si user, alam mo kung anong nangyari."

### Lesson 2.10 – Building RESTful API with AI Assistance
- RESTful conventions: GET, POST, PUT/PATCH, DELETE
- Nested resources
- API versioning (v1, v2)
- Complete CRUD API building with AI pair programming
- **Taglish:** "Sa lesson na ito, gagawa tayo ng kumpletong API gamit ang AI — from scratch to fully tested endpoints."

---

## ⚛️ PHASE 3: NEXT.JS FRONTEND DEVELOPMENT
*Ang Next.js ay React framework — dito mo bubuuin ang modern, mabilis na frontend.*

### Lesson 3.1 – Next.js App Router Fundamentals
- Next.js project structure (App Router)
- Pages vs Layouts, `page.tsx`, `layout.tsx`
- Server Components vs Client Components
- File-based routing
- Using AI to generate pages at layouts
- **Taglish:** "Sa App Router, ang folder structure mo ang nagde-define ng URLs — `app/products/page.tsx` = `/products`."

### Lesson 3.2 – React Essentials for Next.js
- JSX, Components, Props
- State management: `useState`, `useEffect`
- Event handling, conditional rendering
- Using AI to create React components: "Gumawa ka ng ProductCard component na may props ng title, price, at image..."

### Lesson 3.3 – Styling with Tailwind CSS (AI-Assisted)
- Installing Tailwind CSS sa Next.js
- Utility-first classes: spacing, colors, typography, flex, grid
- Responsive design: `sm:`, `md:`, `lg:`, `xl:`
- Using AI to generate styled components
- **Taglish:** "Describe mo lang kay AI ang itsura ng gusto mong UI: 'Gumawa ka ng card component na may shadow, rounded corners, at hover effect.' Si AI na bahala sa Tailwind classes."

### Lesson 3.4 – Data Fetching in Next.js
- Server-side data fetching (Server Components)
- Client-side fetching: `useEffect` + `fetch` o SWR/React Query
- Static vs Dynamic rendering
- Using AI to generate data fetching logic
- **Taglish:** "Sa Next.js, puwedeng sa server pa lang naka-fetch na ang data (server components) o sa browser (client components)."

### Lesson 3.5 – Forms & Mutations (Server Actions)
- Server Actions in Next.js 14+
- Form handling with validation
- `useFormState` at `useFormStatus`
- Using AI to create form components with validation
- **Taglish:** "Ang Server Actions ay bagong feature — puwedeng mag-process ng form data nang direkta sa server, hindi na kailangan ng separate API endpoint."

### Lesson 3.6 – State Management (Context API & Zustand)
- React Context API for global state
- Zustand: lightweight state management
- When to use which
- Using AI to set up state management
- **Taglish:** "Kung simpleng global state lang (e.g., user auth), Context API sapat na. Kung complex, Zustand ang mas malinis."

### Lesson 3.7 – Authentication UI & Protected Routes
- Login/Register forms
- Middleware for route protection
- Session management sa frontend
- Using AI to generate auth UI
- **Taglish:** "Dapat may middleware sa Next.js para i-check kung naka-login ang user bago ma-access ang dashboard."

### Lesson 3.8 – Error Handling & Loading States
- `error.tsx`, `loading.tsx`, `not-found.tsx` (Next.js conventions)
- Suspense boundaries
- Using AI to create error boundaries at loading skeletons
- **Taglish:** "Built-in sa Next.js ang error handling — gumawa ka lang ng `error.tsx` file sa folder, automatic 'yun ang lalabas."

### Lesson 3.9 – Optimizing Next.js (Images, Fonts, SEO)
- Next.js Image component (`next/image`)
- Font optimization (`next/font`)
- Metadata API for SEO
- Using AI to generate metadata at optimize assets
- **Taglish:** "Si `next/image` automatic na nag-o-optimize ng images — lazy loading, resizing, at modern formats. Gamitin mo 'to, huwag `<img>`."

---

## 🔗 PHASE 4: API INTEGRATION & FULL-STACK COMMUNICATION
*Dito pagdurugtungin ang Laravel backend at Next.js frontend.*

### Lesson 4.1 – Laravel CORS & API Configuration
- CORS setup sa Laravel (config/cors.php)
- API prefix at versioning
- Sanctum/Laravel Passport (SPA authentication intro)
- Using AI to configure CORS
- **Taglish:** "Kapag magkaiba ang domain ng frontend (`localhost:3000`) at backend (`localhost:8000`), kailangan ng CORS para payagan ang requests."

### Lesson 4.2 – Fetching Data from Laravel API to Next.js
- Server-side fetching sa Next.js (Server Components)
- Axios vs native `fetch`
- Handling loading, error, at success states
- Using AI to generate API service files
- **Taglish:** "Gumawa ng `api.ts` file na naglalaman ng lahat ng API calls — para isang lugar lang ang titingnan kapag may babaguhin."

### Lesson 4.3 – CRUD Operations: Full-Stack Integration
- Create, Read, Update, Delete mula Next.js papuntang Laravel
- Form submissions, confirmations, toast notifications
- Optimistic updates
- Using AI to generate complete CRUD workflows
- **Taglish:** "Buuin natin ang buong flow — from button click sa Next.js, papuntang Laravel API, papuntang MySQL, pabalik sa UI."

### Lesson 4.4 – File Uploads: Frontend to Backend
- File input sa Next.js, FormData
- Handling file uploads sa Laravel (muling bisitahin)
- Progress bars, preview images
- Using AI to generate upload components
- **Taglish:** "Ang file upload ay asynchronous — gumamit ng FormData at progress indicator para magandang UX."

### Lesson 4.5 – Real-Time Features (WebSockets with Laravel Reverb)
- Introduction to WebSockets
- Laravel Reverb setup
- Real-time notifications, chat, o live updates
- Using AI to set up broadcasting
- **Taglish:** "Hindi na kailangan mag-refresh ng page — kapag may bagong data, automatic lalabas. Real-time = happy users."

### Lesson 4.6 – Error Handling & API Response Standardization
- Consistent API response structure
- Error codes at messages
- Frontend error handling (toast, modal, inline)
- Using AI to create error handling utilities
- **Taglish:** "Lahat ng API response mo dapat may iisang format — para predictable ang error handling sa frontend."

---

## 🔐 PHASE 5: AUTHENTICATION, AUTHORIZATION & SECURITY
*Proteksyunan ang app at data ng users — critical ito sa kahit anong production app.*

### Lesson 5.1 – Laravel Sanctum for SPA Authentication
- Installing at configuring Laravel Sanctum
- Token-based authentication vs session-based
- Login, register, logout API endpoints
- Using AI to generate auth controllers
- **Taglish:** "Ang Sanctum ay magaan na authentication package — perfect para sa SPA (Single Page Application) tulad ng Next.js."

### Lesson 5.2 – NextAuth.js Integration (Alternative to Sanctum)
- What is NextAuth.js? (Auth.js)
- Setting up with Laravel API as backend
- Credentials provider, OAuth (Google, GitHub)
- Using AI to configure NextAuth
- **Taglish:** "NextAuth.js ay swak kung gusto mo ng built-in na auth UI at OAuth providers. Puwede ring gamitin kasabay ng Laravel backend."

### Lesson 5.3 – Role-Based Access Control (RBAC)
- Designing user roles (admin, editor, user)
- Middleware for role checking
- Frontend: conditional rendering base sa role
- Using AI to generate RBAC logic
- **Taglish:** "Hindi lahat ng user dapat may access sa admin panel — mag-check ng role bago mag-render ng component o mag-process ng request."

### Lesson 5.4 – API Security Best Practices (AI-Guided)
- Rate limiting sa Laravel
- Input sanitization at XSS prevention
- CSRF tokens
- HTTPS enforcement
- Using AI to audit security
- **Taglish:** "Sabihin mo kay AI: 'I-audit mo ang security ng API routes ko at mag-suggest ng improvements.'"

### Lesson 5.5 – Password Hashing, Tokens & Secure Storage
- `bcrypt` hashing sa Laravel
- JWT vs opaque tokens
- Storing tokens securely sa frontend (httpOnly cookies vs localStorage)
- Password reset flow
- Using AI to implement password reset
- **Taglish:** "Huwag i-store ang tokens sa localStorage kung puwede sa httpOnly cookies — mas secure laban sa XSS attacks."

### Lesson 5.6 – Email Verification & Two-Factor Authentication
- Email verification flow sa Laravel
- Setting up mail (Mailtrap for development)
- 2FA concept at implementation
- Using AI to generate verification workflows
- **Taglish:** "Sa production, kailangan i-verify ang email ng user — para siguradong totoong tao ang nagre-register."

### Lesson 5.7 – Security Testing & Vulnerability Scanning (with AI)
- Common vulnerabilities (OWASP Top 10)
- Using AI to scan code for vulnerabilities
- Penetration testing basics
- Security headers (CSP, HSTS)
- **Taglish:** "Gamitin si AI para maghanap ng potential security holes — 'Check my code for SQL injection vulnerabilities at XSS.'"

---

## 🧪 PHASE 6: TESTING, DEBUGGING & PERFORMANCE
*Siguraduhing matibay at mabilis ang application — testing at optimization.*

### Lesson 6.1 – Laravel Testing (Pest/PHPUnit) with AI
- Unit tests vs Feature tests
- Pest PHP: modern testing framework
- Testing API endpoints, authentication, database
- Using AI to generate test cases: "Write Pest tests for my Product CRUD API..."
- **Taglish:** "Ang test ang safety net mo — kapag may binago ka, malalaman mo agad kung may nasira. Si AI na magsusulat ng boilerplate tests."

### Lesson 6.2 – Next.js Testing (Jest + React Testing Library)
- Component testing
- Integration testing
- End-to-end (E2E) testing with Playwright
- Using AI to generate frontend tests
- **Taglish:** "Test kung nagre-render nang tama ang components, kung gumagana ang forms, at kung tama ang navigation."

### Lesson 6.3 – AI-Assisted Debugging Techniques
- Using AI to explain error messages
- "Rubber duck debugging" with AI
- Stack trace analysis at suggestion ng fix
- **Taglish:** "I-paste mo lang ang error message kay AI: 'Bakit nagkakaganito ang error na 'to? Paano i-fix?'"

### Lesson 6.4 – Laravel Performance Optimization
- Query optimization (N+1 problem, eager loading)
- Caching strategies (Redis, model caching)
- Queue optimization
- Using AI to identify performance bottlenecks
- **Taglish:** "Gamitin ang Laravel Debugbar para makita ang queries — kapag maraming duplicate, may problema."

### Lesson 6.5 – Next.js Performance Optimization
- Bundle analysis (`@next/bundle-analyzer`)
- Code splitting at lazy loading
- Image at font optimization
- Server Components vs Client Components (best practices)
- **Taglish:** "Next.js may built-in na performance features — pero kailangan mo pa ring maging mindful sa bundle size at data fetching strategy."

### Lesson 6.6 – Logging, Monitoring & Error Tracking
- Laravel logging (daily logs, external services)
- Frontend error tracking (Sentry)
- Health checks at monitoring
- Using AI to set up monitoring
- **Taglish:** "Kapag nasa production na, hindi mo na pwedeng i-`dd()` ang errors — kailangan ng proper logging at monitoring tools."

---

## 🚀 PHASE 7: DEPLOYMENT, DEVOPS & MAINTENANCE
*Ilabas na sa mundo ang ginawa mong application.*

### Lesson 7.1 – Preparing for Production (AI Checklist)
- Environment configuration (`.env` for production)
- Asset compilation at minification
- Database migration strategy for production
- Using AI to generate deployment checklist
- **Taglish:** "Sabihin mo kay AI: 'Gumawa ka ng pre-deployment checklist para sa Laravel + Next.js app.'"

### Lesson 7.2 – Deploying Laravel Backend
- Deployment options: VPS (DigitalOcean, Linode), shared hosting, Laravel Forge
- Server setup (Nginx, PHP-FPM, MySQL)
- CI/CD basics (GitHub Actions)
- Using AI to generate deployment scripts
- **Taglish:** "Ang Laravel Forge ay parang personal assistant para sa server management — pero mahal. Kung tipid, manual VPS setup."

### Lesson 7.3 – Deploying Next.js Frontend
- Vercel (recommended for Next.js)
- Self-hosting with Docker
- Environment variables sa production
- Custom domain at SSL
- **Taglish:** "Ang Vercel ang pinakamadaling i-deploy ang Next.js — ilang clicks lang, live na. Libre para sa small projects."

### Lesson 7.4 – MySQL Database in Production
- Managed databases (PlanetScale, DigitalOcean Managed DB)
- Backups at disaster recovery
- Database migration sa production (zero downtime)
- Using AI to generate backup scripts
- **Taglish:** "Huwag kalimutang mag-backup ng database — automated gabi-gabi. Kapag nasira, may babalikan."

### Lesson 7.5 – Maintenance, Updates & Continuous Improvement
- Monitoring uptime (UptimeRobot, Laravel Pulse)
- Dependency updates (Composer, npm)
- Handling user feedback at bug reports
- Iterative improvement with AI
- **Taglish:** "Ang software development ay hindi natatapos sa deployment — tuloy-tuloy ang improvement base sa user feedback."

---

## 🏆 PHASE 8: CAPSTONE PROJECTS
*Ilapat lahat ng natutunan sa real-world projects.*

### Lesson 8.1 – Capstone Project 1: Task Management System
- **Features:** User auth, project CRUD, task assignment, real-time updates, file attachments
- **Tech:** Laravel API + Next.js + MySQL + Laravel Reverb (WebSockets)
- **AI Role:** Scaffolding, debugging, test generation
- **Taglish:** "Gagawa ka ng parang Trello o Jira — full-stack with real-time updates. Kayang-kaya with AI assistance."

### Lesson 8.2 – Capstone Project 2: E-Commerce Platform
- **Features:** Product listing, cart, checkout, order tracking, admin dashboard, payment integration (PayMongo/Stripe)
- **Tech:** Laravel + Next.js + MySQL + Redis (caching)
- **AI Role:** Complex query generation, UI component creation, payment integration
- **Taglish:** "E-commerce na may admin panel — dito mo marerealize ang power ng AI-assisted development."

### Lesson 8.3 – Capstone Project 3: Social Media / Community App
- **Features:** Posts, comments, likes, follows, notifications, chat
- **Tech:** Laravel + Next.js + MySQL + Pusher/WebSockets
- **AI Role:** Real-time features, complex relationships, UI/UX
- **Taglish:** "Sarili mong social network — mas simple sa Facebook pero with core features."

### Lesson 8.4 – Capstone Project 4: AI-Enhanced SaaS Application
- **Features:** Your own SaaS idea + AI integration (e.g., AI content generator, AI analytics)
- **Tech:** Laravel + Next.js + MySQL + AI API integration (OpenAI, Claude)
- **AI Role:** AI feature integration, billing system, multi-tenancy
- **Taglish closing note:** "Ito na ang pinaka-advanced — gagawa ka ng SaaS na may AI features. Dito mo pagsasamahin lahat: backend, frontend, database, AI tools, deployment. After nito, ready ka na sa kahit anong web dev challenge. Congrats!"

---

## 📚 RECOMMENDED RESOURCES

| Resource | Bakit Maganda? |
|----------|----------------|
| **Laravel Documentation** | Official docs, updated, may examples. I-prompt mo kay AI: "Explain Laravel routing based on docs..." |
| **Next.js Documentation** | Sobrang linaw, may interactive examples. |
| **Claude Code CLI Docs** | Official guide sa paggamit ng Claude Code. |
| **Laracasts** | Video tutorials (may bayad pero may free series). |
| **Traversy Media (YouTube)** | Crash courses sa Laravel at Next.js. |
| **Vercel Templates** | Pre-built Next.js templates, pwedeng pag-aralan ang structure. |
| **Laravel News & Laravel Daily** | Latest updates at tutorials. |

---

## ✅ COURSE COMPLETION CHECKLIST

- [ ] Marunong nang gumamit ng AI tools (Claude Code / OpenCode) bilang coding assistant
- [ ] Kaya nang mag-design ng MySQL database na normalized at optimized
- [ ] Nakakapag-develop ng RESTful API gamit ang Laravel (Controllers, Models, Middleware, Resources)
- [ ] Nakakapag-build ng modern UI gamit ang Next.js App Router at Tailwind CSS
- [ ] Marunong nang mag-integrate ng Laravel backend at Next.js frontend
- [ ] Naipatupad ang kumpletong authentication, authorization, at security best practices
- [ ] May karanasan sa testing, debugging, at performance optimization
- [ ] Nakapag-deploy ng full-stack application sa production
- [ ] Nakatapos ng kahit isang capstone project mula Phase 8

---

> **Ang AI ay tool — ikaw pa rin ang developer. Gamitin mo ito para mapabilis ang trabaho, hindi para palitan ang pag-iisip. Sa bawat project, mas gumagaling ka, mas bumababa ang oras ng development, at mas tumataas ang kalidad. Good luck, ka-developer!** 🇵🇭🤖⚛️🐘