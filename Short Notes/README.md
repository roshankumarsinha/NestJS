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
| 8   | Dependency Injection in NestJS                    | [▶](https://www.youtube.com/watch?v=Fgikn8N_mus) | ⬜  |
| 9   | REST API & HTTP Methods + Postman                 | [▶](https://www.youtube.com/watch?v=Uyk6bwm2eWI) | ⬜  |
| 10  | Create REST APIs (GET/POST/PUT/PATCH/DELETE)      | [▶](https://www.youtube.com/watch?v=w9JYelWOSj4) | ⬜  |
| 11  | DTOs & Interfaces Explained                       | [▶](https://www.youtube.com/watch?v=E3TbXT2TR5Q) | ⬜  |
| 12  | Validating DTOs with class-validator              | [▶](https://www.youtube.com/watch?v=IIKZVHy1Dqw) | ⬜  |
| 13  | Custom Pipes                                      | [▶](https://www.youtube.com/watch?v=KUj0XcnD85U) | ⬜  |
| 14  | Protecting Routes using Guards                    | [▶](https://www.youtube.com/watch?v=iJeJGVk9ZX8) | ⬜  |
| 15  | Role-Based Authorization in Guards                | [▶](https://www.youtube.com/watch?v=MjbElEDIYnQ) | ⬜  |
| 16  | Exception Filters & Custom Error Handling         | [▶](https://www.youtube.com/watch?v=OgQPOMsPn4A) | ⬜  |
| 17  | Middleware in NestJS                              | [▶](https://www.youtube.com/watch?v=5JhFvdPwkKA) | ⬜  |
| 18  | Lifecycle Events / Hooks                          | [▶](https://www.youtube.com/watch?v=NpS7qpim3IQ) | ⬜  |
| 19  | Lifecycle Hooks: onModuleInit & onAppShutdown     | [▶](https://www.youtube.com/watch?v=xp4jDjWG_tE) | ⬜  |
| 20  | Environment Variables & .env                      | [▶](https://www.youtube.com/watch?v=gMCUp31uYgY) | ⬜  |
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
