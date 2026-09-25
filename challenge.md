# Frontend Technical Challenge (Angular)

## Introduction

Thank you for taking part in our selection process.

This challenge is designed for a **junior frontend developer**. The goal is to build a small web application using Angular that allows users to locate stores on an interactive map and explore the products available in each location.

We are interested in how you structure a solution, make technical decisions, and communicate your work. A simple, clear, and maintainable solution is preferred over unnecessary complexity.

You are free to use any resources available to you, including:

- Official documentation
- Online tutorials and technical references
- Artificial Intelligence tools
- Third-party libraries
- Development tools of your choice

Using these resources is welcome. Be prepared to explain the important decisions in your solution and the parts you implemented.

## Scenario

A retail company wants to provide a simple tool that allows users to:

- Visualize store locations on a map.
- Access information about each store.
- Consult the products available in each location.

The application should consume data from external or simulated sources and present it in a user-friendly way.

## Data Model

You may use any data source you consider appropriate:

- Public APIs
- Mock APIs
- JSON Server
- Static JSON files
- In-memory services

The following structures are expected.

### Stores

```json
{
  "id": 1,
  "name": "Madrid Centro",
  "latitude": 40.4167,
  "longitude": -3.70325
}
```

### Products

```json
{
  "id": 100,
  "storeId": 1,
  "name": "Laptop Lenovo",
  "price": 799,
  "stock": 12
}
```

Each product belongs to a store through the `storeId` field.

## Functional Requirements

### 1. Interactive Map

Display all stores on an interactive map. Each store must be represented by a marker.

Users should be able to:

- Navigate the map.
- Zoom in and out.
- Select a store.

You may use any mapping technology of your choice, such as Leaflet, OpenLayers, Google Maps, MapLibre, or Azure Maps.

### 2. Store Details

When a user selects a store, display at least:

- Store name
- Geographic location
- Number of available products

The presentation format is left to your discretion.

### 3. Product Catalog

Users must be able to view the list of products available in a selected store.

At minimum, show:

- Product name
- Price
- Stock

### 4. Store Search

Provide a mechanism that allows users to search for stores by name.

### 5. Navigation

Use Angular routing to organize the application. The structure of screens and navigation flow is up to you.

### 6. Error Handling

The application should handle failures gracefully, including:

- Data loading errors
- Missing information
- Connectivity issues

Provide meaningful feedback to users when an error occurs.

### 7. Responsive Design

The application should work correctly on both desktop and mobile devices.

## Technical Requirements

The solution must be developed using:

- Angular, preferably the latest stable version
- TypeScript
- Git

You may use any additional libraries that you consider appropriate.

## Deliverables

The challenge must be delivered through a Git repository containing:

### Source Code

A complete and executable application.

### README

The repository must include instructions covering:

- Local setup and development
- Production build
- Docker build and run commands
- Relevant technical decisions
- Future improvements

### Docker Support

The application must be runnable through Docker. A reviewer should be able to start it by following the README instructions.

### Git History

Include the Git history used during development. Meaningful commits are appreciated, but a perfect commit history is not expected.

## Time Expectation

The expected effort is approximately **4 to 8 hours**.

Please prioritize quality and maintainability over the number of implemented features. You do not need to implement every possible improvement.

## Evaluation Criteria

We will evaluate several areas, including but not limited to:

### Functional Requirements

- Correct implementation of the requested features
- Overall usability

### Angular Knowledge

- Component design
- Routing
- Services
- State handling
- Data flow
- TypeScript usage

### Code Quality

- Readability
- Maintainability
- Naming conventions
- Separation of concerns

### Development Practices

- Git usage
- Documentation
- Project organization
- Dockerization

### Technical Judgment

- Decision making
- Prioritization
- Problem solving
- Ability to explain trade-offs

## Open Section

The requirements above represent the minimum expected functionality. Additional features, improvements, optimizations, or enhancements are welcome when they add value.

Examples include improved accessibility, loading states, filtering, sorting, tests, or a polished user experience. Prioritize your additions and explain them briefly in the README.

We are interested in understanding how you identify opportunities, decide what to implement, and work within the available time.

## Review Session

After submission, we may schedule a short technical discussion to review your solution.

Possible discussion topics include:

- Architectural decisions
- Trade-offs and priorities
- Challenges encountered during development
- Potential future improvements
- Production-readiness considerations
- How AI or other tools were used, if applicable

## Final Notes

There is no expectation of a perfect solution. The objective is to understand how you approach development tasks, structure a frontend application, solve problems, communicate technical decisions, and grow beyond the minimum requirements when given freedom to do so.

Good luck, and enjoy the challenge!

```text
                         .-==========-.
                     _.-'   .------.   '-._
                  .-'     .'  .--.  '.     '-.
                .'       /   /####\   \       '.
               /        |   |##/\##|   |        \
              /         |   |#|  |#|   |         \
             ;       .--+---+------+---+--.       ;
             |      /   |  _  ||  _  |   \      |
             |     |    | / \ || / \ |    |     |
             |     |    | \_/ || \_/ |    |     |
             |      \   |____/||\____|   /      |
             ;       '._  .---++---.  _.'       ;
              \          /  _||||_  \          /
               '.       |  / |||| \  |       .'
                 '-._   |_/__||||__\_|   _.-'
                    /\      ||||      /\
                   /  \____/||||\____/  \
                  /     __/||||\__     \
                 /_____/  ||||||  \_____\
                /      \  ||||||  /      \
               /        \_||||||_/        \
              /      .---\||||/---.      \
             /____.-'    /||||\    '-.____\
             |    \     /||||||\     /    |
             |     \___/||||||||\___/     |
             |      |  ||||||||||  |      |
             |      |__||||||||||__|      |
             '------'  ||||||||||  '------'

       MAY THE CODE BE WITH YOU.
       Good luck, and enjoy the challenge!
```
