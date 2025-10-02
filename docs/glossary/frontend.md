# Glossary
## Frontend Development
Us techies love our terms and acronyms! Throughout my career, I've encountered and learned numerous technical terms that I use regularly but have never formally documented or explained. This glossary serves as both a reference document for others and an exercise for me in teaching, challenging me to explain complex concepts succinctly and clearly.

### Design and Architecture
#### Atomic Design
Atomic Design is a methodology for creating design systems by breaking down interfaces into smaller, reusable components. It consists of five stages: atoms, molecules, organisms, templates, and pages.

#### Component-Driven Architecture
Component-Driven Architecture is a design approach where applications are built using reusable, self-contained components. It promotes modularity and scalability in frontend development.

#### Responsive Design
Responsive Design ensures that web applications adapt to different screen sizes and devices. It uses techniques like fluid grids, flexible images, and media queries.

### State Management
#### Client State
Client State refers to data that exists only on the client side and is not synchronized with a server. It includes UI state, form inputs, and local component data.

#### Global State
Global State refers to data that is shared across multiple components in an application. It is often managed using state management libraries like Redux or Context API.

#### Immutability
Immutability is a principle where data structures cannot be modified after creation. It ensures predictable state updates and simplifies debugging.

#### Local State
Local State refers to data that is managed within a single component. It is typically used for temporary or component-specific data.

#### Memoization
Memoization is an optimization technique that caches the results of expensive function calls. It improves performance by avoiding redundant computations.

#### Selectors
Selectors are functions used to extract and compute derived data from a state object. They are commonly used in state management libraries like Redux.

#### Server State
Server State refers to data fetched from a server and managed in the client application. It often involves caching and synchronization with the server.

#### State Hydration
State Hydration is the process of initializing client-side state with data from the server. It is commonly used in server-side rendering (SSR) applications.

#### Store
A Store is a centralized place to manage application state. It is commonly used in state management libraries like Redux.

### Performance Optimization
#### Chunking
Chunking is the process of splitting a JavaScript bundle into smaller files (chunks). It improves performance by loading only the necessary chunks.

#### Code Splitting
Code Splitting is a technique to split an application into smaller bundles that can be loaded on demand. It improves performance and reduces initial load times.

#### Dynamic Imports
Dynamic Imports allow JavaScript modules to be loaded on demand. They are commonly used for code splitting and lazy loading.

#### Lazy Loading
Lazy Loading is a technique where resources are loaded only when they are needed. It improves performance by reducing initial load times.

#### Throttling
Throttling is a technique to limit the frequency of function execution. It is commonly used to improve performance in event-driven applications.

#### Tree Shaking
Tree Shaking is a technique used to remove unused code from a JavaScript bundle. It helps reduce the size of the final build.

### Metrics and Tools
#### Core Web Vitals
Core Web Vitals are a set of metrics that measure the performance and user experience of a website. They include metrics like Largest Contentful Paint (LCP), First Input Delay (FID), and Cumulative Layout Shift (CLS).

#### Lighthouse
Lighthouse is an open-source tool for auditing the performance, accessibility, and SEO of web applications. It provides actionable recommendations for improvement.

### Styling
#### Bootstrap
Bootstrap is a CSS framework for building responsive and mobile-first web applications. It includes pre-designed components and a grid system.

#### CSS Modules
CSS Modules are a way to scope CSS styles to specific components. They prevent style conflicts by generating unique class names.

#### CSS-in-JS
CSS-in-JS is a technique where CSS is written directly in JavaScript files. It allows for dynamic styling and better integration with JavaScript frameworks.

#### Material UI
Material UI is a popular React component library that implements Google's Material Design guidelines. It provides pre-designed components for building user interfaces.

### Frameworks and Libraries
#### Angular
Angular is a TypeScript-based framework for building web applications. It provides a complete solution for building dynamic and scalable applications.

#### D3.js
D3.js is a JavaScript library for creating data visualizations using HTML, SVG, and CSS. It provides powerful tools for manipulating data and creating interactive charts.

#### Vue
Vue is a progressive JavaScript framework for building user interfaces. It is designed to be incrementally adoptable and focuses on simplicity and flexibility.

### Component Development
#### Chromatic
Chromatic is a visual testing tool for Storybook. It automates UI testing and helps catch visual regressions.

#### Storybook
Storybook is a tool for developing and testing UI components in isolation. It provides a sandbox environment for building and documenting components.