name: New Issue
description: Description
title: "[Create New Issue]: "
labels: ["GWOC21"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to make an issue!
  - type: textarea
    id: description
    attributes:
      label: Description
      description: Enter a brief description
      placeholder: Please include a summary. Please also include relevant motivation and context. 
      value: "Description"
    validations:
      required: true
  - type: dropdown
    id: version
    attributes:
      label: Field
      description: What Field you want to work on
      options:
        - Android Dev (Flutter)
        - Android Dev (Java)
        - Android Dev (Kotlin)
        - Backend Dev (Java)
        - Backend Dev (.NET)
        - Backend Dev (PHP)
        - Backend Dev (Python)
        - C/CPP
        - Competitive Programming
        - Cyber Security
        - DSA
        - Database
        - Datascience with Python
        - Datascience with R
        - Frontend Dev (HTML, CSS, JS)
        - Frontend Dev (React, Angular, Vue)
        - Golang
        - Interview Prep
        - Java (Domain)
        - JavaScript
        - MERN
        - Machine Learning
        - Open Source
        - Python (Domain)
        - Rust
        - Statistics
        - UI/UX
    validations:
      required: true
  - type: dropdown
    id: contribtype
    attributes:
      label: Type of Contribution
      multiple: true
      options:
        - Audio
        - Video
        - Documentation
        - Others
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct]()
      options:
        - label: I follow [Contributing Guidelines](https://github.com/girlscript/winter-of-contributing/blob/main/.github/CONTRIBUTING.md) & [Code of conduct](https://github.com/girlscript/winter-of-contributing/blob/main/.github/CODE_OF_CONDUCT.md) of this project.
          required: true