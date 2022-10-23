

```databaseTable
sources:
- type: directory
  path: "10 - Projects/10.2 - HomeWork"
fields:
- name: file
  type: fileName
  label: 📚 Name
  dark: true
  width: 1%
- name: start
  label: 🗓️ Start
  type: date
  width: 1%
- name: due
  label: ⏱️ Due
  type: date
  width: 1%
- name: course
  label: 🎒 Class
  type: link
  multiple: true
  width: 20%
  sources:
  - type: directory
    path: "20 - Areas/20.1 Courses"
- name: status
  label: Status
  type: dropdown
  width: 20%
  options:
  - label: In Progress
    value: InProgress
    color: red
    dark: true
  - label: Completed
    value: Completed
    color: green
    dark: true
  - label: Waiting
    value: Waiting
    color: skyblue
    dark: true

- name: notes
  label: 🗒️ Notes
  type: text

```
