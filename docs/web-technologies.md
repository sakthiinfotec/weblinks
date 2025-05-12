#### [Functional Programming](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
Functional programming (often abbreviated FP) is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions. Contrast with object oriented programming, where application state is usually shared and colocated with methods in objects.

- Pure functions
- Function composition
- Avoid shared state
- Avoid mutating state
- Avoid side effects

Functional code tends to be more concise, more predictable, and easier to test than imperative or object oriented code — but if you’re unfamiliar with it and the common patterns associated with it, functional code can also seem a lot more dense, and the related literature can be impenetrable to newcomers.

**Side Effects**  
A side effect is any application state change that is observable outside the called function other than its return value. Side effects include:

- Modifying any external variable or object property (e.g., a global variable, or a variable in the parent function scope chain)
- Logging to the console
- Writing to the screen
- Writing to a file
- Writing to the network
- Triggering any external process
- Calling any other functions with side-effects

**Reusability Through Higher Order Functions**  
Functional programming tends to reuse a common set of functional utilities to process data. Object oriented programming tends to colocate methods and data in objects. Those colocated methods can only operate on the type of data they were designed to operate on, and often only the data contained in that specific object instance.

JavaScript has first class functions, which allows us to treat functions as data — assign them to variables, pass them to other functions, return them from functions, etc…

A higher order function is any function which takes a function as an argument, returns a function, or both. Higher order functions are often used to:
- Abstract or isolate actions, effects, or async flow control using callback functions, promises, monads, etc…
- Create utilities which can act on a wide variety of data types
- Partially apply a function to its arguments or create a curried function for the purpose of reuse or function composition
- Take a list of functions and return some composition of those input functions

**Declarative vs Imperative**  
Functional programming is a declarative paradigm, meaning that the program logic is expressed without explicitly describing the flow control.

**Imperative** programs spend lines of code describing the specific steps used to achieve the desired results — the flow control: How to do things.

**Declarative** programs abstract the flow control process, and instead spend lines of code describing the data flow: What to do. The how gets abstracted away.

For example, this **imperative mapping** takes an array of numbers and returns a new array with each number multiplied by 2:
```javascript
const doubleMap = numbers => {
  const doubled = [];
  for (let i = 0; i < numbers.length; i++) {
    doubled.push(numbers[i] * 2);
  }
  return doubled;
};

console.log(doubleMap([2, 3, 4])); // [4, 6, 8]
```

This **declarative mapping** does the same thing, but abstracts the flow control away using the functional Array.prototype.map() utility, which allows you to more clearly express the flow of data:
```javascript
const doubleMap = numbers => numbers.map(n => n * 2);

console.log(doubleMap([2, 3, 4])); // [4, 6, 8]
```

**Functional programming favors:**

- Pure functions instead of shared state & side effects
- Immutability over mutable data
- Function composition over imperative flow control
- Lots of generic, reusable utilities that use higher order functions to act on many data types instead of methods that only operate on their colocated data
- Declarative rather than imperative code (what to do, rather than how to do it)
- Expressions over statements
- Containers & higher order functions over ad-hoc polymorphism

#### Authentication
Two Factor Authentication, or 2FA, is an extra layer of protection used to ensure the security of online accounts beyond just a username and password. It is the use of two separate security factors to confirm a user’s claimed identity. There are three types of factors to choose from when building a solution:

1. Something the user knows like a password or PIN
2. Something the user has such as their mobile device or a code sent to you
3. Something the user is, such as a biometric

Two-factor authentication has traditionally included the use of a password as the first security factor and the second commonly includes a text with a code sent to your smartphone, or biometrics using your fingerprint, face, or retina.

There are various ways to protect accounts via two-factor authentication: biometrics, one-time passwords, phone call, email verification codes, QR codes, hardware tokens

- Fingerprints
- Retinal patterns
- Voice recognition 
- Face recognition 
- Handwritten signatures 

Options to configure 2FA are:  
**Security key:**
Use a physical security key over USB or NFC, fingerprint reader, facial recognition, or password/PIN as a security key.

**Authenticator app:**
Use an application to get two-factor authentication codes when prompted.


