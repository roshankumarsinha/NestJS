# NestJS — Complete Course Notes

Lecture-wise notes for **The Techzeen — NestJS Tutorial** series
Playlist: https://www.youtube.com/playlist?list=PL5OhSdfH4uDt6iG-qze_Q3qgik6VKHeRU

**How these notes work**

- One section per lecture, in order, each with its video link.
- A concept is explained **in full where it first appears**; later lectures only cross-reference it (e.g. Guards are explained at Video 14, so Video 44 just links back). This keeps the file long but not repetitive.
- Blocks marked **⚠️ Correction / Beyond the video** are additions from outside the tutorial — API changes, production gotchas, or things the video simplified. Treat these as the more current guidance.

---

## Course Index

✅ = written up below · ⬜ = not yet added

| #   | Lecture                                           | Link                                             |     |
| --- | ------------------------------------------------- | ------------------------------------------------ | --- |
| 1   | Why NestJS? What Problem It Solves                | [▶](https://www.youtube.com/watch?v=K_OjtrsJGTk) | ✅  |
| 2   | Installation & First App with the CLI             | [▶](https://www.youtube.com/watch?v=Hz7IFywSxJk) | ✅  |
| 3   | File & Folder Structure Explained                 | [▶](https://www.youtube.com/watch?v=XpVpoHLSTFg) | ✅  |
| 4   | Create Your First Controller with CLI             | [▶](https://www.youtube.com/watch?v=yE2GvMqSuxQ) | ✅  |
| 5   | Services: @Injectable, CLI, Constructor Injection | [▶](https://www.youtube.com/watch?v=Cd-a0EUpj_8) | ✅  |
| 6   | Modules in NestJS                                 | [▶](https://www.youtube.com/watch?v=BQ_1hHJAlWM) | ✅  |
| 7   | NestJS Architecture Explained                     | [▶](https://www.youtube.com/watch?v=o6V8xzEhDPA) | ✅  |
| 8   | Dependency Injection in NestJS                    | [▶](https://www.youtube.com/watch?v=Fgikn8N_mus) | ✅  |
| 9   | REST API & HTTP Methods + Postman                 | [▶](https://www.youtube.com/watch?v=Uyk6bwm2eWI) | ✅  |
| 10  | Create REST APIs (GET/POST/PUT/PATCH/DELETE)      | [▶](https://www.youtube.com/watch?v=w9JYelWOSj4) | ✅  |
| 11  | DTOs & Interfaces Explained                       | [▶](https://www.youtube.com/watch?v=E3TbXT2TR5Q) | ✅  |
| 12  | Validating DTOs with class-validator              | [▶](https://www.youtube.com/watch?v=IIKZVHy1Dqw) | ✅  |
| 13  | Custom Pipes                                      | [▶](https://www.youtube.com/watch?v=KUj0XcnD85U) | ✅  |
| 14  | Protecting Routes using Guards                    | [▶](https://www.youtube.com/watch?v=iJeJGVk9ZX8) | ✅  |
| 15  | Role-Based Authorization in Guards                | [▶](https://www.youtube.com/watch?v=MjbElEDIYnQ) | ✅  |
| 16  | Exception Filters & Custom Error Handling         | [▶](https://www.youtube.com/watch?v=OgQPOMsPn4A) | ✅  |
| 17  | Middleware in NestJS                              | [▶](https://www.youtube.com/watch?v=5JhFvdPwkKA) | ✅  |
| 18  | Lifecycle Events / Hooks                          | [▶](https://www.youtube.com/watch?v=NpS7qpim3IQ) | ✅  |
| 19  | Lifecycle Hooks: onModuleInit & onAppShutdown     | [▶](https://www.youtube.com/watch?v=xp4jDjWG_tE) | ✅  |
| 20  | Environment Variables & .env                      | [▶](https://www.youtube.com/watch?v=gMCUp31uYgY) | ✅  |
| 21  | MongoDB Introduction                              | [▶](https://www.youtube.com/watch?v=rs0xuTVovLQ) | ⬜  |
| 22  | Connect NestJS with MongoDB Atlas                 | [▶](https://www.youtube.com/watch?v=ZUaOXqKuc5E) | ⬜  |
| 23  | Create & Register Mongoose Schemas                | [▶](https://www.youtube.com/watch?v=q197qAzb0VI) | ⬜  |
| 24  | Insert Data (POST API)                            | [▶](https://www.youtube.com/watch?v=608mxgB5IoI) | ⬜  |
| 25  | Get Data: find() & findById()                     | [▶](https://www.youtube.com/watch?v=gBmGWSpO7IE) | ⬜  |
| 26  | Update with PUT & findByIdAndUpdate               | [▶](https://www.youtube.com/watch?v=tccQ3rwmmYA) | ⬜  |
| 27  | Update with PATCH — PUT vs PATCH                  | [▶](https://www.youtube.com/watch?v=ul-_E9ARwSA) | ⬜  |
| 28  | Delete Data (DELETE API)                          | [▶](https://www.youtube.com/watch?v=q_yKiuzI88U) | ⬜  |
| 29  | Data Relationships in MongoDB                     | [▶](https://www.youtube.com/watch?v=ZgTS6mbUOhw) | ⬜  |
| 30  | One-to-One via Embedding                          | [▶](https://www.youtube.com/watch?v=N9DHAZn0Cf0) | ⬜  |
| 31  | One-to-One via Referencing                        | [▶](https://www.youtube.com/watch?v=ULmdPRL7QRY) | ⬜  |
| 32  | One-to-Many via Embedding                         | [▶](https://www.youtube.com/watch?v=ObpBY8xerVQ) | ⬜  |
| 33  | One-to-Many via Referencing                       | [▶](https://www.youtube.com/watch?v=6xMl9fFdV8E) | ⬜  |
| 34  | Many-to-Many via Referencing                      | [▶](https://www.youtube.com/watch?v=rrkaCC2iC8w) | ⬜  |
| 35  | PostgreSQL & TypeORM Explained                    | [▶](https://www.youtube.com/watch?v=S9yeUbVBT-s) | ⬜  |
| 36  | Connect Supabase PostgreSQL (TypeORM Setup)       | [▶](https://www.youtube.com/watch?v=9vULzFAAxdg) | ⬜  |
| 37  | Insert Data into Supabase PostgreSQL              | [▶](https://www.youtube.com/watch?v=BIJeWSLkCwY) | ⬜  |
| 38  | Fetch Data (GET API with TypeORM)                 | [▶](https://www.youtube.com/watch?v=JKD5gD8Hdro) | ⬜  |
| 39  | Update Data (PUT API with TypeORM)                | [▶](https://www.youtube.com/watch?v=sE9mY_Fph_g) | ⬜  |
| 40  | Delete Data from PostgreSQL                       | [▶](https://www.youtube.com/watch?v=n50peUYhIpE) | ⬜  |
| 41  | Filter & Search using @Query()                    | [▶](https://www.youtube.com/watch?v=c65XNX58hqo) | ⬜  |
| 42  | JWT Explained — Authentication vs Authorization   | [▶](https://www.youtube.com/watch?v=GRSkwtywXfM) | ⬜  |
| 43  | Supabase JWT Authentication with Login API        | [▶](https://www.youtube.com/watch?v=CyX5lzJPT4Y) | ⬜  |
| 44  | JWT Authentication with MongoDB                   | [▶](https://www.youtube.com/watch?v=qry1F5ibO4U) | ✅  |
| 45  | What is GraphQL? GraphQL vs REST                  | [▶](https://www.youtube.com/watch?v=jwmkOUMyzJE) | ⬜  |
| 46  | GraphQL CRUD App with MongoDB                     | [▶](https://www.youtube.com/watch?v=EaHzlvyObAU) | ⬜  |
| 47  | Prisma ORM & Neon DB                              | [▶](https://www.youtube.com/watch?v=RvZ3G1jH4dU) | ⬜  |
| 48  | CRUD with GraphQL, Prisma & Neon                  | [▶](https://www.youtube.com/watch?v=H-VMmVcWQEs) | ⬜  |
| 49  | Rate Limiting using Throttler                     | [▶](https://www.youtube.com/watch?v=VjkX4Fm3YFM) | ✅  |
| 50  | Deploy NestJS App on Railway                      | [▶](https://www.youtube.com/watch?v=V5ocs-gHzo4) | ✅  |

---

# Part 1 — Foundations

## Video 1 — Why NestJS? What Problem It Solves

**▶ https://www.youtube.com/watch?v=K_OjtrsJGTk**

### The problem: Express gives you freedom, and freedom doesn't scale

The dominant Node.js backend framework has been **Express.js**:

```js
const express = require("express");
const app = express();

app.get("/users", (req, res) => {
  res.send("Users");
});
```

This is perfect for a small project — a handful of routes, one or two developers. But now picture the backend of Amazon, Uber, or a core banking system:

- 100+ endpoints
- 50+ engineers committing daily
- database connections, auth, caching, email, payments, logging, notifications

Express has no opinion on how any of that should be arranged.

### "Unopinionated" — what it actually means

Express doesn't tell you how to structure anything. Three developers on the same team can each do this and Express won't object:

```
Dev A                Dev B                Dev C
project/             project/             project/
 ├── routes           ├── api              └── everything.js
 ├── controllers      ├── business
 └── services         └── database
```

- **Advantage:** maximum flexibility, tiny learning curve.
- **Cost:** two years later, nobody can find anything. You end up with the classic archaeology layer:

```
controllers2/
controllers_new/
routes_v2/
new_routes/
helpers_final/
helpers_final_latest/
```

### NestJS is opinionated

NestJS's answer is: _"I'll give you the structure. Follow it."_ Every NestJS project on earth looks roughly the same:

```
src/
 ├── app.module.ts
 ├── users/
 │    ├── users.controller.ts
 │    ├── users.service.ts
 │    └── users.module.ts
 └── products/
      ├── products.controller.ts
      ├── products.service.ts
      └── products.module.ts
```

A new hire opens the repo and immediately knows:

| File       | Responsibility                                                       |
| ---------- | -------------------------------------------------------------------- |
| Controller | Receives HTTP requests, returns responses. No business logic.        |
| Service    | Business logic. Does the actual work.                                |
| Module     | Groups related controllers/services and declares their dependencies. |

That predictability — not raw performance — is the reason enterprises adopt it.

**Real-world analogy — hospitals.** If every hospital invented its own department names, a nurse transferring between them would be lost for weeks. Instead every hospital has Reception, Doctors, Pharmacy, Billing, Emergency. Walk into any one and you can work on day one. Express is "invent your own departments"; NestJS is the standard hospital layout.

### Architecture borrowed from Angular

NestJS deliberately copied Angular's ideas for the server side: **Modules, Providers/Services, Dependency Injection, Decorators, TypeScript-first.**

```ts
// Angular
@Injectable()
export class UserService {}

// NestJS — identical concept
@Injectable()
export class UserService {}
```

If you know Angular, NestJS will feel like home.

> **⚠️ Beyond the video — for anyone coming from Spring Boot**
> The Angular comparison only helps if you know Angular. The closer mental map is Spring:
>
> | NestJS                 | Spring Boot equivalent                         |
> | ---------------------- | ---------------------------------------------- |
> | `@Module`              | `@Configuration` + component scanning boundary |
> | `@Controller`          | `@RestController`                              |
> | `@Injectable` provider | `@Service` / `@Component`                      |
> | Nest DI container      | Spring IoC container                           |
> | Guards                 | Spring Security filters / `HandlerInterceptor` |
> | Pipes                  | argument resolvers + Bean Validation           |
> | Interceptors           | AOP around-advice                              |
> | Exception Filters      | `@ControllerAdvice` / `@ExceptionHandler`      |
>
> Decorators in Nest are the analogue of Java annotations — they attach metadata (via `reflect-metadata`) that the framework reads at startup to wire everything together.

### Why TypeScript matters here

Plain JavaScript will happily do the wrong thing:

```js
function add(a, b) {
  return a + b;
}
add("10", 20); // → "1020"  ...and no error
```

TypeScript catches it at compile time:

```ts
function add(a: number, b: number) {
  return a + b;
}
add("10", 20); // ✗ compiler error
```

On a 500-endpoint codebase with 50 contributors, this class of bug is the difference between a quiet Tuesday and a production incident.

### What you get out of the box

| Feature              | Express     | NestJS                                 |
| -------------------- | ----------- | -------------------------------------- |
| Routing              | ✅          | ✅                                     |
| Dependency Injection | ❌ manual   | ✅ built-in                            |
| Modules              | ❌          | ✅                                     |
| Validation           | extra setup | ✅ first-class                         |
| Testing              | extra setup | ✅ built-in (Jest + `@nestjs/testing`) |
| TypeScript           | optional    | ✅ default                             |
| Microservices        | extra work  | ✅ built-in                            |
| WebSockets           | extra work  | ✅ built-in                            |

### Dependency Injection — the single most important idea

Consider the dependency chain:

```
UserController → UserService → DatabaseService
```

Without DI you construct everything by hand:

```ts
const db = new DatabaseService();
const userService = new UserService(db);
const controller = new UserController(userService);
```

With Nest you just _declare what you need_ and the framework supplies it:

```ts
constructor(private readonly userService: UserService) {}
```

Nest looks at the constructor's type, finds the matching provider in the module, instantiates it once (singleton by default), and hands it over.

**Why this matters in practice:** in a unit test you swap `UserService` for a fake without touching the controller's code. That's the whole point — your classes depend on _types_, not on concrete construction. This is covered properly at Video 8.

### Modular architecture

A NestJS app is split by **feature**, not by technical layer:

```
src/
 ├── users/
 ├── products/
 ├── orders/
 ├── payments/
 └── reviews/
```

Each folder is a self-contained module with its own controller, service, and module file. Benefits: easier maintenance, isolated tests, independent scaling, fast onboarding — and a clean seam if you ever split a feature into its own microservice.

### The mental model to carry through the whole course

```
Client
  ↓
Controller      ← handles the HTTP layer only
  ↓
Service         ← business logic
  ↓
Repository / Database
```

Concretely, `GET /users`:

```
Browser → UsersController → UsersService → Database
Browser ← UsersController ← UsersService ←
```

Almost everything in NestJS is a variation on this flow. Later lectures insert extra stages (Guards, Pipes, Interceptors, Filters), but the spine never changes.

> **⚠️ Beyond the video — two honest caveats**
>
> 1. **NestJS is not a replacement for Express — it sits on top of it.** By default Nest uses `@nestjs/platform-express` under the hood; you can swap in `@nestjs/platform-fastify` for more throughput. Nest is an _architectural layer_, not a new HTTP server.
> 2. **It isn't free.** You pay in a compile step, a steeper learning curve, and more boilerplate per feature. For a 5-endpoint internal tool, Express or Fastify is genuinely the better call. Nest pays off when the team and the surface area grow.

### Interview questions from this lecture

**Q. What is NestJS?**
A progressive Node.js framework built with TypeScript for building scalable, maintainable server-side applications, using a modular architecture with dependency injection.

**Q. Why NestJS over Express?**
Nest supplies modular structure, DI, TypeScript by default, and built-in testing/microservices/WebSocket support. Express is more flexible but leaves architecture entirely to you.

**Q. Is NestJS built on Express?**
Yes — Express is the default HTTP platform, but Nest is platform-agnostic and can run on Fastify instead.

**Q. What's the single biggest advantage?**
The combination of modular architecture and dependency injection, which is what keeps large codebases maintainable and testable.

### Takeaway

```
Node.js                 (runtime)
   ↓
Express / Fastify       (basic HTTP framework)
   ↓
NestJS                  (structure, DI, and enterprise features on top)
```

Small project → Express is fine. Large, long-lived, multi-team project → NestJS earns its keep.

---

## Video 2 — Installation & Your First App with the CLI

**▶ https://www.youtube.com/watch?v=Hz7IFywSxJk**

Looks like "just installation," but it introduces several backend fundamentals worth getting right.

### The dependency stack

```
Computer → Node.js → npm → Nest CLI → NestJS Application
```

Like building a house: the land is your machine, Node.js is the workforce, npm is the toolshed, the Nest CLI is the architect, and the app is the house. Remove any lower layer and everything above collapses.

### 1. What Node.js actually is

The memorised line is "Node.js lets JavaScript run outside the browser." What's really going on: **Node.js is a runtime environment** — it embeds the V8 engine and adds the OS-level APIs that browsers deliberately withhold.

**Analogy.** You speak Hindi; the other person speaks only English. A translator sits between you. Node.js is that translator between JavaScript and the operating system.

Browser JavaScript can't touch the filesystem, open a TCP socket, or connect to a database. Node can:

```js
const fs = require("fs");
fs.readFile("data.txt", (err, data) => {
  console.log(data.toString());
});
```

That's why every Node backend framework — Express, Fastify, Nest — needs it:

```
NestJS → Express/Fastify → Node.js → Operating System
```

> **⚠️ Version gotcha.** NestJS 11 requires a modern Node LTS (Node 20+); Node 18 reached end-of-life in April 2025. If `nest new` fails with cryptic errors, check `node -v` first — a too-old Node is the most common cause. Verify the current minimum in the official docs, since this moves with each major release.

### 2. npm — the package manager

**npm = Node Package Manager.** Think Play Store / App Store, but for code libraries.

Without it you'd download source archives and resolve dependency trees by hand. With it:

```bash
npm install @nestjs/core
```

**Analogy.** Building a house, you don't manufacture your own bricks, cement, and doors — you buy them. Same with backend libraries.

**`package.json` is your shopping list:**

```json
{
  "name": "my-app",
  "dependencies": {
    "@nestjs/core": "^11.0.0"
  }
}
```

**`node_modules/` is the delivery.** `package.json` records what you _ordered_; `node_modules/` holds the actual _goods_ that `npm install` fetched.

> **⚠️ Beyond the video.** `node_modules/` must be in `.gitignore` — it's huge and reproducible. But **`package-lock.json` must be committed**: it pins the exact resolved versions so your machine, your teammate's machine, and the Railway build server all install byte-identical trees. Skipping this is the classic "works on my machine" bug.

### 3. The Nest CLI

**CLI = Command Line Interface.** Without it, every new feature means:

```bash
mkdir users
touch users.controller.ts users.service.ts users.module.ts
# ...and manually wire each one into the module
```

With it, one command scaffolds everything — files, module registration, and test stubs:

```bash
nest generate resource users     # or: nest g resource users
```

**Analogy.** Building furniture by hand-sawing and hand-drilling takes hours; with power tools it takes minutes. The CLI is your power tool.

**Installing it:**

```bash
npm install -g @nestjs/cli
```

Piece by piece: `npm` = the package manager · `install` = install a package · `-g` = globally, so the `nest` command works from any directory · `@nestjs/cli` = the package name.

> **⚠️ Beyond the video — prefer `npx` over a global install.**
> A global CLI silently drifts out of sync with your project's Nest version, which produces scaffolding that doesn't match your codebase. Safer:
>
> ```bash
> npx @nestjs/cli new my-app
> ```
>
> and inside an existing project, use the local copy so the CLI version always matches the project:
>
> ```bash
> npx nest g resource users
> ```

### 4. Creating the project

```bash
nest new my-app
```

What the CLI does, in order:

1. Creates `src/` and `test/` folders
2. Writes config files — `package.json`, `tsconfig.json`, `nest-cli.json`, ESLint/Prettier configs
3. Prompts for your package manager (npm / yarn / pnpm) and runs the install
4. Generates working starter code — a Hello World API that runs immediately

What you get:

```
src/
├── app.controller.ts
├── app.service.ts
├── app.module.ts
└── main.ts
```

Don't try to understand all four yet — Videos 3–7 break them down. For now:

```
main.ts → AppModule → Controller → Service
```

### 5. Running it

```bash
npm run start
```

`npm run <name>` executes the matching entry in `package.json`:

```json
{ "scripts": { "start": "nest start" } }
```

> **⚠️ Correction / the one thing to change immediately.**
> `npm run start` compiles once and runs — it does **not** reload when you edit a file, so you'll be restarting manually all day. For development always use watch mode:
>
> ```bash
> npm run start:dev
> ```
>
> The generated `package.json` also ships `start:debug` (watch + inspector) and `start:prod` (runs the compiled `dist/main`, used in deployment — see Video 50).

### 6. Ports

One machine runs many programs at once — Chrome, VS Code, Spotify, your Nest server. A **port** is how the OS decides which program an incoming request belongs to.

```
localhost:3000   localhost:5000   localhost:8000
```

**Analogy.** The building is your computer; ports are flat numbers. Flat 101 = port 3000, Flat 102 = port 5000. A courier arrives — the flat number decides who receives it.

> **⚠️ Beyond the video — the deployment trap.**
> The generated `main.ts` should read the port from the environment, not hardcode it:
>
> ```ts
> await app.listen(process.env.PORT ?? 3000);
> ```
>
> Hosts like Railway, Render, and Heroku inject a `PORT` variable and expect your app to bind to it. Hardcoding `3000` is the single most common reason a deploy "succeeds" but the URL returns nothing. This connects directly to Video 50.

### 7. What happens when you open localhost:3000

```
Browser → GET / → Nest Server → AppController → AppService → "Hello World!" → Browser
```

The generated code:

```ts
// app.controller.ts
@Get()
getHello(): string {
  return this.appService.getHello();
}

// app.service.ts
getHello(): string {
  return 'Hello World!';
}
```

Notice the controller does nothing except delegate. That thin-controller / fat-service split is the same flow introduced in Video 1, and it holds for every endpoint you'll ever write in Nest.

### Interview questions from this lecture

**Q. What is Node.js?** A JavaScript runtime environment that lets JavaScript execute outside the browser with access to OS-level APIs.
**Q. What is npm?** The Node Package Manager, used to install and manage project dependencies.
**Q. What is the Nest CLI?** A command-line tool that scaffolds and manages NestJS projects and their building blocks.
**Q. Why use it?** It automates setup and file generation, and keeps structure consistent across a team.
**Q. What does `nest new project-name` do?** Creates a new app, generates the initial structure, and installs dependencies.
**Q. What does `npm run start` do?** Runs the `start` script from `package.json`, which boots the Nest server.

### Mental model after Video 2

```
Node.js → npm → Nest CLI → Nest Project
                              ↓
                           main.ts
                              ↓
                          AppModule
                              ↓
                          Controller
                              ↓
                           Service
                              ↓
                          Response
```

`main.ts`, `AppModule`, Controller, and Service are still fuzzy — that's expected. Video 3 opens up the folder structure, and Videos 4–8 explain each building block properly.

---

## Video 3 — File & Folder Structure Explained

**▶ https://www.youtube.com/watch?v=XpVpoHLSTFg**

Most people skip straight to controllers and services, then get stuck on: _why is there a `dist`? why both `package.json` and `package-lock.json`? what actually happens when `npm install` runs?_ Worth ten minutes now.

### The whole tree

```
my-app/
├── dist/                 compiled JavaScript output
├── node_modules/         installed dependencies
├── src/                  your code — 95% of your time
├── test/                 end-to-end tests
├── .gitignore
├── nest-cli.json         Nest CLI settings
├── package.json          project blueprint
├── package-lock.json     exact dependency snapshot
├── tsconfig.json         TypeScript compiler settings
└── README.md
```

**Analogy — a company.** `src` is the staff actually doing work, `node_modules` is the warehouse of tools you bought, `dist` is the finished product shipped to customers, `package.json` is the company's registration document, and `.gitignore` says what never leaves the building.

### 1. `src/` — where you live

```
src/
├── main.ts
├── app.module.ts
├── app.controller.ts
└── app.service.ts
```

**Analogy — the kitchen.** Food gets prepared here; everything else in the project exists to support it.

As the app grows, `src/` is organised by feature, not by layer (the modular architecture from Video 1). A food-delivery app:

```
src/
├── users/
├── restaurants/
├── orders/
├── payments/
└── delivery/
```

### 2. `main.ts` — the entry point

The first file that runs.

```ts
async function bootstrap() {
  const app = await NestFactory.create(AppModule);
  await app.listen(3000);
}
bootstrap();
```

- **`NestFactory.create(AppModule)`** — walks the module graph starting from `AppModule`, instantiates every provider, resolves all dependencies, and builds the application instance. This is the DI container booting up.
- **`app.listen(3000)`** — binds the HTTP server to a port and starts accepting requests.

```
npm run start → main.ts → AppModule → Controllers → Services → app ready
```

**Analogy — a shopping mall.** Before any shop can serve customers, security unlocks the gate and the power comes on. `main.ts` is that opening sequence.

> **⚠️ Reminder from Video 2.** Use `app.listen(process.env.PORT ?? 3000)`, not a hardcoded `3000`. `main.ts` is also where you'd later add global pipes, CORS, and Swagger — it's the app-wide setup file.

### 3. `app.module.ts` — the root module

```ts
@Module({
  imports: [],
  controllers: [AppController],
  providers: [AppService],
})
export class AppModule {}
```

Every feature module eventually gets registered here, directly or transitively. Think of it as the org chart's root: Nest starts here and discovers the entire application from it. Modules get their own lecture at Video 6.

### 4. `app.controller.ts` — the receptionist

```ts
@Get()
getHello() {
  return this.appService.getHello();
}
```

Receives the request, delegates, returns the response. Notice it contains no logic of its own.

### 5. `app.service.ts` — the worker

```ts
getHello() {
  return 'Hello World';
}
```

The receptionist doesn't do the work; the worker does. This thin-controller / fat-service split is the flow from Video 1 and it holds everywhere:

```
Browser → GET / → Controller → Service → Response
```

### 6. `dist/` — compiled output

Node executes JavaScript, not TypeScript. So before running, your code is compiled:

```
src/users.service.ts  →  dist/users.service.js
```

**Analogy.** `src` is the blueprint; `dist` is the actual house. `npm run build` is the construction crew.

**Never edit files in `dist/`** — the next build overwrites them.

> **⚠️ Beyond the video — the stale-`dist` bug.** If you delete or rename a `.ts` file, its old compiled `.js` can linger in `dist/` and keep executing, producing "I deleted this code but it's still running" confusion. Nest's generated `nest-cli.json` sets `"deleteOutDir": true` to wipe `dist` before each build — if you ever hit ghost behaviour in production, this is the first thing to check.

### 7. `node_modules/` — the warehouse

Frequently 500 MB for a 20 MB project. Everything you install lands here, including Nest itself:

```
node_modules/
├── @nestjs/
├── express/
├── rxjs/
└── typescript/
```

**Never edit it by hand** — the next `npm install` discards your changes.

**Can you delete it?** Yes, safely. `npm install` rebuilds it from `package.json`. Deleting `node_modules` and reinstalling is a legitimate first-line fix for weird dependency errors.

### 8. `package.json` — the project's identity card

Covered in Video 2 as the shopping list; here's what interviewers actually probe.

**Dependencies** declare what the project needs:

```json
{ "dependencies": { "@nestjs/core": "^11.0.0" } }
```

**Scripts** are named shortcuts:

```json
{ "scripts": { "start": "nest start" } }
```

So `npm run start` executes `nest start`. You can add your own:

```json
{ "scripts": { "hello": "echo Hello Roshan" } }
```

```bash
npm run hello   # → Hello Roshan
```

> **⚠️ Worth knowing.** `dependencies` ship to production; `devDependencies` (TypeScript, Jest, ESLint, the CLI) are build/test-time only. Put a runtime package in the wrong bucket and it will work locally but crash on a production install.

### 9. `package-lock.json` — why it exists

This is the file beginners ignore and shouldn't.

In `package.json`:

```json
{ "express": "^5.0.0" }
```

The `^` means _"any compatible newer version."_ So today `npm install` gives you `5.0.1`; next month, `5.0.5`. Different machines, different versions — and you get:

```
Works on my machine 😎     Fails in production 😭
```

`package-lock.json` fixes this by recording the **exact resolved version of every package and every sub-dependency**, so everyone installs a byte-identical tree.

| `package.json`           | `package-lock.json`                |
| ------------------------ | ---------------------------------- |
| Declares what's required | Records exactly what was installed |
| Hand-edited              | Auto-generated                     |
| Small                    | Large                              |
| Blueprint                | Installation snapshot              |

**Analogy — ordering a laptop.** `package.json` says "1 laptop, 1 mouse, 1 keyboard." `package-lock.json` says "Dell Inspiron 15, serial XYZ123; Logitech M331; K380." Precise enough to reproduce the exact order.

> **⚠️ Beyond the video — `npm ci` beats `npm install` for builds.**
> On a build server or in Docker, use:
>
> ```bash
> npm ci
> ```
>
> It installs strictly from the lockfile, refuses to silently update anything, fails loudly if the lockfile and `package.json` disagree, and is faster. `npm install` may _modify_ the lockfile — which is precisely what you don't want in a reproducible build.

### 10. `.gitignore`

```gitignore
node_modules
dist
```

Both are large and fully reproducible from `package.json`, so they don't belong in version control.

**Analogy.** You share the recipe and the ingredient list — you don't ship the entire kitchen. `package.json` is enough; anyone can run `npm install` and recreate the rest.

### 11. `test/`

Contains the **end-to-end** tests (`app.e2e-spec.ts`) plus the Jest e2e config.

> **⚠️ Correction.** The video implies tests live in `test/`. Only e2e tests do. **Unit tests sit next to the code they test** inside `src/` — `nest g service users` produces `users.service.ts` _and_ `users.service.spec.ts` in the same folder. That co-location is deliberate: a unit test should move, and rot, together with its source file.

### 12. `nest-cli.json`

Settings the CLI reads when scaffolding and building — source root, whether to wipe `dist` before builds, asset copying, and (for larger setups) monorepo configuration with multiple apps and shared libraries. When `nest generate controller users` decides where to put the file, this is what it consults.

### 13. `tsconfig.json` — the file the video skips

Listed in the tree but never explained, and two of its settings are load-bearing:

```jsonc
{
  "compilerOptions": {
    "experimentalDecorators": true,
    "emitDecoratorMetadata": true, // ← this is what makes DI work
  },
}
```

`emitDecoratorMetadata` tells TypeScript to emit constructor **parameter types** into the compiled output. That's how Nest can read `constructor(private userService: UserService)` and know which provider to inject — without it, type-based dependency injection silently stops working. If DI ever fails with "cannot resolve dependency" on a fresh setup, check this first.

Nest also generates this config with `"strictNullChecks": false`, which is more permissive than most teams want. Tightening it early is much less painful than tightening it at 50 files.

### Interview questions from this lecture

**Q. If `node_modules` and `package-lock.json` are deleted, can the project be restored?**
Yes — `npm install` reads `package.json` and reinstalls everything.
_Nuance worth adding:_ you get a **working** project, but not necessarily an **identical** one. Without the lockfile, `^` ranges resolve to whatever is newest and compatible, so you may pick up different patch versions. That's exactly the risk the lockfile exists to eliminate.

**Q. If `package.json` is deleted but `node_modules` still exists?**
Much worse. `package.json` is the source of truth for which packages are direct dependencies and at what ranges; `node_modules` is a flat pile that doesn't distinguish what you asked for from what got pulled in transitively.

**Q. What gets committed to Git?**
`src/`, `package.json`, `package-lock.json`, configs. **Not** `node_modules/`, `dist/`, or `.env`.

### Production perspective

The repository holds source and manifests; the server reconstructs the rest:

```bash
npm ci          # install exactly what the lockfile says
npm run build   # TypeScript → dist/
npm run start:prod
```

This is precisely what Railway runs for you in Video 50.

### For your Spring background

| NestJS              | Maven/Gradle equivalent                     |
| ------------------- | ------------------------------------------- |
| `package.json`      | `pom.xml` / `build.gradle`                  |
| `package-lock.json` | dependency lock / resolved versions         |
| `node_modules/`     | `~/.m2` (but local to the project)          |
| `dist/`             | `target/`                                   |
| `npm ci`            | `mvn -o clean install` against a pinned set |

### Mental model after Video 3

```
src/                 your code
 ├── main.ts         starts the app
 ├── app.module.ts   root module
 ├── app.controller  receives requests
 └── app.service     business logic
node_modules/        installed libraries
dist/                compiled output
package.json         blueprint
package-lock.json    exact versions
tsconfig.json        compiler settings (DI depends on it)
.gitignore           what stays out of Git
test/                e2e tests
```

If you understand `src/`, `package.json`, and `package-lock.json`, you've covered most beginner-level structure questions. Videos 4–8 move on to the actual building blocks: Controllers, Services, Modules, and Dependency Injection.

---

## Video 4 — Controllers (and generating one with the CLI)

**▶ https://www.youtube.com/watch?v=yE2GvMqSuxQ**

This is where NestJS actually begins. Controllers are the first of the core building blocks, and getting them right makes everything after easier.

### What a controller is for

**Analogy — a restaurant.** A customer says "one pizza." The chef doesn't take the order; the **waiter** does, then passes it to the kitchen. In Nest the controller is the waiter — it receives requests and hands the actual work off.

A controller's job is exactly three things:

- receive HTTP requests
- route them to the right handler method
- return a response

It is **not** responsible for database queries, business logic, or calculations.

### Why not put the logic in the controller

Beginners write this:

```ts
@Controller("users")
export class UsersController {
  @Get()
  getUsers() {
    // database query
    // business logic
    // validation
    // calculations
    return users;
  }
}
```

A waiter who takes orders, cooks, washes dishes, and handles payment doesn't scale. The controller should delegate:

```ts
@Controller("users")
export class UsersController {
  constructor(private readonly userService: UserService) {}

  @Get()
  getUsers() {
    return this.userService.getUsers();
  }
}
```

Beyond tidiness, there's a concrete payoff: business logic in a service can be unit-tested without spinning up an HTTP server, and reused from a scheduled job or a queue consumer that has no HTTP request at all.

### `@Controller()` — the first decorator

A **decorator attaches metadata** to a class or method. It tells Nest to treat this class differently.

```ts
export class AppController {} // Nest sees: an ordinary class

@Controller()
export class AppController {} // Nest sees: a request handler
```

**Analogy — a signboard.** A building with no sign is just a building. Put "Hospital" on the front and everyone knows what happens inside. The decorator is the signboard.

At startup Nest walks the module graph from `AppModule`, reads these decorators via `reflect-metadata` (the mechanism enabled by `emitDecoratorMetadata` — see Video 3), and builds a route table.

### Route prefix

```ts
@Controller("users")
export class UsersController {}
```

The argument is a **base path**. Everything in this class now lives under `/users`.

### Route handlers and HTTP method decorators

```ts
@Controller("users")
export class UsersController {
  @Get()
  getUsers() {
    return "All Users";
  }
}
```

`GET /users` → `"All Users"`.

The method decorators map directly to HTTP verbs:

| Decorator        | Verb   | Meaning        | Example                         |
| ---------------- | ------ | -------------- | ------------------------------- |
| `@Get()`         | GET    | read           | `GET /users` — list users       |
| `@Post()`        | POST   | create         | `POST /users` — create a user   |
| `@Put(':id')`    | PUT    | replace        | `PUT /users/1` — replace user 1 |
| `@Patch(':id')`  | PATCH  | partial update | `PATCH /users/1`                |
| `@Delete(':id')` | DELETE | delete         | `DELETE /users/1`               |

The path passed to the method decorator is appended to the controller prefix:

```ts
@Controller("products")
export class ProductsController {
  @Get() getProducts() {} // GET /products
  @Get("featured") getFeatured() {} // GET /products/featured
  @Post() createProduct() {} // POST /products
}
```

> **⚠️ Beyond the video — route order matters, and this bites everyone once.**
> Nest matches routes **top to bottom**, first match wins. So this is broken:
>
> ```ts
> @Get(':id')      getOne() {}        // ← matches "featured" too!
> @Get('featured') getFeatured() {}   // ← unreachable, dead code
> ```
>
> A request to `/products/featured` hits `getOne()` with `id = "featured"`. **Always declare static routes before dynamic (`:param`) ones.** The symptom is confusing — the endpoint "exists" but returns the wrong handler's output.

> **⚠️ Beyond the video — what the video's handlers are missing.**
> `@Put(':id') updateUser() {}` declares a URL parameter but never reads it. To actually get at request data you need parameter decorators:
>
> ```ts
> @Put(':id')
> updateUser(@Param('id') id: string, @Body() body: UpdateUserDto) {}
> ```
>
> `@Param()`, `@Body()`, `@Query()`, `@Headers()` are covered properly in Videos 10–11. Just note that a route declaring `:id` without a `@Param('id')` is incomplete.

> **⚠️ Beyond the video — return values and status codes.**
> Whatever you return is automatically serialised to JSON; you don't touch `res.send()`. Default status is **200**, except `@Post()` which defaults to **201 Created**. Override with `@HttpCode(204)`. Handlers can also return a `Promise` or an RxJS `Observable` and Nest will resolve it before responding.

### Generating a controller with the CLI

```bash
nest g controller users
# long form: nest generate controller users
```

Creates:

```
src/users/
├── users.controller.ts
└── users.controller.spec.ts
```

…and registers it in the nearest module automatically:

```ts
@Module({ controllers: [UsersController] })
```

No manual wiring. Without the CLI you'd create the file, write the boilerplate, and remember to register it — every single time.

Useful flags: `--no-spec` skips the test file, `--flat` puts the file in the current folder instead of creating a subfolder.

Note that `users.controller.spec.ts` is a **unit test**, and it lands in `src/` next to the controller — not in `test/`. That's the co-location point from Video 3.

### Watch mode

Already flagged in Video 2, and the instructor rightly hammers it here: use

```bash
npm run start:dev
```

`npm run start` requires a manual restart after every edit; `start:dev` watches the filesystem and restarts automatically.

### Request lifecycle

```ts
@Get()
getUsers() {
  return ['John', 'Jane'];
}
```

```
Browser → GET /users → Nest server → route matching
       → UsersController.getUsers() → ["John","Jane"] → response
```

Every request in the app follows this shape; later lectures insert Guards, Pipes, Interceptors, and Filters into the middle of it.

### For your Spring background

| NestJS                 | Spring                                          |
| ---------------------- | ----------------------------------------------- |
| `@Controller('users')` | `@RestController` + `@RequestMapping("/users")` |
| `@Get()` / `@Post()`   | `@GetMapping` / `@PostMapping`                  |
| `@Param('id')`         | `@PathVariable("id")`                           |
| `@Body()`              | `@RequestBody`                                  |
| `@Query('q')`          | `@RequestParam("q")`                            |

Same idea throughout: annotations/decorators declare routing metadata, and the framework builds the dispatch table at startup.

### Interview questions from this lecture

**Q. What is a Controller?** A class that handles incoming HTTP requests and returns responses — the application's entry point.
**Q. What is `@Controller()`?** A class decorator marking the class as a controller and optionally setting a route prefix.
**Q. What is `@Get()`?** A method decorator mapping HTTP GET requests to a handler method.
**Q. Why keep business logic out of controllers?** Separation of concerns — controllers handle the HTTP layer only, services hold reusable, independently testable logic.
**Q. `start` vs `start:dev`?** `start` runs once; `start:dev` runs in watch mode with automatic restart.

### The one thing to remember

```
Client → Controller → Service → Database
```

Controller: ✅ receive requests · ✅ call services · ✅ return responses
Controller: ❌ database queries · ❌ business logic · ❌ calculations

Next up: Services (Video 5), then Modules (Video 6) — after which the foundation is complete.

---

## Video 5 — Services, @Injectable and Constructor Injection

**▶ https://www.youtube.com/watch?v=Cd-a0EUpj_8**

If the controller is the entry point (Video 4), the service is the brain. Between them they account for most NestJS interview questions.

### Before and after

Everything crammed into the controller:

```ts
@Controller("products")
export class ProductsController {
  @Get()
  getProducts() {
    const products = [
      { id: 1, name: "Laptop" },
      { id: 2, name: "Phone" },
    ];
    return products;
  }
}
```

Split properly — service holds the work:

```ts
@Injectable()
export class ProductsService {
  getAllProducts() {
    return [
      { id: 1, name: "Laptop" },
      { id: 2, name: "Phone" },
    ];
  }
}
```

```ts
@Controller("products")
export class ProductsController {
  constructor(private readonly productsService: ProductsService) {}

  @Get()
  getProducts() {
    return this.productsService.getAllProducts();
  }
}
```

Extending the restaurant analogy from Video 4: the waiter is the controller, the **chef is the service**. A waiter who cooks, and a chef who takes orders, both make the restaurant worse.

A service holds business logic, calculations, database queries, external API calls, and validation logic. In a real e-commerce app each feature gets one: `ProductsService`, `OrdersService`, `PaymentsService`, `UsersService`, `ReviewsService`.

### `@Injectable()` — what it actually does

```ts
@Injectable()
export class ProductsService {}
```

It marks the class as something the DI container can construct and hand out.

> **⚠️ Correction — a subtle but interview-worthy point.**
> The video says `@Injectable()` "registers the service with NestJS." It doesn't. **Registration happens in the module's `providers` array.** A class listed in `providers: [ProductsService]` is what makes it available for injection.
>
> What `@Injectable()` actually does is tell TypeScript to emit constructor **parameter type metadata** for that class (via `emitDecoratorMetadata`, Video 3), so Nest can resolve _the service's own_ dependencies. A service with no constructor dependencies technically works in `providers[]` without the decorator — but the moment you inject anything into it, it breaks with a confusing "cannot resolve dependency" error.
>
> **Rule: always add `@Injectable()` to every provider.** Just know that `providers: []` is what registers it, and that's the answer that shows you understand the mechanism.

### Where things get registered

```ts
@Module({
  controllers: [ProductsController],   // ← controllers here
  providers: [ProductsService],        // ← services here
})
```

For now: **service = provider**. Providers get their own treatment in Video 6/8 — the category is broader than just services (it also covers factories, values, and custom tokens).

### Dependency Injection

Without DI, a class builds its own dependencies:

```ts
export class ProductsController {
  private productService = new ProductsService(); // tightly coupled
}
```

That's hard to test (you can't substitute a fake), hard to replace, and every consumer creates its own copy.

With DI you declare what you need and Nest supplies it — note the absence of `new`:

```ts
constructor(private readonly productsService: ProductsService) {}
```

**Analogy — company laptops.** If every employee buys their own laptop, you get twenty different setups and no way to standardise or replace them. If the company issues laptops, provisioning is centralised and swapping one out is trivial. Nest creates, manages, and injects your objects the same way.

**How Nest resolves it at startup:**

```
ProductsController needs ProductsService
        ↓
Nest reads the constructor's parameter type metadata
        ↓
Looks up ProductsService in the module's providers
        ↓
Instantiates it (once) and injects the instance
```

### `private readonly` — what the keywords do

```ts
constructor(private readonly productsService: ProductsService) {}
```

This is TypeScript's **parameter property** shorthand: writing `private` or `readonly` on a constructor parameter automatically declares a class field _and_ assigns it. Without the shorthand you'd write:

```ts
private readonly productsService: ProductsService;
constructor(productsService: ProductsService) {
  this.productsService = productsService;
}
```

- **`private`** — accessible only inside the class. `this.productsService.getAllProducts()` works; `controller.productsService` from outside does not.
- **`readonly`** — can't be reassigned after construction. `this.productsService = new AnotherService()` is a compile error. Dependencies shouldn't change mid-flight.

> **⚠️ Beyond the video — providers are singletons.**
> By default Nest creates **one instance per application**, shared by every class that injects it. This has a direct consequence: **never store per-request state on a service** (a `currentUser` field, a request-scoped counter), because it will leak across concurrent requests from different users. Services should be stateless.
> Nest does offer `Scope.REQUEST` (new instance per request) and `Scope.TRANSIENT` (new instance per consumer), but request-scoping cascades up the dependency chain and hurts performance — reach for it only when you genuinely need it.

### Generating with the CLI

```bash
nest g service products
```

Creates `products.service.ts` and `products.service.spec.ts`, and adds the class to the module's `providers` array automatically.

### Route parameters

```ts
@Get(':id')
getProductById(@Param('id') id: string) {
  return this.productsService.getProductById(Number(id));
}
```

`/products/1` → Nest extracts `1` from the path and hands it over via `@Param('id')`.

### Why the conversion to number

**URL parameters always arrive as strings.** `/products/1` gives you `"1"`, not `1` — `typeof id` is `"string"`. So comparisons like `product.id === id` silently fail (`1 === "1"` is `false`), which is a classic first-week bug.

> **⚠️ Correction — don't use `Number(id)` in the handler.**
> `Number("abc")` returns `NaN` without throwing, so `/products/abc` sails through to your service and produces a confusing empty result or crash deeper in the stack. The idiomatic Nest solution is a **pipe**, which validates and transforms before the handler ever runs:
>
> ```ts
> @Get(':id')
> getProductById(@Param('id', ParseIntPipe) id: number) {
>   return this.productsService.getProductById(id);   // already a number
> }
> ```
>
> `/products/abc` now returns a clean `400 Bad Request` automatically, and your handler receives a properly typed `number`. Pipes are covered in Video 13 — but start using `ParseIntPipe` immediately.

### Full request lifecycle

```
Client → GET /products/1
       → route matches @Get(':id')
       → ProductsController.getProductById("1")
       → ProductsService.getProductById(1)
       → business logic
       → { "id": 1, "name": "Laptop" }
```

### Why this makes testing easier

```ts
calculateDiscount(price: number) {
  return price * 0.9;
}
```

Inside a controller, testing this means booting an HTTP server and firing a request. Inside a service, it's a plain method call:

```ts
expect(service.calculateDiscount(100)).toBe(90);
```

And because the controller receives its dependency through the constructor, a controller test can inject a fake service — Nest's `Test.createTestingModule({...}).overrideProvider(ProductsService).useValue(mock)` exists precisely for this. **That substitutability is the real payoff of DI**, not the reduced typing.

### For your Spring background

| NestJS                        | Spring                                 |
| ----------------------------- | -------------------------------------- |
| `@Injectable()`               | `@Service` / `@Component`              |
| `providers: [X]` in `@Module` | bean registration / component scan     |
| constructor injection         | constructor injection (identical idea) |
| singleton by default          | singleton scope by default             |
| `Scope.REQUEST`               | `@RequestScope`                        |

The mental model transfers almost exactly, including the "keep singletons stateless" discipline.

### Interview questions from this lecture

**Q. What is a Service?** A provider holding business logic, injectable into other classes via DI.
**Q. Why keep logic in services?** Separation of concerns, reusability across HTTP/jobs/queues, and testability without HTTP.
**Q. What is `@Injectable()`?** A decorator marking a class as a provider manageable by the DI container — with the nuance above that `providers[]` performs the registration.
**Q. What is constructor injection?** Dependencies declared as constructor parameters and supplied automatically by the framework.
**Q. Why `readonly`?** Prevents reassigning a dependency after injection.
**Q. Why `private`?** Restricts access to within the class.
**Q. What scope do providers have by default?** Singleton — one shared instance per application.

### The architecture to memorise

```
Customer → Waiter (Controller) → Chef (Service) → Kitchen Storage (Database)
```

A controller should never become a chef; a service should never become a waiter.

Next: Modules (Video 6) and Dependency Injection in depth (Video 8) — which together explain how Nest wires the whole graph at startup.

---

## Video 6 — Modules

**▶ https://www.youtube.com/watch?v=BQ_1hHJAlWM**

You have controllers and services. The open question: **how does Nest know which ones belong together, and where to look when resolving a dependency?** Modules are the answer, and they're the point where Nest stops resembling Express.

### The problem

A flat `src/` with 100+ files — every controller and service piled together — becomes unnavigable within months.

**Analogy — a shopping mall.** Shoes, food, electronics, clothes, and medicines dumped in one hall is unusable. Floor 1 electronics, Floor 2 clothing, Floor 3 food court is navigable. Modules are the floors.

A module is simply **a container that groups related controllers, providers, and other modules** — and, crucially, defines a DI boundary (more on that below).

### The `@Module()` decorator

```ts
@Module({
  controllers: [EmployeeController],
  providers: [EmployeeService],
})
export class EmployeeModule {}
```

| Key           | Meaning                                                              |
| ------------- | -------------------------------------------------------------------- |
| `controllers` | Controllers this module owns — their routes get registered           |
| `providers`   | Services/providers instantiated and available **inside this module** |
| `imports`     | Other modules whose exported providers this module needs             |
| `exports`     | Providers this module makes visible to modules that import it        |

The decorator is metadata, exactly like `@Controller()` and `@Injectable()` — it tells Nest what kind of class this is and how to wire it.

### `exports` — the part the video skips, and the #1 source of DI errors

The lecture covers `controllers`, `providers`, and `imports` but never mentions `exports`. That omission will cost you an afternoon, so here it is:

> **⚠️ Providers are private to their module by default.**
>
> Listing `EmployeeService` in `EmployeeModule`'s `providers` makes it injectable **only within `EmployeeModule`**. If `ProductService` (in a different module) tries to inject it, you get:
>
> ```
> Nest can't resolve dependencies of ProductService (?).
> Please make sure that the argument EmployeeService at index [0]
> is available in the ProductModule context.
> ```
>
> **Two things are required**, not one:
>
> ```ts
> // 1. the owning module must publish it
> @Module({
>   providers: [EmployeeService],
>   exports: [EmployeeService], // ← without this, nothing works
> })
> export class EmployeeModule {}
>
> // 2. the consuming module must import the module
> @Module({
>   imports: [EmployeeModule], // ← not the service, the module
>   providers: [ProductService],
> })
> export class ProductModule {}
> ```
>
> Note you import the **module**, never the service directly. And `imports` only grants access to what the imported module explicitly **exports** — not its entire `providers` list.

> **⚠️ For your Spring background — this is the big behavioural difference.**
> In Spring, any bean in the application context is injectable anywhere; there's no per-package visibility. Nest is the opposite: **modules encapsulate their providers**, and you opt into sharing via `exports`. This trips up almost every Spring developer moving to Nest, because the failure mode ("can't resolve dependencies") looks like a missing `@Injectable()` when it's really a missing `exports`.

### AppModule — the root

```ts
@Module({
  imports: [EmployeeModule],
})
export class AppModule {}
```

`main.ts` bootstraps `AppModule`; Nest then walks its `imports` recursively to discover the entire application.

**Analogy — a company.** `AppModule` is the CEO who knows every department; each department module knows its own staff.

```
AppModule
├── EmployeeModule → EmployeeController, EmployeeService
├── ProductModule  → ProductController,  ProductService
└── OrderModule    → OrderController,    OrderService
```

### Forgetting to import a module

If a module isn't reachable from `AppModule`'s import graph, Nest never loads it — its routes 404 and its providers don't exist. Classic beginner bug.

> **⚠️ Small correction.** The video presents importing into `AppModule` as a manual step. In practice `nest g module employee` **updates `AppModule`'s `imports` array for you**. The manual step only comes up when you move files around by hand or create modules without the CLI — worth knowing so you check rather than assume.

### Building a feature end to end

```bash
nest g module employee
nest g controller employee
nest g service employee
```

```
src/employee/
├── employee.module.ts
├── employee.controller.ts
└── employee.service.ts
```

The CLI wires all three: controller into `controllers`, service into `providers`, module into `AppModule.imports`.

```
AppModule → EmployeeModule → EmployeeController → EmployeeService
```

At startup: `main.ts` creates `AppModule` → sees `imports: [EmployeeModule]` → loads it → registers its controller's routes and instantiates its providers → `GET /employee` is live.

### Folder structure

Organise by **feature**, not by technical layer — the same point made in Videos 1 and 3, and this is where it becomes concrete:

```
src/
├── users/
│   ├── users.module.ts
│   ├── users.controller.ts
│   ├── users.service.ts
│   ├── dto/
│   └── entities/
└── products/
    └── ...
```

Grouping by layer (`controllers/`, `services/`) works at 5 files and falls apart at 50, because a single feature change means editing four distant folders.

### A module organises; it does not compute

Modules do **not** handle requests, calculate anything, or query databases. They only organise, register, and connect.

```
Controller = Waiter · Service = Chef · Module = the restaurant building
```

The building doesn't cook.

> **⚠️ Beyond the video — three module features you'll meet soon.**
>
> 1. **Dynamic modules** — `SomeModule.forRoot(config)` / `registerAsync(...)`. You've already seen them: `ThrottlerModule.forRoot()` (Video 49) and `JwtModule.registerAsync()` (Video 44). They're modules that take configuration and build themselves accordingly.
> 2. **`@Global()`** — marks a module's exports as available everywhere without importing it. Convenient for config, but it defeats encapsulation; use it sparingly, as the Nest docs themselves advise.
> 3. **Circular dependencies** — when two modules import each other, wrap both sides in `forwardRef(() => OtherModule)`. Usually a hint that a shared piece should be extracted into a third module instead.

### Interview questions from this lecture

**Q. What is a Module?** A class decorated with `@Module()` that groups related controllers and providers and defines a DI boundary.
**Q. Why do we need them?** Organisation, maintainability, scalability, and scoped dependency management.
**Q. What is `AppModule`?** The root module — the entry point from which Nest builds the dependency graph.
**Q. What does `imports` do?** Makes another module's **exported** providers available in this module.
**Q. What happens if a module isn't imported?** Nest never loads it; its routes and providers don't exist.
**Q. How do you share a service between two modules?** Export it from the owning module and import that module where it's needed. _(This is the question the video leaves you unable to answer.)_

### Mental model after Video 6

```
AppModule
    ├── EmployeeModule
    │      ├── EmployeeController
    │      └── EmployeeService   (exported if others need it)
    ├── ProductModule
    └── OrderModule
```

Module = container and DI boundary. Controllers and services do the work; the module decides what exists and who can see it.

Next: Video 7 zooms out to the overall architecture, and Video 8 covers Dependency Injection properly.

---

## Video 7 — Architecture (consolidation)

**▶ https://www.youtube.com/watch?v=o6V8xzEhDPA**

This is a **revision lecture** — it re-explains Controllers, Services, Modules, DI, and Decorators to assemble them into one picture. Since all five are already covered above, this section stays short and covers only what's genuinely new: the **startup sequence** and the **provider vs service** distinction.

### The architecture, assembled

```
main.ts → AppModule → Feature Module → Controller → Service (Provider) → Database
                                            ↑            ↓
                                        response ← business logic
```

Restaurant version: Customer → Waiter (Controller) → Chef (Service) → Kitchen Storage (Database), all inside the Restaurant (Module).

A realistic enterprise tree:

```
AppModule
├── UsersModule    → UsersController,    UsersService
├── ProductsModule → ProductsController, ProductsService
├── OrdersModule   → OrdersController,   OrdersService
└── PaymentsModule → PaymentsController, PaymentsService
```

**Controller vs Service** (a standing interview question):

| Controller                        | Service                      |
| --------------------------------- | ---------------------------- |
| Receives requests, handles routes | Business logic, calculations |
| Returns responses                 | Talks to the database        |
| Thin                              | Thick                        |

> **⚠️ Mild caution on "fat service."** The video's framing is right — logic belongs in the service, not the controller. But a service that grows to 1,500 lines is its own problem. In real projects logic gets split further: repositories for data access, domain/helper classes for rules, the service orchestrating between them. "Fat" means _relative to the controller_, not _unbounded_.

### What actually happens at startup

1. `main.ts` runs, calling `NestFactory.create(AppModule)`
2. Nest instantiates `AppModule`
3. It walks `imports` recursively, loading every reachable module
4. Each module registers its `controllers` and `providers`
5. Nest builds the **dependency graph** — reading constructor parameter metadata to work out that `EmployeeController` needs `EmployeeService`, and in what order to instantiate things
6. Routes are registered and `app.listen()` starts accepting requests

Everything is resolved **at startup, not per request**. That's why a wiring mistake (a missing `exports`, a circular dependency) crashes the app on boot rather than failing silently later — a genuinely good property.

### Provider vs Service — the one new idea here

The video says "services are providers, and the reverse isn't always true." That's correct and worth unpacking, because _provider_ is the broader category:

> **A provider is anything registered in a module's `providers` array that the DI container can inject.**

`EmployeeService`, `AuthService`, `EmailService`, `LoggerService` are all providers that happen to be services. But a provider doesn't have to be a class you wrote:

```ts
@Module({
  providers: [
    // 1. shorthand — "useClass" with the class as its own token
    EmployeeService,

    // 2. useValue — inject a plain object or constant
    { provide: 'APP_CONFIG', useValue: { retries: 3, region: 'ap-south-1' } },

    // 3. useClass — swap the implementation behind a token
    { provide: EmailService, useClass: SendGridEmailService },

    // 4. useFactory — compute the provider, with its own dependencies
    {
      provide: 'DB_CONNECTION',
      useFactory: (config: ConfigService) => createConnection(config.get('DB_URL')),
      inject: [ConfigService],
    },
  ],
})
```

`useClass` is what makes testing and environment-swapping clean: point `EmailService` at a real implementation in production and a no-op in tests, and **no consumer changes**. That's the payoff DI was promising back in Video 5.

> **⚠️ Beyond the video — you cannot inject a TypeScript interface, and this surprises Spring developers.**
> Interfaces are erased at compile time, so there's no runtime token for Nest to match against. This does **not** work:
>
> ```ts
> constructor(private mailer: IEmailService) {}   // ✗ no runtime type
> ```
>
> Use a string or symbol token instead:
>
> ```ts
> // module
> { provide: 'EMAIL_SERVICE', useClass: SendGridEmailService }
>
> // consumer
> constructor(@Inject('EMAIL_SERVICE') private mailer: IEmailService) {}
> ```
>
> In Spring you'd inject `EmailService` (the interface) directly and let the container pick the implementation. In Nest, injection is by **token**, and a class is only usable as a token because classes survive to runtime. Prefer exported `const` tokens over raw strings so typos become compile errors.

### Decorators, recapped

`@Controller()`, `@Injectable()`, `@Module()`, `@Get()/@Post()/...` are all metadata labels. Nest reads them at startup (via `reflect-metadata` — see the `emitDecoratorMetadata` note in Video 3) to decide what each class is and how to wire it.

### Interview questions from this lecture

**Q. Describe NestJS architecture.** Modular: modules group controllers and providers; controllers handle HTTP; providers hold logic; DI wires them at startup.
**Q. What is a provider?** Anything registered in `providers` that the DI container can inject — services, factories, values, or alternative class implementations.
**Q. Is every provider a service?** No. Every service is a provider; providers also include `useValue`, `useFactory`, and `useClass` registrations.
**Q. When is the dependency graph built?** At application startup, not per request.

---

## Video 8 — Dependency Injection in depth

**▶ https://www.youtube.com/watch?v=Fgikn8N_mus**

DI was introduced in Video 5 and revisited in Video 7, so this section covers only what this lecture adds: **why** DI exists (three concrete problems), the DI container, loose coupling, and how to debug resolution failures.

### The three problems DI solves

**1. Tight coupling — manual construction doesn't scale.** With `new`, every class must know how to build its entire dependency chain:

```ts
const logger = new LoggerService();
const redis = new RedisService(logger);
const db = new DatabaseService(redis);
const service = new ProductService(db);
const ctrl = new ProductController(service);
```

Add one constructor argument three levels down and every call site breaks. With DI you declare `constructor(private readonly productService: ProductsService) {}` and Nest resolves the whole chain.

**2. Testing.** If a class news up its own dependencies, you can't substitute a fake database — the real one gets called in your unit tests. Injected dependencies can be swapped (Video 5's `overrideProvider`, Video 7's `useClass`).

**3. Duplicate objects.** Three controllers each doing `new LoggerService()` produce three loggers, three connection pools, three of everything.

> **⚠️ Nuance on problem 3.** DI doesn't merely reduce the duplication — providers are **singletons** (Video 5), so all three controllers receive _the same instance_. That's the point, and it's also why services must stay stateless.

### Analogies

**Water supply.** Without DI, every room fetches its own water from the river in buckets. With DI, a pipeline is installed and the kitchen, bathroom, and garden taps just deliver. Nest is the pipeline.

**Company IT.** Employees don't each buy their own laptop; they request one and IT provisions it — standardised, managed, replaceable.

### The vocabulary

- **Dependency** — anything a class needs. `ProductsController` needs `ProductsService`, so the service is its dependency.
- **Injection** — supplying it automatically instead of constructing it.
- **Dependency Injection** — the design pattern where dependencies are provided rather than created.
- **DI container** — Nest's registry of everything it can construct and hand out.

```
DI Container
├── ProductsService
├── UsersService
├── OrdersService
└── LoggerService
```

### How resolution actually works

```
main.ts → AppModule → ProductsModule
        → module registers providers: [ProductsService] into the container
        → Nest constructs ProductsController
        → reads its constructor parameter metadata: needs ProductsService
        → looks it up in the container → instantiates once → injects
```

### The clarification this lecture gets right

The notes end with an important correction to what Videos 5 and 7 implied:

> Registering the provider in the module's `providers` array matters just as much as `@Injectable()`. Without the module registration, Nest cannot inject it.

That matches the correction flagged back in Video 5 — `@Injectable()` marks a class as injectable; `providers: [...]` is what actually registers it. Both are required in practice, and knowing which does what is the interview-grade answer.

### Loose coupling — with an honest caveat

Without DI, the controller knows exactly how its dependency is constructed. With DI it only knows _that it needs one_, not how, when, or by whom it was built.

> **⚠️ Beyond the video — "loose coupling" is oversold here.**
> Writing `constructor(private svc: ProductsService)` still names a **concrete class**. Your controller is decoupled from _construction_, but not from _implementation_ — swap in a different product service and the type annotation has to change.
> Genuine implementation-level decoupling needs a token (Video 7):
>
> ```ts
> constructor(@Inject('PRODUCTS_SERVICE') private svc: IProductsService) {}
> ```
>
> Now the module decides the implementation and the consumer never names it. Most Nest codebases don't bother — injecting the concrete class is idiomatic and fine — but be precise about which kind of coupling you've actually removed, because interviewers do probe this.

### Debugging DI failures

The error you'll meet most often:

```
Nest can't resolve dependencies of the ProductsController (?).
Please make sure that the argument ProductsService at index [0]
is available in the ProductsModule context.
```

Read it precisely: the **`?`** marks the constructor position that failed, and `index [0]` names which argument. Three causes, in order of likelihood:

1. The provider isn't in that module's `providers` array
2. It lives in another module that doesn't **`export`** it, or you didn't `imports` that module (Video 6)
3. A circular dependency between two modules or providers — wrap both sides in `forwardRef(() => Other)`, though usually the better fix is extracting the shared piece into a third module

### Two lesser-used forms

- **Property injection** — `@Inject(X) private x: X;` as a field instead of a constructor parameter. Occasionally needed in base classes; constructor injection is the default everywhere else.
- **Optional dependencies** — `constructor(@Optional() private logger?: LoggerService) {}` resolves to `undefined` instead of throwing when the provider is absent.

### Interview questions from this lecture

**Q. What is Dependency Injection?** A pattern where dependencies are supplied by a container instead of constructed by the consumer.
**Q. What problems does it solve?** Tight coupling, untestability, and duplicate instances.
**Q. What is a dependency?** Any object a class requires to do its job.
**Q. What is the DI container?** Nest's registry of providers, built at startup, that resolves and supplies instances.
**Q. What is loose coupling?** Depending on something you didn't construct — and, done properly, on an abstraction rather than a concrete class.
**Q. Why does `@Injectable()` alone not suffice?** Registration happens through the module's `providers` array; the decorator only enables the class's own dependencies to be resolved.

### The one-sentence summary

> Dependency Injection lets controllers and other classes receive services automatically, without constructing them.

Everything later — Guards, Interceptors, Repositories, Auth services — is wired through this same container, which is why it's worth over-learning now.

---

## Video 9 — REST, HTTP Methods & Postman

**▶ https://www.youtube.com/watch?v=Uyk6bwm2eWI**

This lecture steps outside NestJS to teach general backend vocabulary. Kept short here, with the additions concentrated on the parts that get asked about in interviews and gotten wrong in code.

### API and REST, quickly

An **API** is the controlled interface between a client and a backend. The reason it exists isn't convenience — it's that the alternative (a frontend talking straight to the database) hands every user the ability to read passwords and delete rows. The backend mediates: it authenticates, authorises, validates, and only then touches data.

**REST** (Representational State Transfer) is a set of conventions for designing those APIs. It exists because without conventions you get `/getUsers`, `/fetchUsers`, and `/showAllUsers` in the same codebase.

A **resource** is a noun the API exposes — `/users` is the collection, `/users/1` a single member.

**Naming rules worth following:** plural nouns, no verbs in paths (the HTTP method _is_ the verb), and nesting for relationships:

```
✅ GET /users          ❌ GET /getUsers
✅ GET /users/1/orders ❌ GET /getOrdersByUser?id=1
```

### CRUD → HTTP → NestJS

| CRUD             | HTTP   | Nest decorator           | Example                      |
| ---------------- | ------ | ------------------------ | ---------------------------- |
| Create           | POST   | `@Post()`                | `POST /users` + body         |
| Read             | GET    | `@Get()` / `@Get(':id')` | `GET /users`, `GET /users/1` |
| Update (full)    | PUT    | `@Put(':id')`            | replaces the whole record    |
| Update (partial) | PATCH  | `@Patch(':id')`          | changes only the fields sent |
| Delete           | DELETE | `@Delete(':id')`         | `DELETE /users/1`            |

### PUT vs PATCH

Given `{ id: 1, name: "Roshan", email: "roshan@gmail.com", age: 30 }`:

- `PUT /users/1` with `{ name: "Rahul", email: "rahul@gmail.com", age: 25 }` **replaces** the record.
- `PATCH /users/1` with `{ age: 31 }` changes **only** `age`.

> **⚠️ Beyond the video — idempotency is the follow-up question.**
> "PUT is full, PATCH is partial" is the answer everyone gives. The distinction interviewers actually probe is **idempotency**: making the same request twice has the same effect as making it once.
>
> | Method | Safe (no change) | Idempotent      |
> | ------ | ---------------- | --------------- |
> | GET    | ✅               | ✅              |
> | PUT    | ❌               | ✅              |
> | DELETE | ❌               | ✅              |
> | POST   | ❌               | ❌              |
> | PATCH  | ❌               | not necessarily |
>
> `POST /orders` twice creates two orders — that's why double-clicking "Pay" is dangerous and why the payment endpoint got a strict rate limit in Video 49. `PUT /users/1` twice leaves exactly one user in the same state.

> **⚠️ Beyond the video — most "PUT" implementations are actually PATCH.**
> Strictly, PUT _replaces_: fields absent from the body should be cleared or reset, not left alone. Plenty of real code merges instead, which quietly makes PUT behave like PATCH and surprises API consumers. Either implement replacement properly, or expose PATCH and skip PUT — the latter is what most modern APIs do.

Status codes for these routes were covered in Video 4: `@Post()` returns **201** by default, everything else **200**, and `204 No Content` is the conventional response to a successful DELETE.

### Statelessness

Each request is independent — the server keeps no memory of previous requests, so every request must carry everything needed to process it.

> **⚠️ Worth being precise.** "Stateless" doesn't mean _no authentication_ or _no state anywhere_. It means the **server holds no per-client session state between requests**. The state lives with the client and is presented each time — which is exactly what the `Authorization: Bearer <token>` header does in Video 44. That's the whole appeal of JWT over server-side sessions.
>
> Why it matters practically: any instance can serve any request, so you can scale horizontally behind a load balancer. And note the counter-example you've already seen — the throttler's default **in-memory** request counters (Video 49) _are_ server-side state, which is precisely why they break across multiple instances and need Redis.

### Postman

Needed because you can't easily issue POST/PUT/PATCH/DELETE by typing into a browser address bar. Postman lets you choose the method, set headers, attach a JSON body, and manage auth tokens.

> **⚠️ Small correction.** The video says browsers "mainly support GET." Browsers can issue every HTTP method via `fetch`/`XHR`, and HTML forms support GET and POST. The accurate statement is narrower: **the address bar only issues GET**, so manual testing of other verbs needs a tool. Postman, Insomnia, Bruno, VS Code's REST Client, or plain `curl` all work.

### Request lifecycle

```
POST /users → route matches @Post() → controller → service → persistence → response
```

Same spine as every previous lecture; the only new element is that POST carries a **body**, which the next lectures teach you to extract (`@Body()`) and validate (DTOs, Video 11–12).

### Interview questions from this lecture

**Q. What is an API?** A defined interface letting systems exchange data and functionality without exposing internals.
**Q. What is REST?** An architectural style for stateless APIs built on standard HTTP methods and resource-based URLs.
**Q. What is statelessness?** The server stores no client session between requests; each request carries everything needed.
**Q. PUT vs PATCH?** Full replacement vs partial update — and PUT is idempotent while PATCH need not be.
**Q. Which methods are idempotent?** GET, PUT, DELETE (and HEAD/OPTIONS). POST is not.

---

## Video 10 — Building a Complete CRUD API

**▶ https://www.youtube.com/watch?v=w9JYelWOSj4**

First lecture where everything assembles into a working API. A Student Management System with an in-memory array standing in for a database.

### Setup

```bash
nest g module student
nest g controller student
nest g service student
```

The array lives on the service:

```ts
@Injectable()
export class StudentService {
  students = [
    { id: 1, name: "Roshan", age: 30 },
    { id: 2, name: "Rahul", age: 28 },
  ];
}
```

> **⚠️ Note on the fake database.** This is mutable state on a singleton provider — exactly what Video 5 warned against. Here it's deliberate, but be clear about the consequences: **the data resets on every restart** (including every `start:dev` reload), and with two instances behind a load balancer each would hold its own divergent copy. That's the whole reason Videos 21+ move to MongoDB.

### The two new decorators

| Decorator      | Reads from          | `PATCH /student/1` with `{"age":31}` |
| -------------- | ------------------- | ------------------------------------ |
| `@Param('id')` | the URL path        | `"1"`                                |
| `@Body()`      | the request payload | `{ age: 31 }`                        |

`@Query()` and `@Headers()` come later (Video 41 covers query-based filtering).

### The five operations

```ts
// GET /student
getStudents() { return this.students; }

// GET /student/:id
getStudentById(id: number) {
  return this.students.find(s => s.id === id);
}

// POST /student
createStudent(student) {
  this.students.push(student);
  return student;
}

// PUT /student/:id — replace
const index = this.students.findIndex(s => s.id === id);
this.students[index] = body;

// PATCH /student/:id — merge
const student = this.students.find(s => s.id === id);
Object.assign(student, updateData);

// DELETE /student/:id
this.students = this.students.filter(s => s.id !== id);
```

`Object.assign(target, source)` copies the source's keys onto the target, leaving untouched fields intact — which is precisely PATCH semantics.

Route params arrive as strings, hence `Number(id)` — but use `ParseIntPipe` instead, as corrected in Video 5.

### The controller template

```ts
@Controller("student")
export class StudentController {
  constructor(private readonly studentService: StudentService) {}

  @Get() getStudents() {}
  @Get(":id") getStudentById() {}
  @Post() createStudent() {}
  @Put(":id") updateStudent() {}
  @Patch(":id") patchStudent() {}
  @Delete(":id") deleteStudent() {}
}
```

You'll write this shape hundreds of times. Note `@Get()` sits above `@Get(':id')` — static before dynamic, per Video 4.

---

### ⚠️ Five bugs in this implementation

The video's code runs, but it's broken in ways worth fixing before you build on it.

**1. `createStudent` never assigns an `id` — this one is fatal.**
The service pushes the request body straight into the array, so the new record has `{ name, age }` and **no `id`**. Every subsequent operation on that student silently fails: `getStudentById` can't find it, PATCH can't find it, DELETE can't remove it. Fix:

```ts
createStudent(student: CreateStudentDto) {
  const newStudent = { id: this.nextId++, ...student };
  this.students.push(newStudent);
  return newStudent;
}
```

Never let the client supply the primary key.

**2. Missing records return `200 OK` with an empty body, not `404`.**
`find()` returns `undefined`, and Nest serialises that as an empty 200 response. Callers can't distinguish "no such student" from "student with no data":

```ts
getStudentById(id: number) {
  const student = this.students.find(s => s.id === id);
  if (!student) throw new NotFoundException(`Student ${id} not found`);
  return student;
}
```

`NotFoundException` is available from `@nestjs/common` right now — you don't need to wait for exception filters (Video 16). The same applies to PUT, PATCH, and DELETE.

**3. `this.students[index] = body` when `index === -1` is a silent JavaScript trap.**
`findIndex` returns `-1` for a missing id, and `arr[-1] = value` doesn't throw — it attaches a `"-1"` **property** to the array without changing its length or contents. So `PUT /student/999` returns success while doing nothing. Guard the index before assigning.

**4. `@Body() body` is untyped, so the API accepts literally anything.**
`body` is `any`. `POST /student` with `{"nonsense": true}`, a bare string, or a 10 MB payload all sail through into your data. The fix is DTOs plus a validation pipe — Videos 11 and 12, and this is exactly the gap they exist to close.

**5. PATCH lets a client rewrite the primary key.**
`Object.assign(student, updateData)` copies _every_ key from the body. `PATCH /student/1` with `{"id": 999}` changes the student's id, corrupting the collection. Once DTOs are in place, `ValidationPipe({ whitelist: true, forbidNonWhitelisted: true })` strips or rejects unexpected properties. Until then, pick the fields explicitly rather than blanket-assigning.

---

### What the lecture is really teaching

Beyond CRUD mechanics, three durable ideas:

1. **Request data has several sources** — path (`@Param`), body (`@Body`), query string, headers. Knowing which decorator reads which is most of request handling.
2. **Controller/service separation holds even for trivial logic** — the controller extracts and delegates; the service decides.
3. **RESTful routing is a fixed pattern** — `GET /x`, `GET /x/:id`, `POST /x`, `PATCH /x/:id`, `DELETE /x/:id`.

### The production version

Only the service's internals change when a real database arrives:

```ts
getStudents() { return this.studentRepository.find(); }   // TypeORM
getStudents() { return this.prisma.student.findMany(); }  // Prisma
getStudents() { return this.studentModel.find(); }        // Mongoose
```

Controller, module, decorators, and routing stay identical — which is the payoff of having kept logic out of the controller.

### Interview questions from this lecture

**Q. `@Param()` vs `@Body()`?** Path values vs request payload.
**Q. Why `Number(id)`?** Route params are always strings; comparison with `===` against a numeric id fails otherwise. Better: `ParseIntPipe`.
**Q. PUT vs PATCH in code?** PUT replaces the array element; PATCH merges via `Object.assign`.
**Q. Which decorator handles POST?** `@Post()`.

---

## Video 11 — DTOs & Interfaces

**▶ https://www.youtube.com/watch?v=E3TbXT2TR5Q**

Directly addresses bug #4 from Video 10: `@Body() body` accepts anything at all.

### What a DTO is

**DTO = Data Transfer Object** — a declaration of what data is allowed to travel from client to server.

**Analogy — a passport application.** The form asks for name, date of birth, and address. Submit "favourite cricket team" alongside and it's ignored, because the form defines what's accepted. A DTO is that form.

```
src/customer/
├── dto/
│   └── create-customer.dto.ts
├── interfaces/
│   └── customer.interface.ts
├── customer.controller.ts
├── customer.service.ts
└── customer.module.ts
```

```ts
export class CreateCustomerDto {
  name: string;
  email: string;
  age: number;
}
```

```ts
@Post()
createCustomer(@Body() createCustomerDto: CreateCustomerDto) {
  return this.customerService.create(createCustomerDto);
}
```

Compared to `@Body() body`, you gain a self-documenting parameter name, editor autocomplete, and a compile error if you reference `createCustomerDto.salary`.

### Why a class, not an interface

Because decorators can't be applied to interfaces, and validation (Video 12) is decorator-driven:

```ts
export class CreateCustomerDto {
  @IsString()
  name: string;
}
```

The deeper reason: **interfaces are erased at compile time and emit no JavaScript at all.** A class survives to runtime, so `ValidationPipe` has an actual constructor to inspect via `emitDecoratorMetadata` (Video 3). This is the same runtime-erasure fact behind not being able to inject an interface (Video 7) — one language rule, showing up in two places.

### Interfaces

A TypeScript contract describing an object's shape:

```ts
export interface Customer {
  id: number;
  name: string;
  email: string;
  age: number;
}
```

```ts
customers: Customer[] = [];
```

Now `this.customers.push({ id: 1, name: 'Roshan' })` is a compile error — `email` and `age` are missing. Without the annotation, `customers = []` is `any[]` and TypeScript checks nothing.

### DTO vs Interface

| DTO                              | Interface                     |
| -------------------------------- | ----------------------------- |
| Defines incoming request data    | Defines an object's shape     |
| A class — exists at runtime      | Erased at compile time        |
| Supports decorators / validation | Cannot carry decorators       |
| Used at the controller boundary  | Used anywhere in the codebase |

### Why keep them separate

Request shape and stored shape genuinely differ:

```ts
// what the client may send
export class CreateCustomerDto {
  name: string;
  email: string;
}

// what your system stores
export interface Customer {
  id: number;
  name: string;
  email: string;
  createdAt: Date;
  updatedAt: Date;
}
```

`id`, `createdAt`, and `updatedAt` are **server-generated**. Leaving them out of the DTO is what stops a client from setting its own primary key — the exact vulnerability flagged as bug #5 in Video 10.

### The limitation the lecture correctly admits

The video says outright that a bare DTO validates nothing, and that's the single most important sentence in it. Worth stating precisely:

> **⚠️ TypeScript types do not exist at runtime.**
> `@Body() dto: CreateCustomerDto` gives you **editor-time** safety only. At runtime the parameter is whatever JSON arrived — Nest performs no checking and no filtering. So this still passes straight through:
>
> ```json
> { "name": 123, "age": "hello", "isAdmin": true }
> ```
>
> The DTO is a **shape declaration** until Video 12 attaches `class-validator` decorators and a `ValidationPipe`. And note that extra properties are **not** stripped by default — that requires `new ValidationPipe({ whitelist: true })`. Calling a plain DTO a "security guard" is aspirational; right now it's a name tag.

---

### ⚠️ Two problems in this implementation

**1. `id: this.customers.length + 1` produces duplicate ids.**
It works only while nothing is ever deleted:

```
[{id:1}, {id:2}, {id:3}]   → delete id 2 → [{id:1}, {id:3}]
length = 2 → next id = 3   → collision with the existing id 3
```

Now two customers share an id and every lookup returns the wrong one. The video's later example uses `Date.now()`, which is better but still collides for two requests inside the same millisecond. Use a monotonic counter, a UUID, or — once you reach Videos 21+ — let the database assign it.

**2. There's no `UpdateCustomerDto`, and hand-writing one duplicates the create DTO.**
Nest ships mapped types for exactly this:

```ts
import { PartialType } from "@nestjs/mapped-types";

export class UpdateCustomerDto extends PartialType(CreateCustomerDto) {}
```

Every field becomes optional while keeping its validation rules — correct PATCH semantics for free. `PickType`, `OmitType`, and `IntersectionType` cover the other combinations. Add one field to the create DTO and the update DTO follows automatically.

> **⚠️ Beyond the video — DTOs on the way out, too.**
> This lecture covers input only. Returning your stored object directly leaks whatever it contains — which becomes urgent in Video 44, where the customer record holds a **password hash**. Two options: map to an explicit response type, or mark fields with `@Exclude()` and enable `ClassSerializerInterceptor`. Decide before you have an auth system, not after.

### For your Spring background

`CreateCustomerDto` with `@IsString()` is the direct analogue of a request DTO/record with Bean Validation annotations, and `ValidationPipe` plays the role of `@Valid`. The entity-vs-DTO separation discipline is identical. The one thing with no Java equivalent is interface erasure — Java interfaces exist at runtime, which is why Spring can inject and reflect over them and Nest cannot.

### Interview questions from this lecture

**Q. What is a DTO?** An object defining the structure of data transferred between client and server.
**Q. Why use DTOs?** Consistent request contracts, readability, type safety, and a place to hang validation rules.
**Q. What is an interface?** A compile-time TypeScript contract describing an object's shape.
**Q. DTO vs interface?** DTOs are runtime classes at the request boundary carrying validation; interfaces are erased type declarations.
**Q. Why must DTOs be classes?** Validation needs runtime metadata, and only classes survive compilation.
**Q. Does a DTO alone validate anything?** No — not without `class-validator` decorators and a `ValidationPipe`.

### Mental model after Video 11

```
Client → Controller (@Body() CreateCustomerDto) → Service → Customer (interface) → storage
```

Input shape and stored shape are now distinct types. Video 12 makes the input shape actually enforced.

---

## Video 12 — Validating DTOs with class-validator & ValidationPipe

**▶ https://www.youtube.com/watch?v=IIKZVHy1Dqw**

The lecture that turns the Video 11 DTO from a name tag into an actual gate. This one is accurate — the additions below are things it leaves out rather than corrections.

### Why a bare DTO validates nothing

Covered in Video 11: TypeScript types are erased at compile time. `name: string` emits no JavaScript, so at runtime Nest has no idea `age` was supposed to be a number.

**Analogy — airport security.** The DTO is the signboard listing what's allowed through. Without a guard reading it, people walk past with a banana, a TV, and a microwave. `ValidationPipe` is the guard.

### The three pieces

```bash
npm install class-validator class-transformer
```

**1. `class-validator`** supplies the rule decorators:

```ts
import { IsString, IsInt, IsEmail, IsNotEmpty } from "class-validator";

export class CreateCustomerDto {
  @IsString()
  @IsNotEmpty()
  name: string;

  @IsEmail()
  email: string;

  @IsInt()
  age: number;
}
```

Everyday validators: `@IsString()`, `@IsNumber()`, `@IsInt()`, `@IsBoolean()`, `@IsEmail()`, `@IsNotEmpty()`, `@Min()/@Max()`, `@Length()`, `@IsEnum()`, `@IsUUID()`, `@IsDateString()`.

**2. `class-transformer`** converts the incoming plain JSON object into an actual `CreateCustomerDto` instance — necessary because the validators read metadata attached to the class, and a plain object carries none.

**3. `ValidationPipe`** runs the whole thing before the controller:

```ts
// main.ts
app.useGlobalPipes(new ValidationPipe());
```

A **pipe** is data middleware — it intercepts request data before the handler executes:

```
Client → ValidationPipe → valid? → yes → Controller → Service
                                  → no  → 400, controller never runs
```

Registering globally beats decorating every endpoint with `@Body(new ValidationPipe())`.

### Invalid input

```json
{ "name": "Roshan", "age": "hello" }
```

```json
{ "statusCode": 400, "message": ["age must be an integer number"] }
```

Note `message` is an **array** — one entry per failed rule, which is what lets a frontend highlight several fields at once.

### `whitelist` and `forbidNonWhitelisted`

```ts
app.useGlobalPipes(
  new ValidationPipe({
    whitelist: true,
    forbidNonWhitelisted: true,
  }),
);
```

Given `{ "name": "Roshan", "age": 30, "salary": 100000 }`:

| Config                         | Behaviour                                                |
| ------------------------------ | -------------------------------------------------------- |
| neither                        | `salary` reaches your controller untouched               |
| `whitelist: true`              | `salary` is silently **stripped**                        |
| `+ forbidNonWhitelisted: true` | request **rejected**: `property salary should not exist` |

**Analogy.** The passport form accepts name, DOB, and address. `whitelist` quietly discards the "Instagram password" you wrote in the margin; `forbidNonWhitelisted` hands the form back and refuses to process it.

This closes bug #5 from Video 10 — a client can no longer smuggle `{"id": 999}` into a PATCH body and rewrite the primary key.

> **⚠️ Gotcha — `whitelist` strips fields that have no validation decorator.**
> "Whitelisted" means _"has at least one class-validator decorator,"_ not _"declared in the DTO."_ So:
>
> ```ts
> export class CreateCustomerDto {
>   @IsString() name: string;
>   age: number; // ← no decorator
> }
> ```
>
> With `whitelist: true`, `age` is **silently removed from every request**. You add a field, forget the decorator, and the value vanishes with no error anywhere. When a field mysteriously arrives as `undefined`, this is the first thing to check.

> **⚠️ Beyond the video — `transform: true` is the option you'll miss most.**
>
> ```ts
> new ValidationPipe({
>   whitelist: true,
>   forbidNonWhitelisted: true,
>   transform: true,
> });
> ```
>
> Without it, the object handed to your controller is a **plain object**, not a DTO instance — so DTO methods and defaults don't exist, and route/query params stay strings. With it, plus `class-transformer`'s `@Type`:
>
> ```ts
> export class FindCustomersDto {
>   @Type(() => Number)
>   @IsInt()
>   page: number; // "2" from the query string arrives as 2
> }
> ```
>
> This is the general solution to the string-conversion problem that `ParseIntPipe` solves one parameter at a time (Video 5).

> **⚠️ Beyond the video — nested objects and arrays are not validated by default.**
> A nested DTO is silently skipped unless you mark it explicitly:
>
> ```ts
> export class CreateOrderDto {
>   @ValidateNested({ each: true })
>   @Type(() => OrderItemDto) // required — without it, nothing is checked
>   items: OrderItemDto[];
> }
> ```
>
> For arrays of primitives use the `each` option: `@IsString({ each: true }) tags: string[];`
> This is a common source of "validation passed but the data is garbage."

> **⚠️ Beyond the video — optional fields and update DTOs.**
> `@IsOptional()` skips the remaining validators when a field is absent — essential for PATCH. Combined with `PartialType` from Video 11:
>
> ```ts
> export class UpdateCustomerDto extends PartialType(CreateCustomerDto) {}
> ```
>
> every field becomes optional while keeping its rules.

> **⚠️ Beyond the video — a global pipe created with `new` cannot inject anything.**
> `app.useGlobalPipes(new ValidationPipe())` sits outside the DI container. If a custom pipe ever needs a service, register it as a provider instead:
>
> ```ts
> { provide: APP_PIPE, useClass: ValidationPipe }
> ```
>
> Same applies to `APP_GUARD`, `APP_INTERCEPTOR`, and `APP_FILTER` — which is exactly how the global `ThrottlerGuard` gets registered in Video 49.

### Production baseline

```ts
app.useGlobalPipes(
  new ValidationPipe({
    whitelist: true,
    forbidNonWhitelisted: true,
    transform: true,
  }),
);
```

Set this up once, on day one of a project.

### For your Spring background

`class-validator` is Bean Validation (`@NotNull`, `@Email`, `@Size`), and `ValidationPipe` plays the role of `@Valid` on a controller parameter. `whitelist`/`forbidNonWhitelisted` have no Bean Validation equivalent — the closest is Jackson's `FAIL_ON_UNKNOWN_PROPERTIES`, and unlike Jackson this is on a per-DTO basis and off by default.

### Interview questions from this lecture

**Q. Why don't DTOs validate on their own?** TypeScript types don't survive compilation; runtime validation needs decorators plus a pipe.
**Q. What is `class-validator`?** A decorator library defining validation rules on class properties.
**Q. Why is `class-transformer` needed?** Validators operate on class instances; it converts the incoming plain object into one.
**Q. What does `ValidationPipe` do?** Validates (and optionally transforms) request data before the handler runs, throwing 400 on failure.
**Q. `whitelist` vs `forbidNonWhitelisted`?** Strip unknown properties vs reject the request containing them.
**Q. What does `transform: true` do?** Returns a real DTO instance and applies type conversions such as string → number.

### Mental model after Video 12

```
Client → DTO + ValidationPipe → Controller → Service
```

The first genuine security checkpoint in the application. Video 13 shows how to write custom pipes when the built-in validators aren't enough.

---

## Video 13 — Custom Pipes

**▶ https://www.youtube.com/watch?v=KUj0XcnD85U**

`ValidationPipe` (Video 12) is one built-in pipe. This lecture shows the general mechanism and how to write your own.

### What a pipe is

> A class implementing `PipeTransform` that runs on request data **before** the handler executes.

**Analogy — airport security.** Passengers pass through a checkpoint that can verify identity, reject people, and remove prohibited items before anyone reaches the terminal.

Pipes do exactly two things:

- **Transform** — `"123"` → `123`, `"roshan"` → `"ROSHAN"`, `"  x  "` → `"x"`
- **Validate** — reject `{ "age": -10 }` before it can do damage

### Built-in pipes

`ParseIntPipe`, `ParseFloatPipe`, `ParseBoolPipe`, `ParseUUIDPipe`, `ParseEnumPipe`, `ParseArrayPipe`, `DefaultValuePipe`, `ValidationPipe`.

```ts
@Get(':id')
findOne(@Param('id', ParseIntPipe) id: number) {}
```

`/users/10` → `10` (a real number). `/users/abc` → `400 Validation failed`, handler never runs.

`DefaultValuePipe` is worth knowing — it supplies a fallback before other pipes see the value:

```ts
@Query('page', new DefaultValuePipe(1), ParseIntPipe) page: number
```

### Writing one

```bash
nest g pipe common/pipes/uppercase
```

```ts
@Injectable()
export class UppercasePipe implements PipeTransform {
  transform(value: string) {
    return value.toUpperCase();
  }
}
```

`PipeTransform` is an interface that obliges the class to implement `transform()`. **Whatever `transform()` returns becomes the value the handler receives** — the controller never sees the original.

```ts
@Post()
create(@Body('name', UppercasePipe) name: string) {
  return name;      // "roshan" → "ROSHAN"
}
```

Conventional home for reusable cross-cutting classes:

```
src/common/
├── pipes/
├── guards/
├── interceptors/
└── filters/
```

### Custom validation pipes

```ts
@Injectable()
export class AgeValidationPipe implements PipeTransform {
  transform(value: number) {
    if (value < 18) throw new BadRequestException("Age must be at least 18");
    return value;
  }
}
```

Throwing inside a pipe aborts the request — the controller is skipped and Nest converts the exception into an HTTP response.

### Where pipes can be applied

| Scope      | Syntax                        | Applies to                      |
| ---------- | ----------------------------- | ------------------------------- |
| Parameter  | `@Param('id', ParseIntPipe)`  | one parameter                   |
| Method     | `@UsePipes(ValidationPipe)`   | every parameter of that handler |
| Controller | `@UsePipes(...)` on the class | every handler in it             |
| Global     | `app.useGlobalPipes(...)`     | every request                   |

Passing the **class** (`ParseIntPipe`) lets Nest instantiate it through DI; passing an **instance** (`new ParseIntPipe({...})`) lets you configure it but bypasses DI. For a global pipe that needs injected dependencies, use the `APP_PIPE` provider (Video 12).

---

### ⚠️ Three problems with the video's examples

**1. `transform()` takes a second argument the lecture never mentions — and you need it.**

```ts
transform(value: any, metadata: ArgumentMetadata) {
  // metadata = { type: 'body' | 'query' | 'param' | 'custom', metatype, data }
}
```

`metadata.type` tells you _where_ the value came from and `metadata.data` gives the key name. Without checking it, a pipe behaves differently depending on how it's attached — which is exactly what goes wrong next.

**2. The `TrimPipe` as written crashes when applied to a whole body.**

```ts
transform(value: string) { return value.trim(); }
```

Attached to a single field (`@Body('name', TrimPipe)`) it's fine. Attached to the whole body (`@UsePipes(TrimPipe)` or `@Body(TrimPipe)`), `value` is an **object**, `value.trim` is `undefined`, and you get a `TypeError` — a 500, not a 400. Guard it:

```ts
transform(value: any, { type }: ArgumentMetadata) {
  if (typeof value === 'string') return value.trim();
  if (type === 'body' && value && typeof value === 'object') {
    return Object.fromEntries(
      Object.entries(value).map(([k, v]) => [k, typeof v === 'string' ? v.trim() : v]),
    );
  }
  return value;
}
```

**3. The closing "professional example" doesn't work as shown.**
It chains `TrimPipe → UppercasePipe → ValidationPipe` over a body and claims the output is `{ name: "ROSHAN", email: "roshan@gmail.com" }` — name uppercased _and_ email lowercased. A single pipe chain can't apply different rules to different fields; it sees one value. You'd need `@Body('name', TrimPipe, UppercasePipe)` and `@Body('email', TrimPipe, LowercasePipe)` as separate parameters, which is clumsy.

> **⚠️ Better approach — do per-field normalisation in the DTO, not in pipes.**
> `class-transformer`'s `@Transform()` runs per property, so each field gets its own rule and the whole thing stays in one place:
>
> ```ts
> export class CreateUserDto {
>   @Transform(({ value }) => value?.trim())
>   @IsString()
>   name: string;
>
>   @Transform(({ value }) => value?.trim().toLowerCase())
>   @IsEmail()
>   email: string;
> }
> ```
>
> (Requires `transform: true` on the `ValidationPipe` — Video 12.) Reserve custom pipes for **parameter-level** concerns: parsing a path param, validating a single scalar, applying a domain rule like a PAN or GST format check.

---

### Execution order — the interview question

The lecture contrasts middleware and pipes but doesn't give the full sequence. Worth memorising, because it's asked constantly and the intuitive guess is wrong:

```
Request
  → Middleware
  → Guards                (authentication / authorisation)
  → Interceptors (before)
  → Pipes                 (validation / transformation)
  → Route handler
  → Interceptors (after)
  → Exception filters     (on any thrown error)
Response
```

**Guards run before pipes.** So an unauthenticated request is rejected _before_ its body is ever validated — which is the right order, and also why the `ThrottlerGuard` in Video 49 can reject floods without paying validation cost.

Middleware vs pipes, precisely: middleware runs before routing is resolved and works on the raw `req`/`res` (logging, correlation IDs, `trust proxy`); pipes run after the handler is known and operate on individual, already-parsed arguments.

### Interview questions from this lecture

**Q. What is a pipe?** A class implementing `PipeTransform` that validates or transforms request data before the handler runs.
**Q. What are the two responsibilities?** Transformation and validation.
**Q. What does `transform()` return?** The value the handler receives.
**Q. Where can pipes be applied?** Parameter, method, controller, or globally.
**Q. Middleware vs pipes?** Middleware: pre-routing, raw request/response. Pipes: post-routing, per-argument.
**Q. Do guards or pipes run first?** Guards.

---

## Video 14 — Guards: Protecting Routes

**▶ https://www.youtube.com/watch?v=iJeJGVk9ZX8**

Everything built so far is wide open — anyone can call any endpoint. Guards are the access-control layer.

### Authentication vs Authorization

|                    | Question           | Example                            |
| ------------------ | ------------------ | ---------------------------------- |
| **Authentication** | _Who are you?_     | Verifying an email/password login  |
| **Authorization**  | _What may you do?_ | Only admins can `DELETE /users/10` |

**Analogy.** Authentication is showing ID at the building entrance. Authorization is whether that ID opens the CEO's office.

### What a guard is

> A class that decides whether a request may reach the route handler.

**Analogy — a cinema.** The usher checks your ticket. Valid → you enter. Invalid → you don't. The screening itself never knows you existed.

Guards sit at a specific point in the lifecycle (the full order was covered in Video 13):

```
Client → Middleware → Guard → Pipe → Controller → Service
```

Guards run **before pipes**, so unauthenticated requests are rejected before you spend anything on validation.

### `CanActivate` and `canActivate()`

```ts
@Injectable()
export class AuthGuard implements CanActivate {
  canActivate(context: ExecutionContext): boolean {
    return true; // true → proceed, false → blocked
  }
}
```

```bash
nest g guard guards/auth
```

> **⚠️ The video only shows the synchronous form.** Real guards do async work — verifying a JWT, loading a user, checking a permission table. The signature allows it:
>
> ```ts
> canActivate(ctx: ExecutionContext): boolean | Promise<boolean> | Observable<boolean>
> ```
>
> Just `async canActivate(...)` and `await` inside. Without knowing this you end up returning a `Promise` object, which is truthy, so **every request passes regardless of the result** — a silent auth bypass.

### `ExecutionContext`

Gives access to the current request:

```ts
const request = context.switchToHttp().getRequest();
request.headers;
request.body;
request.params;
```

The `switchToHttp()` indirection exists because Nest guards also run over WebSockets, gRPC/microservices, and GraphQL — the context is transport-agnostic, and you pick the transport you're in.

### The video's token guard

```ts
canActivate(context: ExecutionContext): boolean {
  const request = context.switchToHttp().getRequest();
  const token = request.headers.authorization;
  return token === 'secret123';
}
```

```ts
@UseGuards(AuthGuard)
@Get()
getProducts() { return []; }
```

Or protect an entire controller:

```ts
@UseGuards(AuthGuard)
@Controller("products")
export class ProductController {}
```

---

### ⚠️ Two things to fix before reusing this pattern

**1. Returning `false` gives `403`, but a missing or bad credential should be `401`.**

The video states — correctly — that a `false` return produces `403 Forbidden`. But the semantics are wrong for this case:

| Code                 | Meaning                                                               |
| -------------------- | --------------------------------------------------------------------- |
| **401 Unauthorized** | I don't know who you are — credentials missing, malformed, or expired |
| **403 Forbidden**    | I know exactly who you are, and you still may not do this             |

A wrong token is a 401. Clients rely on this distinction: 401 typically triggers a token refresh or redirect to login, while 403 shows "access denied." Throw explicitly rather than returning `false`:

```ts
canActivate(context: ExecutionContext): boolean {
  const request = context.switchToHttp().getRequest();
  const token = request.headers.authorization;
  if (token !== 'secret123') {
    throw new UnauthorizedException('Invalid or missing token');
  }
  return true;
}
```

Guards may throw any HTTP exception; Nest turns it into the right response. Use `403`/`ForbiddenException` in the **roles** guard of Video 15, where identity is known but permission is lacking.

**2. The guard authenticates but attaches nothing, so the handler still doesn't know who called.**

The lecture lists "extract user, attach user to request" under a future JWT example, but that step is what makes a guard useful:

```ts
const payload = this.jwtService.verify(token);
request.user = payload; // ← now downstream code can use it
return true;
```

```ts
@Get('profile')
getProfile(@Req() req) { return req.user; }
```

Cleaner still, a custom parameter decorator:

```ts
export const CurrentUser = createParamDecorator(
  (_data, ctx: ExecutionContext) => ctx.switchToHttp().getRequest().user,
);

@Get('profile')
getProfile(@CurrentUser() user) { return user; }
```

This is exactly what Passport's `JwtStrategy` does for you automatically in Video 44 — worth understanding manually first.

---

### Guard scopes — including the one the video omits

| Scope              | How                                                       |
| ------------------ | --------------------------------------------------------- |
| Method             | `@UseGuards(AuthGuard)` on a handler                      |
| Controller         | `@UseGuards(AuthGuard)` on the class                      |
| **Global**         | `app.useGlobalGuards(new AuthGuard())`                    |
| **Global with DI** | `{ provide: APP_GUARD, useClass: AuthGuard }` in a module |

The `APP_GUARD` form is the one you'll actually use, because a guard created with `new` can't inject `JwtService` or `ConfigService`. It's also precisely how the global `ThrottlerGuard` is registered in Video 49.

> **⚠️ A global auth guard needs an escape hatch.** Once every route is protected, `/login` and `/health` are locked out too. The standard pattern is a `@Public()` marker read by `Reflector`:
>
> ```ts
> export const Public = () => SetMetadata("isPublic", true);
>
> // inside the guard
> const isPublic = this.reflector.getAllAndOverride("isPublic", [
>   context.getHandler(),
>   context.getClass(),
> ]);
> if (isPublic) return true;
> ```
>
> `Reflector` reads metadata attached by custom decorators — the same mechanism Video 15 uses for roles.

### Why not put this in the controller

```ts
@Get()
getUsers(@Req() req) {
  if (req.headers.authorization !== 'secret123') throw new Error();
  return [];
}
```

Repeated in every handler, easy to forget in one, and impossible to audit. A guard centralises it — and forgetting `@UseGuards` on a route is at least visible in one place.

### Guard vs pipe vs middleware

|            | Runs                            | Answers                                  |
| ---------- | ------------------------------- | ---------------------------------------- |
| Middleware | before routing, raw `req`/`res` | logging, CORS, correlation IDs           |
| **Guard**  | after routing, before pipes     | _may this request proceed?_              |
| Pipe       | after guards, per argument      | _is this data valid / what shape is it?_ |

### For your Spring background

Guards are the Spring Security filter chain plus `@PreAuthorize`, expressed as injectable classes. `request.user` is the analogue of `SecurityContextHolder`, except Nest makes you attach it yourself (or lets Passport do it in Video 44).

### Interview questions from this lecture

**Q. What is a guard?** A class deciding whether a request may reach its handler.
**Q. Which interface and method?** `CanActivate` / `canActivate()`.
**Q. What if it returns `false`?** Nest blocks the request with `403 Forbidden` — though for authentication failures you should throw `UnauthorizedException` (401) instead.
**Q. What is `ExecutionContext`?** A transport-agnostic handle on the current execution, giving access to the request via `switchToHttp()`.
**Q. Authentication vs authorization?** Identity vs permission.
**Q. Guard vs pipe?** Whether the request proceeds vs what shape its data takes.
**Q. Can `canActivate` be async?** Yes — it may return `boolean`, `Promise<boolean>`, or `Observable<boolean>`.

---

## Video 15 — Role-Based Authorization (RBAC)

**▶ https://www.youtube.com/watch?v=MjbElEDIYnQ**

Video 14 answered _may this request enter?_ This one answers _what may this user do once inside?_ Authentication vs authorization was covered there; here it becomes code.

The target syntax:

```ts
@Roles(Role.Admin)
@Get()
getUsers() {}
```

Four pieces make it work: an **enum**, a **custom decorator**, **metadata**, and a **guard** that reads it via `Reflector`.

### Step 1 — Roles enum

```ts
export enum Role {
  User = "user",
  Admin = "admin",
}
```

Bare strings invite `'admin'` / `'Admin'` / `'ADMIN'` mismatches that fail silently — a typo becomes a permission bug, not a compile error. `Role.Admin` is checkable.

### Step 2 — the `@Roles()` decorator

```ts
export const Roles = (...roles: Role[]) => SetMetadata("roles", roles);
```

**Metadata is data about data.** A book's content is the data; author and category are metadata. Here the handler is the data, and "requires admin" is metadata attached to it.

**Analogy — a sticky note on the route.** `@Roles(Role.Admin)` doesn't _do_ anything by itself; it leaves a note that something else reads later.

This is the same `SetMetadata` mechanism as the `@Public()` decorator sketched in Video 14.

### Step 3 — `RolesGuard` and `Reflector`

`Reflector` is the metadata reader — it's how a guard discovers what the route asked for:

```ts
@Injectable()
export class RolesGuard implements CanActivate {
  constructor(private reflector: Reflector) {}

  canActivate(context: ExecutionContext): boolean {
    const requiredRoles = this.reflector.get<Role[]>(
      "roles",
      context.getHandler(),
    );
    const request = context.switchToHttp().getRequest();
    const userRole = request.headers["x-user-role"];
    return requiredRoles.includes(userRole);
  }
}
```

```ts
@UseGuards(RolesGuard)
@Roles(Role.Admin)
@Get()
getUsers() {}
```

Multiple roles work as an OR — `@Roles(Role.Admin, Role.Manager)` admits either.

---

### ⚠️ Three problems, one of which crashes the app

**1. A route without `@Roles()` throws a 500.**

If the guard is applied to a controller where some handlers have no `@Roles()`, `requiredRoles` is `undefined`, and `undefined.includes(...)` is a `TypeError` — a 500, from your security layer. Always short-circuit:

```ts
const requiredRoles = this.reflector.getAllAndOverride<Role[]>(ROLES_KEY, [
  context.getHandler(),
  context.getClass(),
]);
if (!requiredRoles) return true; // no role requirement → open route
```

**2. `reflector.get(..., context.getHandler())` ignores controller-level `@Roles()`.**

`getHandler()` inspects only the method. Put `@Roles(Role.Admin)` on the controller class expecting to protect every route in it, and the guard sees nothing — every route is then open (or crashes, per problem 1). Use `getAllAndOverride`, which checks the handler first and falls back to the class:

```ts
this.reflector.getAllAndOverride<Role[]>(ROLES_KEY, [
  context.getHandler(),
  context.getClass(),
]);
```

Also export the key rather than repeating a magic string in two files:

```ts
export const ROLES_KEY = "roles";
export const Roles = (...roles: Role[]) => SetMetadata(ROLES_KEY, roles);
```

A typo'd string in the guard reads as `undefined` — which, once you add the fix above, silently makes protected routes **public**.

**3. `x-user-role` isn't a simplification — it's a complete auth bypass.**

The video is upfront that this stands in until JWT arrives, and as a teaching device that's fine. But be blunt about what the code does: **any client can send `x-user-role: admin`.** There is no verification whatsoever. This is worse than having no authorization, because it looks like protection in a code review.

The only trustworthy source of a role is a **signed** token verified server-side:

```ts
// AuthGuard (Video 44) verifies the JWT and attaches the payload
request.user = { id: 1, role: "admin" };

// RolesGuard then reads from there, never from a header
const { user } = context.switchToHttp().getRequest();
return requiredRoles.includes(user.role);
```

Never move the header version past a tutorial branch.

---

### Guard ordering

```ts
@UseGuards(AuthGuard, RolesGuard)
```

Guards execute **in the order listed**, and this order is mandatory: `RolesGuard` reads `request.user`, which only exists because `AuthGuard` put it there. Reverse them and `user` is `undefined`.

```
Client → JWT Auth Guard (who?) → Roles Guard (allowed?) → Pipes → Controller
```

Registered globally via `APP_GUARD` (Video 14), execution follows provider registration order.

### 401 vs 403 — the distinction pays off here

This is where the Video 14 correction lands. In `RolesGuard` the user **is** authenticated; they simply lack permission. That is genuinely `403 Forbidden`:

```ts
throw new ForbiddenException("Insufficient role");
```

Missing/invalid token → `401` (AuthGuard). Valid token, wrong role → `403` (RolesGuard).

### Where RBAC runs out

Roles answer "can admins delete products?" They can't answer **"can this user edit _this_ post?"** — ownership and attribute-based rules need the resource in hand, not just the role:

```ts
if (post.authorId !== user.id && user.role !== Role.Admin) {
  throw new ForbiddenException();
}
```

For anything richer, Nest integrates with CASL for attribute-based access control. Worth knowing the ceiling before you build a 20-role enum trying to encode ownership.

### For your Spring background

This is `@PreAuthorize("hasRole('ADMIN')")` — except Spring ships the plumbing and Nest has you assemble it from `SetMetadata` + `Reflector` + a guard. More code, but the mechanism is fully visible, and the same three pieces power feature flags, `@Public()`, caching hints, and anything else metadata-driven.

### Interview questions from this lecture

**Q. What is RBAC?** Authorization where permissions attach to roles rather than individuals.
**Q. Why an enum for roles?** Type safety and one canonical spelling.
**Q. What does `SetMetadata` do?** Attaches custom metadata to a handler or controller.
**Q. What is `Reflector`?** The utility guards use to read that metadata.
**Q. AuthGuard vs RolesGuard?** Identity vs permission — 401 vs 403.
**Q. Which runs first?** AuthGuard, because the role check needs `request.user`.
**Q. Why read roles from the token rather than a header?** A header is client-controlled; a signed JWT is verified server-side.

---

## Video 16 — Exception Filters & Custom Error Handling

**▶ https://www.youtube.com/watch?v=OgQPOMsPn4A**

Guards and pipes decide what gets rejected; exception filters decide **what a rejection looks like**.

### The problem

Left alone, different endpoints return different error shapes — `{"message":"Not Found"}` here, `{"error":"Order Missing"}` there, `{"status":404}` somewhere else. Frontend developers then write bespoke parsing per endpoint.

**Analogy — a hospital complaint desk.** Rather than every department inventing its own complaint process, there's one desk with one form. Exception filters are that desk.

### Built-in exceptions

`BadRequestException` (400), `UnauthorizedException` (401), `ForbiddenException` (403), `NotFoundException` (404), `ConflictException` (409), `UnprocessableEntityException` (422), `InternalServerErrorException` (500) — all extend `HttpException`.

```ts
throw new NotFoundException("User not found");
// → { "statusCode": 404, "message": "User not found", "error": "Not Found" }
```

Nest already has a built-in global filter producing this. A custom filter is for when you need a **house format**:

```json
{
  "success": false,
  "statusCode": 404,
  "message": "User not found",
  "timestamp": "2026-06-21T10:00:00Z",
  "path": "/users/10"
}
```

### Writing one

```bash
nest g filter common/filters/http-exception
```

```ts
@Catch(HttpException)
export class HttpExceptionFilter implements ExceptionFilter {
  catch(exception: HttpException, host: ArgumentsHost) {
    const ctx = host.switchToHttp();
    const response = ctx.getResponse();
    const request = ctx.getRequest();
    const status = exception.getStatus();

    response.status(status).json({
      statusCode: status,
      timestamp: new Date().toISOString(),
      path: request.url,
      message: exception.message,
    });
  }
}
```

`@Catch(X)` declares which exception types this filter handles. `catch()` is the mandatory method, mirroring `canActivate()` for guards and `transform()` for pipes.

**`ArgumentsHost` vs `ExecutionContext`** — the video calls them "very similar"; precisely, **`ExecutionContext extends ArgumentsHost`** and adds `getHandler()` and `getClass()`. That's exactly why guards can read route metadata with `Reflector` (Video 15) and a plain filter can't.

### Scopes

| Scope          | How                                                      |
| -------------- | -------------------------------------------------------- |
| Method         | `@UseFilters(HttpExceptionFilter)` on a handler          |
| Controller     | `@UseFilters(...)` on the class                          |
| Global         | `app.useGlobalFilters(new HttpExceptionFilter())`        |
| Global with DI | `{ provide: APP_FILTER, useClass: HttpExceptionFilter }` |

Method-level filters take precedence over controller-level, which take precedence over global. As with pipes (Video 12) and guards (Video 14), a filter built with `new` sits outside DI — so if you want to inject a `LoggerService`, use `APP_FILTER`.

---

### ⚠️ Three problems worth fixing

**1. A bare `@Catch()` catches everything — including errors with no `getStatus()`.**

The scaffold generates `@Catch()` with no argument, which catches _all_ exceptions, not just HTTP ones. A `TypeError`, a Mongoose failure, or a dropped DB connection is a plain `Error` with no `getStatus()` method — so `exception.getStatus()` throws **inside your filter**, and Nest falls back to a bare 500 with your formatting lost. Handle both:

```ts
@Catch()
export class AllExceptionsFilter implements ExceptionFilter {
  catch(exception: unknown, host: ArgumentsHost) {
    const ctx = host.switchToHttp();
    const status = exception instanceof HttpException
      ? exception.getStatus()
      : HttpStatus.INTERNAL_SERVER_ERROR;
    ...
  }
}
```

Either keep `@Catch(HttpException)` narrow and add a separate catch-all, or write one filter that handles both branches.

**2. `exception.message` destroys validation error detail.**

This is the one that will actually break your frontend. `ValidationPipe` (Video 12) produces a **per-field array**, but it lives in the response object, not in `.message`:

```ts
exception.message; // → "Bad Request Exception"   ← useless
exception.getResponse(); // → { statusCode: 400, message: ["email must be an email", ...] }
```

Use `getResponse()` so field-level errors survive:

```ts
const res = exception.getResponse();
const message = typeof res === "string" ? res : (res as any).message;
```

Follow the video verbatim and every validation failure collapses to the string "Bad Request Exception" — your form can no longer highlight which field was wrong.

**3. Don't echo internal errors to clients, and don't swallow them.**

`message: exception.message` on a 500 can leak connection strings, SQL fragments, or file paths. Log the real error server-side, return something generic:

```ts
const isServerError = status >= 500;
this.logger.error(
  exception instanceof Error ? exception.stack : String(exception),
);

response.status(status).json({
  success: false,
  statusCode: status,
  timestamp: new Date().toISOString(),
  path: request.url,
  message: isServerError ? "Internal server error" : message,
});
```

A global filter is also the last place an unhandled error passes through — if you don't log here, production failures vanish silently.

---

> **⚠️ Platform note.** `response.status(...).json(...)` is the **Express** API. On Fastify (`@nestjs/platform-fastify`, Video 1) it's `.status(...).send(...)`. Filters written this way are one of the few places Nest's platform-agnosticism leaks.

### Where filters sit

```
Middleware → Guards → Interceptors → Pipes → Controller → Service
                                        ↓ (any throw, at any stage)
                                 Exception Filter → formatted response
```

Filters catch exceptions from **every** layer — a guard's `ForbiddenException` (Video 15) and a pipe's validation failure (Video 12) both land here, not just controller errors.

|            | Purpose                          | When           |
| ---------- | -------------------------------- | -------------- |
| Guard      | may the request proceed?         | before handler |
| Pipe       | validate / transform data        | before handler |
| **Filter** | how should an error be returned? | after a throw  |

### Restaurant analogy, updated

Module = the building · Controller = waiter · Service = chef · Guard = security · Pipe = quality checker · **Exception Filter = the complaint desk**.

### For your Spring background

This is `@ControllerAdvice` + `@ExceptionHandler`, with `@Catch(SomeException)` playing the role of `@ExceptionHandler(SomeException.class)`. The precedence rules (most specific / most local wins) work the same way.

### Interview questions from this lecture

**Q. What is an exception filter?** A class that intercepts thrown exceptions and controls the HTTP response.
**Q. Interface and method?** `ExceptionFilter` / `catch()`.
**Q. What does `@Catch()` do?** Declares which exception types the filter handles; empty means all.
**Q. `ArgumentsHost` vs `ExecutionContext`?** `ExecutionContext` extends it, adding `getHandler()`/`getClass()` for metadata access.
**Q. Can filters be global?** Yes — `useGlobalFilters()`, or `APP_FILTER` when DI is needed.
**Q. How do you preserve validation error details?** Read `exception.getResponse()`, not `exception.message`.

---

## Video 17 — Middleware

**▶ https://www.youtube.com/watch?v=5JhFvdPwkKA**

The last piece of the request lifecycle, and the earliest one to run. The full ordering was already established in Videos 13–16, so this section focuses on middleware's own mechanics and the boundary against guards.

### What it is

> A function that runs **before Nest resolves which handler should serve the request**.

**Analogy — the reception desk.** Before you reach the receptionist, manager, or meeting room, you pass the front desk: sign in, get a visitor badge, have your arrival logged.

That "before routing is resolved" detail is the whole story — it's why middleware is good at route-independent work and bad at anything needing to know _which_ handler was matched.

### Typical uses

Logging, request IDs / correlation IDs, analytics, response headers, IP blocking, `trust proxy` setup, raw-body capture for webhook signature checks.

### Writing one

```bash
nest g middleware common/logger
```

```ts
@Injectable()
export class LoggerMiddleware implements NestMiddleware {
  use(req: Request, res: Response, next: NextFunction) {
    console.log(req.method, req.url);
    next();
  }
}
```

`NestMiddleware` obliges `use()`, the same way `CanActivate` obliges `canActivate()` and `ExceptionFilter` obliges `catch()`.

**`next()` is mandatory.** Omit it and the request hangs — no error, no response, the browser just spins until it times out. Every code path in `use()` must either call `next()` or send a response.

### Registering it

Unlike guards and filters, middleware isn't attached with a decorator — it's configured in the module:

```ts
export class AppModule implements NestModule {
  configure(consumer: MiddlewareConsumer) {
    consumer.apply(LoggerMiddleware).forRoutes("users");
  }
}
```

More options than the video shows:

```ts
consumer.apply(LoggerMiddleware).forRoutes("users", "products"); // several paths
consumer.apply(LoggerMiddleware).forRoutes(UsersController); // a controller class
consumer
  .apply(LoggerMiddleware)
  .exclude("health", "metrics") // opt-out paths
  .forRoutes("*");
consumer.apply(logger).forRoutes({ path: "users", method: RequestMethod.GET });
```

**Functional middleware** is fine when you need no dependencies — a plain `(req, res, next) => {...}` function passed to `apply()`. Use the class form when you need DI.

> **⚠️ Version gotcha — `forRoutes('*')`.** The bare `'*'` wildcard changed with Express 5 / path-to-regexp v8, which recent Nest majors adopted. If you hit a `path-to-regexp` parse error, that's the cause — check the current wildcard syntax in the docs rather than assuming, since this shifted after my knowledge cutoff. For genuinely application-wide middleware, `app.use(logger)` in `main.ts` sidesteps the question entirely.

---

### ⚠️ Two things to get right

**1. Don't use middleware for authentication — and the reason is structural, not stylistic.**

The video shows an auth middleware and then advises preferring guards. The concrete reasons:

- **Middleware has no `ExecutionContext`.** It can't call `context.getHandler()`, so it can't use `Reflector` to read `@Roles()` or `@Public()` metadata (Videos 14–15). Route-aware authorization is impossible.
- **Error handling is less predictable.** A synchronous `throw` in class middleware generally reaches Nest's exception layer, but an **async** middleware that rejects will not — you must catch and call `next(err)`, or you get an unhandled rejection instead of a clean 401.

```ts
async use(req, res, next) {
  try {
    req.user = await this.jwt.verifyAsync(token);
    next();
  } catch (err) {
    next(new UnauthorizedException());   // ← not a bare throw
  }
}
```

Guards run inside Nest's execution context with DI, metadata, and filters all working normally. Use middleware for cross-cutting request processing; use guards for access control.

**2. `console.log(req.method, req.url)` can't log what the lecture says it logs.**

It lists method, URL, IP, **and request duration** as what real systems record — but duration and status code aren't known until the response finishes. Hook the response instead, and use Nest's built-in `Logger` rather than `console.log` so output respects log levels and formatting:

```ts
@Injectable()
export class LoggerMiddleware implements NestMiddleware {
  private readonly logger = new Logger("HTTP");

  use(req: Request, res: Response, next: NextFunction) {
    const start = Date.now();
    res.on("finish", () => {
      this.logger.log(
        `${req.method} ${req.originalUrl} ${res.statusCode} ${Date.now() - start}ms`,
      );
    });
    next();
  }
}
```

---

### The complete lifecycle

```
Client
 → Middleware            request preprocessing, no route context yet
 → Guards                may this proceed?          (401 / 403)
 → Interceptors (before) wrap the call
 → Pipes                 validate & transform       (400)
 → Controller → Service
 → Interceptors (after)  transform the response
 → Exception Filters     on any throw, from any stage
Response
```

| Layer      | Question                 | Knows the route?              |
| ---------- | ------------------------ | ----------------------------- |
| Middleware | preprocess this request? | ❌                            |
| Guard      | may it proceed?          | ✅ (metadata via `Reflector`) |
| Pipe       | is the data valid?       | ✅ (per argument)             |
| Filter     | how to render the error? | partially                     |

_(Interceptors are the one layer not yet covered in this course — they wrap the handler and can transform responses, add caching, or set timeouts.)_

### Restaurant analogy, complete

Module = restaurant · **Middleware = reception desk** · Guard = security · Pipe = quality checker · Controller = waiter · Service = chef · Filter = complaint desk.

### For your Spring background

Middleware is a **Servlet `Filter`** — it sits outside the handler-mapping layer and sees the raw request/response. Guards are closer to `HandlerInterceptor.preHandle()` or the Spring Security filter chain, which _do_ know the resolved handler. The same rule of thumb applies in both frameworks: authentication belongs where handler metadata is available.

### Interview questions from this lecture

**Q. What is middleware?** A function running before the route handler is resolved.
**Q. Interface and method?** `NestMiddleware` / `use()`.
**Q. What if `next()` isn't called?** The request hangs indefinitely.
**Q. How is it registered?** Via `configure(consumer)` in a module implementing `NestModule` — not with a decorator.
**Q. Middleware vs guards?** Preprocessing vs access control; middleware runs first but has no route metadata.
**Q. Why prefer guards for auth?** They have `ExecutionContext`, so they can read `@Roles()`/`@Public()` metadata, and their exceptions integrate cleanly with filters.

---

## Video 18 — Lifecycle Hooks

**▶ https://www.youtube.com/watch?v=NpS7qpim3IQ**

Everything so far happens _per request_. Lifecycle hooks run **once**, at application startup and shutdown — connecting to Redis, warming a cache, closing connections cleanly.

> Methods Nest calls automatically at defined phases. You never invoke them yourself; implementing the interface is enough.

**Analogy — opening and closing a shopping mall.** Every morning: unlock doors, start the AC and escalators, switch on lights. Every night: lights off, escalators stopped, doors locked, reports generated. Nobody re-remembers the checklist daily; it's a fixed procedure.

### The complete hook set

> **⚠️ Correction — `afterModuleInit()` does not exist.**
> The video mentions it "theoretically." There's no such hook in NestJS. The actual set is five, and the video also omits `beforeApplicationShutdown`:

| Hook                                 | Interface                   | When                                          |
| ------------------------------------ | --------------------------- | --------------------------------------------- |
| `onModuleInit()`                     | `OnModuleInit`              | that module's dependencies are resolved       |
| `onApplicationBootstrap()`           | `OnApplicationBootstrap`    | **all** modules initialised, before listening |
| `onModuleDestroy()`                  | `OnModuleDestroy`           | shutdown signal received                      |
| `beforeApplicationShutdown(signal?)` | `BeforeApplicationShutdown` | after all `onModuleDestroy` complete          |
| `onApplicationShutdown(signal?)`     | `OnApplicationShutdown`     | connections closing, last chance to clean up  |

Documented order:

```
startup:   onModuleInit → onApplicationBootstrap
shutdown:  onModuleDestroy → beforeApplicationShutdown → onApplicationShutdown
```

Note the shutdown sequence differs slightly from the video's `onModuleDestroy → onApplicationShutdown` — `beforeApplicationShutdown` sits between them and receives the OS signal (`SIGTERM`, `SIGINT`).

### Usage

```ts
@Injectable()
export class UserService implements OnModuleInit, OnApplicationShutdown {
  onModuleInit() {
    console.log("User module initialised");
  }

  onApplicationShutdown(signal: string) {
    console.log(`Shutting down: ${signal}`);
  }
}
```

Nest detects the implemented interface and calls the method. `service.onModuleInit()` by hand is always wrong.

### `onModuleInit` vs `onApplicationBootstrap`

|                          | Fires when                                        |
| ------------------------ | ------------------------------------------------- |
| `onModuleInit`           | _this_ module is ready — other modules may not be |
| `onApplicationBootstrap` | _every_ module is ready                           |

So anything touching another module's provider belongs in `onApplicationBootstrap`. Within a module, hooks respect dependency order: a provider's hook runs after the hooks of everything it injects.

---

### ⚠️ The critical omission: shutdown hooks don't run by default

Everything the video says about `onModuleDestroy` and `onApplicationShutdown` is **inert** unless you opt in:

```ts
// main.ts
const app = await NestFactory.create(AppModule);
app.enableShutdownHooks(); // ← without this, none of the shutdown hooks fire
await app.listen(process.env.PORT ?? 3000);
```

It's off by default because it attaches listeners to process signals, which carries a small cost. Miss this line and you'll write careful cleanup code, deploy it, and never see it execute — with no error to tell you why.

This matters directly for Video 50: Railway, Render, and Kubernetes all stop a container by sending **`SIGTERM`**. With shutdown hooks enabled you can drain in-flight requests and close pools cleanly; without them the process is killed mid-flight, leaving connections dangling and messages unacknowledged.

### ⚠️ Hooks can be async — and usually should be

The video shows only synchronous examples. Every hook may return a `Promise`, and Nest **awaits** it before proceeding:

```ts
async onModuleInit() {
  await this.redis.connect();
}

async onApplicationShutdown() {
  await this.redis.quit();
}
```

Without `async`/`await`, startup continues before the connection is ready and shutdown completes before cleanup finishes — the exact failures hooks exist to prevent.

### ⚠️ You rarely need these for your main database

The video's headline example is "connect to the database in `onModuleInit`." In practice `TypeOrmModule.forRoot()` (Video 36) and `MongooseModule.forRoot()` (Video 22) manage their own connection lifecycle, including disconnect. Reserve lifecycle hooks for things Nest doesn't wrap for you:

- a hand-rolled Redis / Kafka / RabbitMQ client
- warming an in-memory cache or loading reference data
- registering with a service discovery system, and deregistering on shutdown
- flushing metrics or log buffers before exit

---

### Hooks vs middleware

|                 | Runs                      |
| --------------- | ------------------------- |
| Middleware      | on every request          |
| Lifecycle hooks | once, at startup/shutdown |

### For your Spring background

Direct analogues: `onModuleInit` ≈ `@PostConstruct` / `InitializingBean`, `onApplicationBootstrap` ≈ `ApplicationReadyEvent`, `onModuleDestroy`/`onApplicationShutdown` ≈ `@PreDestroy` / `DisposableBean`. And `enableShutdownHooks()` is roughly Spring Boot's `server.shutdown=graceful` — an explicit opt-in in both frameworks.

### Restaurant analogy, complete

Module = restaurant · Middleware = reception · Guard = security · Pipe = quality checker · Controller = waiter · Service = chef · Filter = complaint desk · **Lifecycle hooks = opening and closing procedures**.

### Interview questions from this lecture

**Q. What are lifecycle hooks?** Methods Nest calls automatically at defined application phases.
**Q. Name them in order.** `onModuleInit` → `onApplicationBootstrap`, then `onModuleDestroy` → `beforeApplicationShutdown` → `onApplicationShutdown`.
**Q. `onModuleInit` vs `onApplicationBootstrap`?** One module ready vs all modules ready.
**Q. Do you call them yourself?** No — implement the interface and Nest invokes them.
**Q. Why might shutdown hooks not fire?** `app.enableShutdownHooks()` wasn't called.
**Q. Can they be async?** Yes, and Nest awaits the returned promise.

---

## Video 19 — Lifecycle Hooks in Practice

**▶ https://www.youtube.com/watch?v=xp4jDjWG_tE**

The hands-on companion to Video 18 — a `DatabaseService` that simulates connecting on startup and disconnecting on shutdown. Kept short here since the concepts are covered above; this section notes only what the demo adds.

### The pattern

```ts
@Injectable()
export class DatabaseService implements OnModuleInit, OnApplicationShutdown {
  private isConnected = false;

  onModuleInit() {
    this.isConnected = true;
    console.log("Database Connected");
  }

  onApplicationShutdown(signal: string) {
    this.isConnected = false;
    console.log(`Database Disconnected (${signal})`);
  }

  status() {
    return { connected: this.isConnected };
  }
}
```

Real implementations swap the flag for `await this.prisma.$connect()` / `await mongoose.connect(...)` — which requires `async onModuleInit()`, per Video 18.

**A useful property:** if `onModuleInit` throws or rejects, Nest **aborts the bootstrap** and the app never starts listening. So the lecture's claim is right — you get fail-fast startup rather than an app that accepts traffic with a dead database and errors on the first query.

### `enableShutdownHooks()`

```ts
app.enableShutdownHooks();
```

This is the fix flagged in the Video 18 notes above — worth recording that **the course does teach it**, just one lecture later than the concept. If your shutdown hooks appear dead, this line is the reason.

### The `signal` parameter

`onApplicationShutdown(signal)` receives the OS signal that triggered shutdown.

> **⚠️ Correction — `SIGKILL` cannot be caught.**
> The video lists `SIGINT`, `SIGTERM`, and `SIGKILL` together as examples. `SIGKILL` (and `SIGSTOP`) are the two signals a process **cannot** trap, by design — the kernel terminates it immediately. No hook of any kind will ever run for a `SIGKILL`. That's exactly why `kill -9` is the last resort, and why cleanup must never be assumed to happen.

> **⚠️ In production the signal you care about is `SIGTERM`, not `SIGINT`.**
> `SIGINT` is Ctrl+C in your terminal. Docker, Kubernetes, and Railway (Video 50) all stop containers by sending **`SIGTERM`**, then waiting a grace period (30s by default on Kubernetes) before escalating to `SIGKILL`. Two practical consequences:
>
> - Your cleanup must finish **well inside** that window, or it's cut off mid-way.
> - Graceful shutdown means: stop accepting new requests, let in-flight ones finish, _then_ close pools.

### On the status endpoint

```ts
@Get()
getStatus() { return this.databaseService.status(); }
```

Fine as a demo. As a real health check it has a flaw: returning `{ "connected": false }` with a **200 OK** tells a load balancer the instance is healthy. Health checks are read by status code — an unhealthy instance must return **503** so the orchestrator stops routing traffic to it. In real projects use `@nestjs/terminus`, which provides health indicators for databases, memory, and disk with correct status codes.

### Interview questions from this lecture

**Q. Purpose of `onModuleInit`?** Initialisation logic once a provider's dependencies are ready.
**Q. Purpose of `onApplicationShutdown`?** Cleanup before the process exits.
**Q. Why might it not fire?** `app.enableShutdownHooks()` wasn't called.
**Q. Which signal does Ctrl+C send?** `SIGINT`. Container orchestrators send `SIGTERM`.
**Q. Can you handle `SIGKILL`?** No — it cannot be trapped.
**Q. What happens if `onModuleInit` throws?** Bootstrap aborts; the application doesn't start.

---

## Video 20 — Environment Variables & ConfigModule

**▶ https://www.youtube.com/watch?v=gMCUp31uYgY**

The last of the fundamentals, and the first genuinely professional practice: configuration lives outside the code.

### Why

**Security.** `const JWT_SECRET = "secret123"` in source means the secret is in Git history forever — and rotating it requires a code change and redeploy. Anyone with repo access can forge tokens (the point made in Video 44).

**Environment portability.** Dev, staging, and production need different database URLs. Without externalised config you edit code to deploy, which is how wrong credentials reach production.

**Analogy — appliances and electricity.** Your TV needs power but doesn't contain a generator; it plugs into a supply provided externally. Same code, different socket, different environment.

### `.env` at the project root

```env
PORT=3000
DB_URL=mongodb://localhost:27017/ecommerce
JWT_SECRET=mysecret
```

**Never commit it.** Add to `.gitignore`:

```gitignore
.env
```

> **⚠️ Do commit a `.env.example`** — the same keys with dummy or blank values. Without it, a new teammate clones the repo and has no idea which variables the app needs; they discover them one crash at a time. This is standard practice and the video omits it.
>
> ```env
> PORT=3000
> DB_URL=
> JWT_SECRET=
> ```

### ConfigModule and ConfigService

```bash
npm install @nestjs/config
```

```ts
@Module({
  imports: [ConfigModule.forRoot({ isGlobal: true })],
})
export class AppModule {}
```

`isGlobal: true` saves importing `ConfigModule` into every feature module. This is the `@Global()` mechanism from Video 6 — and config is the textbook case where the encapsulation trade-off is worth it.

```ts
@Injectable()
export class DatabaseService {
  constructor(private configService: ConfigService) {}

  getDbUrl() {
    return this.configService.get("DB_URL");
  }
}
```

Ordinary constructor injection — the same DI from Video 5.

```
.env → ConfigModule (at startup) → ConfigService → injected into your providers
```

---

### ⚠️ Three gaps that cause real bugs

**1. `.get()` returns `undefined` for a missing or misspelled key — silently.**

```ts
this.configService.get("JWT_SECRET"); // typo'd key → undefined, no warning
```

`undefined` as a JWT signing secret is a security incident, not a typo. Two better options:

```ts
this.configService.getOrThrow<string>("JWT_SECRET"); // fails loudly at read time
this.configService.get<string>("PORT", "3000"); // explicit default
```

**2. Validate the whole config at startup rather than discovering gaps at runtime.**

```ts
ConfigModule.forRoot({
  isGlobal: true,
  validationSchema: Joi.object({
    NODE_ENV: Joi.string()
      .valid("development", "production", "test")
      .default("development"),
    PORT: Joi.number().default(3000),
    DB_URL: Joi.string().required(),
    JWT_SECRET: Joi.string().min(32).required(),
  }),
});
```

Now a missing `DB_URL` **prevents the application from starting** with a clear message, instead of surfacing as a confusing failure on the first request an hour after deploy. Same fail-fast principle as `onModuleInit` throwing in Video 19 — and this is the piece that separates "I know about `.env`" from "I've configured a production service."

**3. Everything from `.env` is a string.**

```env
PORT=3000
DEBUG=false
```

```ts
this.configService.get("PORT"); // "3000"  ← string
this.configService.get("DEBUG"); // "false" ← string, and truthy!
```

`if (config.get('DEBUG'))` is **always true**, because `"false"` is a non-empty string. Either cast explicitly, or let the Joi schema coerce types (`Joi.number()` yields a real number).

---

### Loading order and production

`@nestjs/config` reads **real process environment variables first**, falling back to `.env`. That's precisely why the same code works locally and on Railway (Video 50), where variables are injected by the platform and no `.env` file exists. In production you can set `ignoreEnvFile: true` to make that explicit.

Other options worth knowing: `envFilePath` (point at `.env.development`, `.env.test`, or several files with precedence), and `load` for custom config factories with typed namespaces.

> **⚠️ Honest limit.** A `.env` file is plaintext on disk and visible to anything running as that user. It solves "don't commit secrets to Git," not "protect secrets at rest." Serious deployments use a secret manager (AWS Secrets Manager, Vault, or the platform's own encrypted variable store) and rotate credentials on a schedule.

### How this connects forward

Config plus lifecycle hooks (Videos 18–19) is the standard startup pattern:

```ts
async onModuleInit() {
  await connect(this.configService.get('DB_URL'));
}
```

And the reason `JwtModule.registerAsync()` exists (Video 44) is exactly this ordering problem — the JWT module can't be configured until `ConfigService` has loaded, so its setup is deferred until its injected dependencies are ready.

### For your Spring background

`ConfigModule` ≈ `application.yml` + `@ConfigurationProperties`; `configService.get()` ≈ `@Value("${db.url}")`; the Joi schema ≈ `@Validated` on a config properties class; `NODE_ENV` ≈ Spring profiles. Nest doesn't have a profile system as such — you point `envFilePath` at a different file, or rely on the platform's injected variables.

### Interview questions from this lecture

**Q. Why use environment variables?** Keeps secrets out of source control and lets one build run in many environments.
**Q. What is `ConfigModule`?** The module that loads `.env` and process env into the application at startup.
**Q. What is `ConfigService`?** The injectable used to read those values.
**Q. Why `isGlobal: true`?** Avoids importing `ConfigModule` in every module.
**Q. Should `.env` be committed?** No — commit `.env.example` instead.
**Q. How do you guarantee a required variable exists?** A `validationSchema` at startup, or `getOrThrow()` at read time.
**Q. What type do env values have?** Always strings, unless cast or coerced.

---

# Part 6 — Authentication & Security

## Video 44 — JWT Authentication with MongoDB

**▶ https://www.youtube.com/watch?v=qry1F5ibO4U**

### What changes from Video 43

In Video 43, Supabase handled everything — it stored users, checked passwords, and issued the JWT; Nest only verified the token. Here Nest does the whole job itself: register users, store them in MongoDB, hash passwords, verify passwords, sign JWTs, validate them, and protect routes. No external auth provider.

Why bother? Full control over login logic, signup rules, custom roles, and anything an enterprise app needs that a hosted auth provider won't bend to.

### Packages

| Package            | Purpose                                                                   |
| ------------------ | ------------------------------------------------------------------------- |
| `@nestjs/jwt`      | Sign and verify tokens — `jwtService.sign()`, `jwtService.verify()`       |
| `passport`         | General authentication framework (the "authentication manager")           |
| `passport-jwt`     | The strategy that teaches Passport how to read and validate Bearer tokens |
| `@nestjs/passport` | Nest wrapper around Passport (which is an Express-era library)            |
| `bcrypt`           | Password hashing                                                          |

### Never store plaintext passwords

If your `users` collection looks like this and the database leaks, every user's password is public — and because people reuse passwords, you've also compromised their email and banking accounts:

```
john@gmail.com    123456
alice@gmail.com   password
bob@gmail.com     qwerty
```

Store hashes instead: `$2b$10$ASDKJH...`. Even a DBA with full read access can't recover the original.

### Hashing vs encryption

```
Encryption:  original → encrypt → ciphertext → decrypt → original    (reversible)
Hashing:     password → hash function → fixed-length string          (one-way)
```

There is no "unhash" operation. That's exactly why passwords are hashed and not encrypted — you never need to read a password back, only to check whether a submitted one matches.

### Salt rounds

```ts
bcrypt.hash(password, 10);
```

The `10` is the **cost factor** (salt rounds). Two things happen:

1. bcrypt generates a random **salt** per password, so two users with the same password get different hashes:
   ```
   User A: "123456" → $2b$10$XYZ123...
   User B: "123456" → $2b$10$ABK782...
   ```
   Without a salt, identical hashes would leak the fact that both users chose the same password — and rainbow tables would crack both at once.
2. The cost factor makes hashing deliberately slow (each +1 doubles the work), so brute-forcing the hash is expensive.

> **⚠️ Beyond the video.** 10 rounds is the common default and is reasonable; 12 is the more current recommendation for new systems. Note that the salt is stored _inside_ the resulting hash string — you don't need a separate column for it. Also, `bcrypt` silently truncates input beyond 72 bytes, which matters if you allow long passphrases.

### User schema

Only `email` and the **hashed** password:

```json
{ "email": "john@gmail.com", "password": "$2b$10$ASKDJH..." }
```

### Auth module

Same modular pattern as every other feature (see Video 1) — an `AuthModule` containing the auth controller, auth service, JWT configuration, and the strategy, so authentication logic stays isolated.

```ts
JwtModule.registerAsync({
  imports: [ConfigModule],
  inject: [ConfigService],
  useFactory: (config: ConfigService) => ({
    secret: config.get("JWT_SECRET"),
  }),
});
```

**Why `registerAsync` and not `register`?** The secret comes from `.env` (Video 20), and `ConfigService` must be initialised _before_ the JWT module can read from it. `registerAsync` defers the module's configuration until its injected dependencies are ready.

**Never hardcode the secret.** `secret: "abcdef123"` committed to GitHub means anyone can forge a valid token for any user, including admins. Put it in `.env`, keep `.env` out of git.

### Signup flow

```
Client → POST /signup → Controller → AuthService → bcrypt.hash() → MongoDB → success
```

The controller does almost nothing but forward the body to the service — the same thin-controller pattern as every CRUD lecture.

### Login flow

```
POST /login
  ↓
find user by email  ──not found──→ 401 Unauthorized
  ↓
bcrypt.compare()    ──no match──→ 401 Unauthorized
  ↓
sign JWT → return { access_token }
```

**Why `bcrypt.compare()` and not `===`?** Comparing `"123456"` against `"$2b$10$AKDJH..."` is meaningless. `compare()` extracts the salt and cost from the stored hash, re-hashes the submitted password with those same parameters, and compares the results.

> **⚠️ Beyond the video — two production details.**
>
> 1. Return the **same** error message whether the email doesn't exist or the password is wrong. "User not found" vs "Wrong password" tells an attacker which emails are registered (user enumeration).
> 2. Never put the password hash — or anything sensitive — in the JWT payload. The payload is only **base64-encoded, not encrypted**; anyone holding the token can read it. The signature prevents _tampering_, not _reading_.

### Inside a JWT

```
header . payload . signature
xxxxx  . yyyyy   . zzzzz
```

- **Header** — algorithm and token type
- **Payload** — user id, email, role, expiry
- **Signature** — computed from header + payload + secret; this is what makes tampering detectable

### JWT Strategy

Earlier (Video 43) you verified the token by hand inside a Guard. Passport now does it automatically:

```
Request → AuthGuard('jwt') → JwtStrategy → extract Bearer token
        → verify signature → decode payload → attach to request.user → Controller
```

A **strategy** tells Passport _how_ to authenticate. Think of Passport as a building's security desk that can check identity several ways — JWT, Google, Facebook, GitHub, Local (username/password), OAuth. Here we register the JWT strategy.

Its four automatic jobs: extract the token from `Authorization: Bearer ...`, verify the signature against `JWT_SECRET`, decode the payload, and attach the result to `request.user` so no controller ever decodes a token again.

### Protecting routes

Guards were introduced in Video 14; Passport ships one for JWT:

```ts
@Get('profile')
@UseGuards(AuthGuard('jwt'))
getProfile() {}
```

Without a valid token, the request is rejected before the controller runs.

### Postman testing

| Request        | Body / Header                           | Response                           |
| -------------- | --------------------------------------- | ---------------------------------- |
| `POST /signup` | `{ "email": "...", "password": "..." }` | user created                       |
| `POST /login`  | same                                    | `{ "access_token": "eyJhbGc..." }` |
| `GET /profile` | _(no header)_                           | `401 Unauthorized`                 |
| `GET /profile` | `Authorization: Bearer eyJhbGc...`      | `{ "id": 1, "email": "..." }`      |

### Supabase auth (43) vs custom auth (44)

|                  | Video 43 (Supabase) | Video 44 (NestJS + MongoDB)                |
| ---------------- | ------------------- | ------------------------------------------ |
| User storage     | Supabase            | MongoDB                                    |
| Password check   | Supabase            | NestJS + bcrypt                            |
| JWT generation   | Supabase            | `JwtService.sign()`                        |
| JWT verification | Nest Guard (manual) | Passport JWT Strategy                      |
| Registration     | Supabase Auth       | custom `/signup`                           |
| Login            | Supabase Auth API   | custom `/login`                            |
| Best for         | shipping fast       | full control, production-grade custom auth |

### Key takeaways

- Always hash with bcrypt; never store plaintext.
- The JWT is issued only after a **successful login**, never at signup.
- Passport is the framework; `passport-jwt` is the strategy.
- `JwtStrategy` extracts, verifies, and attaches the user automatically.
- `@UseGuards(AuthGuard('jwt'))` protects any route.

> **⚠️ Beyond the video — what a production system adds.** Token expiry (`signOptions: { expiresIn: '15m' }`) plus a refresh-token flow; rate limiting on `/login` and `/signup` (Video 49); and stripping the password field from every user object you return.

---

## Video 49 — Rate Limiting using Throttler

**▶ https://www.youtube.com/watch?v=VjkX4Fm3YFM**

### The problem authentication doesn't solve

Even with JWT auth in place, nothing stops a client from sending 10,000 requests per second:

```js
while (true) {
  POST / login;
}
```

Your server burns CPU on junk traffic, real users see timeouts, and the database falls over. **Rate limiting** caps how many requests a client can make in a time window.

**Analogy.** A restaurant where one customer orders 100 pizzas per second overwhelms the kitchen and everyone else waits. So the restaurant caps it: three orders per minute, then "please wait."

### Where it sits in the pipeline

```
Client → Rate Limiter → JWT Guard → Role Guard → Validation Pipe → Controller → Service → Database
```

Rate limiting runs **before** the controller — and before JWT verification. If the limit is already blown, Nest returns `429` immediately without even validating the token, which is exactly why it saves resources.

### The two settings

- **TTL (Time To Live)** — the length of the counting window. After it elapses, the counter resets to zero.
- **Limit** — the maximum requests allowed inside that window.

With `TTL = 60s, Limit = 3`:

```
10:00:01  request 1  ✓
10:00:05  request 2  ✓
10:00:20  request 3  ✓
10:00:30  request 4  ✗ 429 Too Many Requests
10:01:01  counter resets → request 1 ✓
```

### How clients are identified

By default Nest tracks counts **per IP address** — each IP gets its own counter:

```
{ "192.168.1.1": 2, "192.168.1.2": 1, "192.168.1.3": 3 }
```

> **⚠️ Beyond the video — two things that bite in production.**
>
> 1. **Behind a proxy or load balancer**, every request appears to come from the proxy's IP, so all your users share one bucket. You must enable `app.set('trust proxy', 1)` (Express) so the real client IP is read from `X-Forwarded-For`. This absolutely applies on Railway (Video 50).
> 2. **The default storage is in-memory**, so counters are per-process. Run two instances and a limit of 3 effectively becomes 6. Real deployments use `@nest-lab/throttler-storage-redis` so all instances share one counter.

### Setup

```bash
npm install @nestjs/throttler
```

Registered in `AppModule`, with `ThrottlerGuard` in the providers to apply it globally.

> **⚠️ Correction — the video's config shape is outdated.**
> The tutorial shows a flat object, which was the v4 API. From **v5 onward** `forRoot()` takes an **array** of named throttler configs, and **`ttl` is in milliseconds**, not seconds:
>
> ```ts
> ThrottlerModule.forRoot([
>   { name: "short", ttl: 60_000, limit: 3 }, // 60 seconds
> ]);
> ```
>
> Passing `ttl: 60` on a modern version gives you a 60-_millisecond_ window — the limit will appear not to work at all. Check the version in your `package.json` against the current docs.

### Global vs route-level

Registered globally, every route shares one rule. But different endpoints need different rules:

| Endpoint                | Sensible limit | Why                                 |
| ----------------------- | -------------- | ----------------------------------- |
| `POST /login`           | 5 / minute     | stops brute-force password guessing |
| `POST /forgot-password` | 3 / hour       | stops email spam                    |
| `POST /send-otp`        | 2 / minute     | stops SMS-cost abuse                |
| `GET /search`           | 100 / minute   | normal use fine, bots throttled     |
| `POST /payment`         | 1 / 10 seconds | prevents accidental double charges  |
| `GET /health`           | unlimited      | monitoring must never be blocked    |

Use the `@Throttle()` decorator on the controller or handler to override the global rule.

### Brute force, concretely

Without limits, an attacker walks the dictionary: `password1`, `password2`, … `password100000`, and eventually gets in. Capped at 5 attempts per minute, the same attack takes years.

### Testing

With `limit = 3`, hitting `GET /employees` in Postman gives `200, 200, 200, 429`.

**Status code recap:** `200` OK · `401` Unauthorized · `404` Not Found · **`429` Too Many Requests** — you've exceeded the allowed rate.

### How it connects back

| Earlier video             | Link                                                                 |
| ------------------------- | -------------------------------------------------------------------- |
| 14 — Guards               | `ThrottlerGuard` is just another Guard running before the controller |
| 17 — Middleware vs Guards | Rate limiting is a Guard, not middleware                             |
| 42–44 — JWT auth          | Apply the strictest limits to `/login` and `/signup`                 |

### The security stack so far

```
Client Request
      ↓
Rate Limiter (Throttler)     ← spam & brute-force
      ↓
JWT Authentication Guard     ← who are you?
      ↓
Roles / Authorization Guard  ← what may you do?
      ↓
Validation Pipe (DTO)        ← is this payload well-formed?
      ↓
Controller → Service → Database
```

Layered like this, even a user with a perfectly valid JWT can't flood your API — the throttler stops them before any business logic runs.

---

# Part 7 — Deployment

## Video 50 — Deploying a NestJS App on Railway

**▶ https://www.youtube.com/watch?v=V5ocs-gHzo4**

_Final video of the series._

### What deployment is

In development your app runs at `http://localhost:3000` — and `localhost` always means _the machine you're sitting at_. Send that URL to a friend and it resolves to **their** computer, not yours. To make the API reachable by anyone, it has to run on a machine that's always on and publicly addressable. That's deployment.

```
localhost:3000  →  https://employee-api-production.up.railway.app
```

Options include Railway, Render, AWS, Azure, GCP, DigitalOcean, and Heroku. This lecture uses **Railway** because it needs almost no configuration.

### What Railway does for you

Railway rents you a computer on the internet and automates: cloning the repo, installing packages, building the project, starting the app, issuing a public URL, and redeploying on every push.

### Prerequisites

1. A **GitHub account** — Railway deploys from a repository, not from your laptop.
2. A working NestJS project.

### Steps

```bash
nest new employee-api
cd employee-api

git init
git add .
git commit -m "Initial Commit"

git remote add origin <repo-url>
git push -u origin main
```

Then in Railway: log in with GitHub → **Import Repository** → pick the repo. The deployment flow is:

```
Laptop → GitHub → Railway
```

### What Railway runs internally

```
git clone            → fetch your code
npm install          → read package.json, install dependencies
npm run build        → TypeScript compiled to JavaScript in dist/
npm run start:prod   → run the compiled app
```

Identical to what you'd type locally — just automated.

### CI/CD

- **CI (Continuous Integration)** — on every push, the code is fetched, dependencies installed, project built, tests run.
- **CD (Continuous Deployment)** — a successful build is deployed automatically.

```
Developer → git push → GitHub → Railway → Deploy → Live API updated
```

No manual file uploads, ever.

### Getting a public URL

**Settings → Networking → Generate Domain** produces e.g. `https://employee-api.up.railway.app`. Now `localhost:3000/employees` becomes `https://employee-api.up.railway.app/employees`.

> **⚠️ Beyond the video — the #1 reason a Railway deploy shows nothing.**
> Railway assigns a port via the `PORT` environment variable and expects your app to bind to it. If `main.ts` hardcodes `3000`, the build succeeds, the logs look healthy, and the URL returns an error. Fix it once:
>
> ```ts
> await app.listen(process.env.PORT ?? 3000);
> ```
>
> (Same point raised in Video 2.)

### Updating

```bash
git add .
git commit -m "add products endpoint"
git push
```

Railway sees the new commit and rebuilds and redeploys on its own.

### Environment variables in production

`.env` (Video 20) holds secrets — `DATABASE_URL`, `JWT_SECRET`, `SUPABASE_KEY` — and must **never** be committed. In production you enter the same keys into Railway's **Variables** dashboard instead. Your code doesn't change at all:

```ts
configService.get("DATABASE_URL");
```

Only the _source_ of the values differs — `.env` locally, the platform's injected environment in production.

### Local vs deployed

| Local                       | Railway                |
| --------------------------- | ---------------------- |
| Runs on your computer       | Runs on a cloud server |
| Only you can reach it       | Anyone can reach it    |
| `localhost`                 | Public domain          |
| Dies when the laptop sleeps | Runs continuously      |
| Manual testing              | Production environment |

### Analogy

Your app is a restaurant. Cooking at home = developing locally; only your family eats. Opening in a busy city = deploying; anyone can walk in. **GitHub is the recipe book, Railway is the building and kitchen**, and every `git push` is an updated recipe that Railway immediately starts cooking and serving.

### Key takeaways

- Deployment = hosting the app on an always-on server with a public address.
- Railway is a PaaS that automates build, deploy, and hosting.
- GitHub is the source of truth; Railway deploys from it.
- CI/CD means every push can ship automatically.
- Secrets live in the platform's variable store, never in the repo.
- Bind to `process.env.PORT`.

> **⚠️ Beyond the video.** Free tiers change constantly — check Railway's current pricing rather than trusting a 2025 tutorial. And this is _deployment_, not _operations_: production also needs logging, health checks, monitoring, and database backups. The instructor points to their DevOps series (Jenkins + Docker + AWS EC2) for the heavier CI/CD path.

### The full journey

```
NestJS Basics → Modules → Controllers → Services → Dependency Injection
→ DTOs → Validation → Pipes → Guards → Middleware → Exception Filters
→ Lifecycle Hooks → Environment Variables → MongoDB (Mongoose) → CRUD
→ Relationships → PostgreSQL → TypeORM → Search & Filtering
→ JWT Authentication → Authorization → Rate Limiting → Deployment
```
