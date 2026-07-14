# TPM-OS

**Professional AI skills forged in real TPM work.**

TPM-OS is the open operating system for Technical Program Managers: a growing library of modular skills designed to help TPMs reason clearly, execute confidently, and lead complex programs without surrendering their individual working style.

## Install and use Program Bootstrap

Program Bootstrap turns your existing program files and context into a draft Project Initiation Document and a supporting Excel workbook.

### Step 1 — Download TPM-OS

1. At the top of this GitHub page, click the green **Code** button.
2. Select **Download ZIP**.
3. Open the downloaded ZIP file.
4. Extract it to a folder on your computer.

You may also clone the repository with Git if you already use Git:

```bash
git clone https://github.com/davidrifkind/TPM-OS.git
```

### Step 2 — Find the Program Bootstrap skill

Inside the extracted repository, open:

```text
TPM-OS/
└── skills/
    └── program-bootstrap/
```

Copy the entire `program-bootstrap` folder. Keep its contents together; the skill needs its instructions, workbook schema, template, and interface metadata.

### Step 3 — Open your personal Codex skills folder

Choose the path for your operating system.

**Windows**

1. Open File Explorer.
2. Click the address bar.
3. Enter:

   ```text
   %USERPROFILE%\.agents\skills
   ```

4. Press Enter.
5. If the `.agents` or `skills` folder does not exist, create it.

The expanded path normally looks like:

```text
C:\Users\YOUR-NAME\.agents\skills
```

**macOS or Linux**

Open:

```text
~/.agents/skills
```

If it does not exist, create it with:

```bash
mkdir -p ~/.agents/skills
```

### Step 4 — Install the skill

Paste the copied `program-bootstrap` folder into the `skills` folder.

The final structure must look like this:

```text
.agents/
└── skills/
    └── program-bootstrap/
        ├── SKILL.md
        ├── agents/
        │   └── openai.yaml
        ├── assets/
        │   └── program-bootstrap-template.xlsx
        └── references/
            └── workbook-schema.md
```

Do not copy only `SKILL.md`; copy the entire folder.

### Step 5 — Restart Codex

Close and reopen Codex so it discovers the newly installed skill. If Codex was already closed during installation, open it normally.

### Step 6 — Start Program Bootstrap

Create a new Codex task and enter:

```text
Use $program-bootstrap to analyze my program files and create a draft initiation workbook.
```

Attach the program material you want it to analyze. Useful inputs include:

- strategy decks;
- charters or briefs;
- roadmaps;
- requirements;
- status reports;
- meeting notes;
- RAID registers;
- Jira exports;
- architecture or planning documents.

You do not need a complete document set. Program Bootstrap is designed to work with incomplete or conflicting information and clearly label what is confirmed, reported, inferred, unknown, or conflicting.

### Step 7 — Review the output

Program Bootstrap produces an editable Excel workbook containing:

1. Project Initiation Document;
2. Workstream Map;
3. Deliverables;
4. Workstreams and Measures;
5. RAID register;
6. Evidence and Gaps.

Review the workbook before treating any owner, date, commitment, decision, or approval as final. Human judgment remains the final authority.

## Current phase

TPM-OS is at the beginning of its development.

Our first milestone is intentionally limited to five battle-hardened skills:

1. Session Bootstrap
2. Program Bootstrap
3. OKR Builder
4. Stakeholder Mapper
5. Executive Review Builder

These five skills are our starting point. We will use real-world feedback and product judgment to decide when they are good enough—and when it is time to add Skill #6.

## Built in the real world

These are not speculative prompt experiments.

The first five TPM-OS skills are being battle-tested in real TPM workflows at NVIDIA—against ambiguous programs, complex stakeholder environments, executive expectations, and the everyday pressure of cross-organizational execution.

The goal is simple: each skill must survive contact with real TPM work.

No confidential or proprietary company information belongs in this repository. TPM-OS is an independent open-source project and is not affiliated with or endorsed by NVIDIA.

## Product principles

- Skills augment a TPM's workflow; they do not replace it.
- Each skill performs one clearly defined professional function.
- Deterministic work belongs in software.
- AI is used for reasoning, ambiguity, and communication.
- Human judgment remains the final authority.
- Outputs should be explainable, reviewable, and useful in real programs.
- External models, runtimes, and tools should remain replaceable.
- TypeScript is the default implementation language.

## What "battle-hardened" means

A skill is not complete because it produces a polished document.

It must have:

- Explicit inputs and outputs
- A repeatable workflow
- Validation and evaluation criteria
- Known failure modes
- Representative examples
- Testing with real TPM scenarios
- Evidence that it materially improves the TPM's work

## Who's behind TPM-OS?

TPM-OS was started by David Rifkind, a Technical Program Manager at NVIDIA and a practitioner of complex, cross-functional program execution.

It grew from a practical conviction: TPMs do not need another assistant telling them how to work. They need discrete, trustworthy skills that plug into the way they already operate.

David is building TPM-OS in public, starting with five battle-hardened skills shaped by real programs and real TPM judgment.

## Repository status

This repository currently contains the product foundation. Individual skill specifications and implementations will be introduced through reviewed pull requests.

See [PRD-000](docs/PRD-000.md) for the foundational product requirements and the [initial skill catalog](skills/README.md) for the five-skill scope.

## License

TPM-OS is licensed under the [Apache License 2.0](LICENSE).
