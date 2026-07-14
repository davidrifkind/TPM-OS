# Install and use Program Bootstrap

Program Bootstrap turns your existing program files and context into a draft Project Initiation Document and a supporting Excel workbook.

## Step 1 — Download TPM-OS

1. At the top of this GitHub page, click the green **Code** button.
2. Select **Download ZIP**.
3. Open the downloaded ZIP file.
4. Extract it to a folder on your computer.

You may also clone the repository with Git if you already use Git:

```bash
git clone https://github.com/davidrifkind/TPM-OS.git
```

## Step 2 — Find the Program Bootstrap skill

Inside the extracted repository, open:

```text
TPM-OS/
└── skills/
    └── program-bootstrap/
```

Copy the entire `program-bootstrap` folder. Keep its contents together; the skill needs its instructions, workbook schema, template, and interface metadata.

## Step 3 — Open your personal Codex skills folder

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

## Step 4 — Install the skill

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

## Step 5 — Restart Codex

Close and reopen Codex so it discovers the newly installed skill. If Codex was already closed during installation, open it normally.

## Step 6 — Start Program Bootstrap

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

## Step 7 — Review the output

Program Bootstrap produces an editable Excel workbook containing:

1. Project Initiation Document;
2. Workstream Map;
3. Deliverables;
4. Workstreams and Measures;
5. RAID register;
6. Evidence and Gaps.

Review the workbook before treating any owner, date, commitment, decision, or approval as final. Human judgment remains the final authority.

[Return to the TPM-OS README](../README.md)
