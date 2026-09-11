# Git Workflow Notes

## Why the repo is the source of truth
- The repository has full history, code review (pull requests), and every teammate has the same copy.
- The org is just a running instance with no version control.
- Team flow: change code -> review -> merge -> deploy to org. The org reflects the repo.

## Key project files
- sfdx-project.json — defines the package directory (force-app)
- force-app/main/default — where all metadata lives
- manifest/package.xml — lists which metadata to pull/push
- .gitignore — keeps secrets (.sf, .sfdx, .env) out of Git

## Package directory
- force-app (marked "default": true in sfdx-project.json)