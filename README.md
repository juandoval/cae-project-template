# CAE Project Template

A Typst template for managing simulation consulting projects from proposal through final delivery.

## Structure

1. Cover page with project metadata and status tracking
2. Proposal — scope, objectives, deliverables, assumptions, limitations
3. Traceability — version history, decision log, issue tracker, client communications
4. Model Definition — geometry, mesh, physics, boundary conditions
5. Verification — convergence, mesh independence, y+ checks
6. Results — KPIs, visualizations, observations
7. Interpretation — engineering analysis, recommendations, next steps
8. Appendix — solver settings, file hashes, reference standards

## Usage

Edit the `project-info` dictionary at the top of the file with your project details. Fill sections as the project progresses.
```typst
#let project-info = (
  client: "Client Name",
  project: "Project Title",
  project-id: "PRJ-001",
  author: "Your Name",
  date: "January 2025",
  version: "v1.0",
  status: "Proposal", // Proposal | In Progress | Review | Complete
)
```

## Compile
```bash
typst compile cae-project-template.typ
```

## References

- ASME V&V 20-2009
- AIAA G-077-1998
