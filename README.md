# The Missing Piece

**Every truth hides a lie.**

A cinematic, browser-based interactive mystery experience. Players investigate a documented real-world case by examining evidence, recording deductions, comparing clues, forming a theory, and reviewing the historical reveal.

## Case 001 — The Great Canadian Maple Syrup Heist

The first case explores the 2011–2012 theft from Quebec's strategic maple syrup reserve. The experience uses a deduction-first approach: players see the clue and make their own interpretation before revealing an investigator's note.

> **Historical integrity note:** The case is based on publicly reported events. The interface, ordering of clues, deduction prompts, and scoring are educational game mechanics—not original police files, actual interview transcripts, or a substitute for court records. Publicly reported roles are summarized cautiously; see `docs/case-research.md`.

## Features

- Cinematic dark-academia interface with antique-gold styling
- Case archive and incident briefing
- Interactive evidence exhibits with player-written deductions and confidence selection
- Suspect/person-of-interest dossiers with clearly labelled educational prompts
- Clue comparison workflow requiring the player to choose a relationship and explain it
- Theory notebook and investigation progress indicator
- Final accusation flow and transparent prototype scoring explanation
- Responsive layout for desktop and mobile browsers
- No build step, dependencies, API keys, or backend required

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser (Chrome, Edge, Firefox, or Safari).
3. Select **OPEN CASE 001** and follow the case flow.

Because this is a static prototype, a local development server is optional. For example, if Python is installed:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Project structure

```text
the-missing-piece/
├── index.html             # Complete self-contained app (HTML, CSS, JavaScript)
├── README.md              # Project overview and setup
├── docs/
│   └── case-research.md   # Research notes, source links, and accuracy caveats
├── LICENSE                # MIT License
└── .gitignore
```

## Tech stack

- HTML5 for semantic page structure
- CSS3 for responsive layout, visual design, modal dialogs, and interaction states
- Vanilla JavaScript for evidence data, navigation, deductions, clue comparison, progress, and final report

## Design decisions

1. **Deduction before explanation:** evidence cards ask the player to interpret a clue before revealing the investigator's note.
2. **Fact versus inference:** case context is labelled, and the UI cautions against treating access or suspicion alone as proof.
3. **Reasoning over guessing:** players must select a relationship between clues and enter a rationale.
4. **Transparent scoring:** the result explains the prototype's scoring rules and explicitly says the score is not a legal judgement.
5. **No API dependency:** the first version is fast to run, inspect, and deploy as a static site.

## Current limitations / next steps

This is an MVP, intentionally built without a backend or external AI service. The clue comparison feedback is rule-based rather than generative AI, and current progress is held in browser memory only. The scoring system is a simple game mechanic and should be improved through playtesting. Next iterations could add:

- A visual detective board where players connect evidence with their own reasoning
- Persistent save/resume using local storage or a backend
- A more rigorous clue dependency graph and case-specific scoring rubric
- Accessibility improvements and keyboard-only testing
- Additional researched cases with source review and careful fact-checking
- Automated tests for the case flow and interactive controls

## Resume-ready description

**The Missing Piece — Interactive Mystery Investigation Web App**  
Designed and built a responsive, browser-based mystery game using HTML, CSS, and vanilla JavaScript. Created an evidence-first investigation flow with player-written deductions, confidence ratings, clue comparison, suspect dossiers, theory tracking, progress feedback, and a transparent final report. Structured the experience to distinguish documented facts from inference and avoid revealing solutions before the player reasons through the evidence.

Use only claims that accurately reflect what you personally built and tested. As this is an early MVP, describe it as a prototype unless you have completed broader testing and deployment.

## License

MIT. See `LICENSE`.
