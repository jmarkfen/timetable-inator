# timetable-inator

A timetable maker and viewer based on the format I encountered in EVSU.

## Features

* Create multiple timetables.
* Show overlapping events on a timetable.
* Print timetables.
* Multiple users.

## Roadmap

Sprint #1: Environment and project setup

- [ ] install [Django](https://docs.djangoproject.com/en/4.2/topics/install/)
- [ ] install [django-browser-reload](https://github.com/adamchainz/django-browser-reload/)
- [ ] create Django server
- [ ] install app scaffolding
- [ ] install [Bootstrap toolkit](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- [ ] install [Popper](https://unpkg.com/@popperjs/core@2)
- [ ] create template for bootstrap base page
- [ ] create template for bootstrap card component
- [ ] create template for save button

Sprint #2: Basic operations on timetables

- [ ] scaffolding: models, views, templates, urls for timetables
- [ ] feature: create timetable
- [ ] feature: timetable list
- [ ] integration: create button on timetable list
- [ ] feature: edit timetable details
  - reuse form from 'create timetable'
- [ ] integration: edit button on timetable list
- [ ] feature: delete timetable
  - show confirmation
- [ ] integration: delete button on timetable details

Sprint #3: Basic operations on events

- [ ] scaffolding: models, views, templates, urls for events
- [ ] feature: create event
- [ ] feature: event list
- [ ] feature: edit event details
- [ ] feature: delete event
- [ ] integration: delete button on event details

Sprint #4: Display events as timetable

- [ ] feature: show timetable table, including overlapping events
  - create function to group events by day then sort each group by time
  - create function to identify and organize overlapping events
  - create function to format data for html table, with rowspan for events and colspan for column headings

Sprint #5: Enhancements and extra functionality

- [ ] feature: tabs to display events as list or timetable
- [ ] feature: print timetable
  - find package to convert html to pdf

Sprint #6: User authentication

- [ ] feature: user login
  - use django's login view
- [ ] feature: user logout
  - use django's logout view
- [ ] feature: user registration
  - use django's registration view

Sprint #7: Customization

- [ ] feature: toggle light/dark mode

## Git Workflow

1. Write down a task `do abc`
2. Create a new branch `do-abc` (you can copy-paste the task)
3. Make commits on branch `do-abc`
4. Rebase `do-abc` with `main` to be able to fast-forward merge
5. Squash and merge `do-abc` to `main`
6. Edit merge message to match task `do abc`