**[Text-to-API app 🚀](https://x.com/Dev__Digest/status/1882423344936735216)**  
￼
How it works:
1. Describe your API in plain text
2. Generate the schema
3. Configure sources
4. /extract data with @Firecrawl_dev￼🔥
5. Store the data
6. Deploy a live endpoint

### [Why Microfrontends Are Taking Over (and Should You Care?)](https://itnext.io/why-microfrontends-are-taking-over-and-should-you-care-8f0fd3ff07ac)
#### Monolithic frontend
- A monolithic frontend means shared dependencies, global state management nightmares, and deployment bottlenecks.
- One small change can impact the entire application, forcing teams into long, painful release cycles.
- In monolithic frontend, you’re locked into a single tech stack — whether it’s React, Vue, Angular or something else.

#### Microfrontend
- Microfrontends aim to fix that by splitting the UI into independently deployable parts.
- One of the biggest drivers behind microfrontends is organizational scale.
- Multiple teams working on different features
- Microfrontends let each team own its piece of the UI, using its own tech stack, build pipeline and release schedule. This means a team working on the checkout flow doesn’t have to wait on the homepage team to finish their feature. Everyone moves faster because they’re decoupled from the rest of the application.
- Not every team wants to (or should) use the same stack.
- With microfrontends, one team might use React for an interactive dashboard, while another prefers Svelte for performance reasons.
- As long as they integrate seamlessly, each team gets the flexibility to choose the best tool for their job.

**They introduce their own set of challenges:**
- **Increased complexity:** Splitting a frontend means more infrastructure to manage.
- **Integration headaches:** Making sure everything plays nicely together requires a solid strategy
- **Duplication risks:** Without proper governance, teams might reinvent the wheel or ship redundant code

### [Why Island Architecture Might Be the Future of Web Performance](https://itnext.io/island-architecture-a-smarter-way-to-build-resilient-systems-0d9b36f6a067)
* You render most of the page statically, then hydrate only the interactive parts (the “islands”).
* only hydrate what needs interactivity, leave everything else as static HTML.
* Modern frameworks like [Astro](https://astro.build/press/#assets) embrace this philosophy.
* You write your page mostly as static HTML and only the parts that need interactivity hydrate when necessary.
* No unnecessary JavaScript, no wasted renders, no overcomplicated state management.
* JS frameworks (e.g. `React`) are hydrating a page. Island frameworks are hydrating components.

#### How to Get Started
Start by identifying which parts of your app actually need JavaScript:
- If a section never changes after the initial render, it doesn’t need hydration;
- If a page is mostly static content, pre-render it.
Frameworks like Astro, Qwik, and even Next.js (with partial hydration) make this process much easier.

If you’re working with React or Vue, try breaking your UI into independent components that only hydrate when necessary.

Keep global state MINIMAL.

Let the browser do what it does best : render static content quickly.


### [Hydration is Pure Overhead (Qwik's Resumability)](https://www.builder.io/blog/hydration-is-pure-overhead#resumability-a-no-overhead-alternative-to-hydration)
- [Qwik](https://qwik.dev/), a framework that is designed around resumabilty and achieves excellent startup performance.
- Hydration is a solution to add interactivity to server-rendered HTML. This is how Wikipedia defines hydration:
> In web development, hydration or rehydration is a technique in which client-side JavaScript converts a static HTML web page, delivered either through static hosting or server-side rendering, into a dynamic web page by attaching event handlers to the HTML elements.


#### 𝐖𝐡𝐲 𝐍𝐞𝐱𝐭.𝐣𝐬 𝐎𝐯𝐞𝐫 𝐑𝐞𝐚𝐜𝐭? 

React is great, but Next.js takes it to the next level! 

✅ 𝐒𝐄𝐎-𝐅𝐫𝐢𝐞𝐧𝐝𝐥𝐲 – Next.js supports Server-Side Rendering (SSR) and Static Site Generation (SSG), making pages load faster and rank better on Google.

✅ 𝐁𝐥𝐚𝐳𝐢𝐧𝐠 𝐅𝐚𝐬𝐭 𝐏𝐞𝐫𝐟𝐨𝐫𝐦𝐚𝐧𝐜𝐞 – Automatic image optimization, code splitting, and Edge Functions ensure your app is lightning-fast.

✅ 𝐁𝐮𝐢𝐥𝐭-𝐢𝐧 𝐀𝐏𝐈 𝐑𝐨𝐮𝐭𝐞𝐬 – No need for a separate backend! You can create serverless functions right inside your Next.js project.

✅ 𝐁𝐞𝐭𝐭𝐞𝐫 𝐃𝐞𝐯𝐞𝐥𝐨𝐩𝐞𝐫 𝐄𝐱𝐩𝐞𝐫𝐢𝐞𝐧𝐜𝐞 – File-based routing, middleware, and automatic TypeScript support make development smoother.

If SEO, speed, and scalability matter, Next.js > React!

### [The Future (and the Past) of the Web is Server Side Rendering | Staic, SPA (Client Side Rendering), SSR, Hydration, Island Architecture](https://deno.com/blog/the-future-and-past-is-server-side-rendering)
**Client-side rendering**  
In CSR, also known as dynamic rendering, the code runs primarily on the client-side, the user’s browser. The client’s browser downloads the necessary HTML, JavaScript, and other assets, and then runs the code to render the UI.
![image](https://github.com/user-attachments/assets/04a8509d-aa37-4d11-a211-2607670b20cd)

The benefits of this approach are two-fold:
**Great user experience:** If you have a wicked-fast network and can get the bundle and data downloaded quickly then, once everything is in place, you’ll have a super-speedy site. You don’t have to go back to the server for more requests, so every page change or data change happens immediately.
**Caching:** Because you aren’t using a server, you can cache the core HTML and JS bundles on a CDN. This means they can be quickly accessed by users and keeps costs low for the company.

**Server-side rendering**  
There are many benefits to moving the work a browser does to render a website to the server:

- Performance is higher with the server because the HTML is already generated and ready to be displayed when the page is loaded.
- Compatibility is higher with server-side rendering because, again, the HTML is generated on the server, so it is not dependent on the end browser.
- Complexity is lower because the server does most of the work of generating the HTML so can often be implemented with a simpler and smaller codebase.
With SSR, we do everything on the server:
![image](https://github.com/user-attachments/assets/2d2efc5e-7b9b-4301-b1ad-1f2b336c7778)

**Isomorphic JavaScript**, also known as Universal JavaScript, describes JavaScript applications which run both on the client and the server.


### How to obtain a key and cert files for a secure production application?
For a secure, real production environment, you should obtain your key and certificate (cert) from a trusted Certificate Authority (CA).

Here's why and how:

*   **Why not self-signed?** While developers can generate self-signed certificates for testing purposes, these are not trusted by browsers and operating systems. Users will see security warnings, which will damage trust in your application. Self-signed certificates do not prove your identity.

*   **Certificate Authorities (CAs):** CAs are trusted third-party organizations that verify your identity and issue digital certificates. These certificates are cryptographically signed and trusted by browsers and operating systems worldwide.

*   **How to obtain a certificate:**
    1.  **Choose a CA:** Research and select a reputable CA (e.g., Let's Encrypt, DigiCert, Sectigo, GlobalSign). Some CAs offer free certificates (like Let's Encrypt), while others charge a fee for more advanced features or higher levels of validation.
    2.  **Generate a Certificate Signing Request (CSR):** Use a tool like OpenSSL to generate a CSR. This process will also generate your private key (`server.key`). *Keep the private key secure. Do not share it.* The CSR contains information about your domain name and organization.
    3.  **Submit the CSR to the CA:** Follow the CA's instructions to submit your CSR.
    4.  **Domain Validation:** The CA will verify that you control the domain name specified in the CSR. The validation process varies depending on the CA and the type of certificate. It may involve proving control of the domain via email, DNS records, or file upload.
    5.  **Certificate Issuance:** Once the CA has validated your domain, they will issue your certificate (`server.cert` or similar).
    6.  **Install the Certificate:** Download the certificate and any intermediate certificates (if provided by the CA). Configure your server (e.g., Node.js, Apache, Nginx) to use the private key and the certificate. The 'fs.readFileSync' lines you provided will read these files into your server configuration.

*   **Developer's role:** A developer is responsible for generating the CSR, submitting it to the CA, configuring the server with the key and certificate, and renewing the certificate when it expires.

*   **Automation:** Consider using tools like Certbot (for Let's Encrypt) to automate the certificate issuance and renewal process.

In summary, developers do *not* generate the final certificates for a production environment. They generate the CSR, manage the private key, and configure the server. The *CA* issues the trusted certificate after verifying the domain.

#### Express.js

**The key to flexibility and modularity in Express: Middleware**  
A middleware allows to intercept an incoming a request and perform dedicated tasks, while the request is processed or before the response is returned.

In essence, a _middleware_ is nothing but a function taking three arguments:

`req`: The incoming request from the client
`res`: The response to be returned to the client
`next`: A function to invoke the next piece of middleware

Since middleware functions have (write-)access to the incoming request objects as well as to the outgoing response objects, they are a very powerful concept that can shape the requests and responses according to a specific purpose.Here is a simple example for logging that will print the time at which a request was received:

```javascript
function loggingMiddleware(req, res, next) {
  console.log(`Received a request at: ${Date.now()}`)
  next()
}
app.use(loggingMiddleware)
```

Middleware can be used for many use cases, such as _authentication_, _caching_, data _transformation_ and _validation_, _execution_ of custom business logic and a lot more.
