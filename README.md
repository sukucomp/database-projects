# database-projects
A working collection of database-management scripts, runbooks, and case studies. Built to close operational gaps that databases managed layer doesn't cover on its own.

## Who I am?

I'm a systems engineer with experiences across maintenance engineering, IT consulting, and cloud infrastructure. I've worked with Azure and AWS.

## Why this repo exists?

None of what's here started as a portfolio piece. Each project began as an incident, a recurring gap, or a question database had no native answer for. I ended up writing a script because the alternative was solving the same problem from memory the next time it came up. I'm publishing them because a script that only lives in one instance's job history helps no one else, and because I'd genuinely rather compare notes with other people doing this work than assume I've found the only way to solve it.

Some of these were built the traditional way, hand-written and refined over time. Others were built with the help of an AI coding assistant, with me driving the requirements, the database-specific edge cases, and the production validation. I've noted which is which in each project's own README.

## What to expect?

Each project lives in its own folder with a README explaining the problem it solves, the approach, and — where relevant — what actually happened when it ran in production, including the parts that didn't work as intended. 

Feedback, alternative approaches, and pull requests are welcome.

## Repository structure
```
database-projects/
├── db/
│   └── sql-db/
│       ├── dms-cdc-setup-rds-sql-server/
│       │   ├── enable-cdc.sql
│       │   └── readme.md
│       ├── extended-events-to-audit-tempdb-growth/
│       │   ├── 1-xe-session.sql
│       │   ├── 2-utility-db-tables.sql
│       │   ├── 3-capture-proc.sql
│       │   ├── 4-scheduling.sql
│       │   ├── 5-retention.sql
│       │   ├── 6-investigation.sql
│       │   └── readme.md
│       ├── fixing-slow-queries-by-adding-database-indexes/
│       │   ├── index-deployment-case-study.sql
│       │   └── readme.md
│       ├── rds-sql-backup-restore-user-role-preservation/
│       │   ├── 1-backup-database.sql
│       │   ├── 2-capture-user-mappings.sql
│       │   ├── 3-restore-database.sql
│       │   ├── 4-replay-user-mappings.sql
│       │   └── readme.md
│       └── table-growth-tracker/
│           ├── readme.md
│           └── table-growth-tracker.sql
└── README.md
```
