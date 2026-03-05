---
name: Bug report
about: Report a bug or other problem
title: Bug Report
labels: bug
assignees: ''

---

name: Bug Report
description: Report a problem with the game
title: "[BUG] "
labels: ["bug"]

body:
  - type: textarea
    id: description
    attributes:
      label: What happened?
      description: Describe the bug
      placeholder: The game crashed after finishing a race.
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Steps to reproduce
      placeholder: |
        1. Start race
        2. Finish race
        3. Game crashes

  - type: textarea
    id: expected
    attributes:
      label: Expected behavior

  - type: dropdown
    id: platform
    attributes:
      label: Platform
      options:
        - Windows
        - Linux
        - Android
        - iOS

  - type: input
    id: version
    attributes:
      label: Game version

  - type: textarea
    id: logs
    attributes:
      label: Logs or screenshots
