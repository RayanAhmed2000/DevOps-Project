# CI/CD Build Pipeline

- install plugin **Build Pipeline**
## open Job **githubpull** 
- Post-build Actions
- Build other projects
- buildandcodereview
- Trigger only if build is stable
## open Job **buildandcodereview**
- Post-build Actions
- Build other projects
- unit test
- Trigger only if build is stable
## open Job **unit test**
- Post-build Actions
- Build other projects
- deploy
- Trigger only if build is stable

# Build Pipeline and tell which job to start first
- dashboard
- click '+' next to All
- Give Name
- Complete Pipeline
- Build pipeline View
- Create
- Upstream / downstream config
- githubpull
- Apply
- Save

# Poll SCM in githubpull
- open job githubpull
- Build Triggers
- Poll SCM
- Schedule
- '*****'
- Apply 
- Save



 
