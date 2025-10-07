# Project Tech Stack

This project leverages a modern full-stack architecture designed to balance developer productivity with long-term scalability and maintainability.

## Frontend

- **Vue 3** – Provides a progressive, component-driven JavaScript framework for building efficient and reactive user interfaces.
- **Quasar Framework** – Supplies a rich UI component library, responsive design system, and first-class PWA tooling, enabling seamless deployment across web, mobile, and desktop platforms.
- **Pinia** – Handles global application state with a clean, modular API that plays nicely with TypeScript.
- **TypeScript** – Adds type safety and improved maintainability, making the frontend more predictable and easier to debug.

## Backend

- **Laravel** – Serves as the primary PHP framework for building RESTful APIs, offering a clean architecture with built-in authentication, validation, and caching features.
- **Laravel Reverb** – Powers the system's real-time WebSocket communication, enabling instant, bidirectional updates across connected clients.
- **PostgreSQL** – Acts as the relational database engine, delivering reliable structured data storage with strong performance and data integrity guarantees.
- **Redis** – Provides a high-performance in-memory data store used for caching (leveraging cache tagging for granular invalidation), job queues, and other low-latency operations.

## Integration

- The frontend communicates with the Laravel backend through secure RESTful API endpoints and WebSocket channels managed by Laravel Reverb.
- Data persistence and querying are managed via Laravel's Eloquent ORM, which interacts with PostgreSQL as the primary data store.
- Laravel's caching layer relies on Redis cache tagging to keep frequently accessed data synchronized without broad cache flushes.

Together, this stack promotes modularity, scalability, and efficiency, maintaining a clear separation between client and server responsibilities while ensuring a smooth developer experience.
