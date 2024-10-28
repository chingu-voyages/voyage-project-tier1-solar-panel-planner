# voyage-project-tier1-solar-panel-planner

## Table of Contents

* [Overview](#overview)
* [General Instructions](#general-instructions)
* [Requirements & Specifications](#requirements-specifications)
* [Acknowledgements](#acknowledgements)
* [About Chingu](#about-chingu)

## Overview

Welcome, Chingus!

The city of Los Angeles is encouraging residents to install private solar panels as part of a local initiative to combat global warming. This project provides a free service where a city-hired specialist evaluates the installation and maintenance costs of solar panels. The initial MVP is a web-based application enabling residents to schedule appointments and allowing city employees to manage and plan these visits effectively.

![Solar Panel Installation](./assets/solar-panel-installation.jpg)

In this voyage, your team will create a user-friendly solar panel planning application that simplifies the process of scheduling evaluations. Get ready to combine your problem-solving skills and creativity to build a tool that makes solar panel installation and maintenance planning a breeze!

The application supports two main roles:

**Resident:** Can request an appointment for a solar panel evaluation by submitting their contact details, address, and preferred timeslot.

**City Hall Employee:** Can access appointment requests, generate visit schedules for specialists, and export planning details in a downloadable/printable format.

![Example Solar Energy App](./assets/example-solar-energy-app.png)

## General Instructions

This project is designed to be worked on by a team rather than an individual
Chingu. This means you and your team will need to thoroughly read and
understand the requirements and specifications below, **_and_** define and
manage your project following the _Agile Methodology_ defined in the
[Voyage Handbook](https://github.com/chingu-voyages/Handbook/blob/main/docs/guides/voyage/voyage.md#voyage-guide).

As you create this project make sure it meets all of the requirements, but once
it reaches MVP, start implementing the optional features or get creative and
extend it in ways we haven't envisioned. In other words, use the power of
teamwork to make it distinctive and unique.

Take note that we haven't given specific direction on what your UI/UX should
look like. This is another area where you and your team can put your creativity 
to work! 

## Requirements & Specifications

### What You Need to Do

The following define the minimum requirements and ideas for features you may
implement to enhance this app, if time permits.

#### Structure

- [ ] This is a purely frontend application. No backend is required.
- [ ] You may use any languages, tools, or libraries you prefer when designing and building this app.
- [ ] You may **_NOT_** use AI-based solution generators like GitHub Copilot.

#### Styling

- [ ] Surprise us!!! Use your team's creativity to make this app distinctive.
- [ ] Add a footer containing a link to your team's GitHub repo.
- [ ] In general, you will find these [UI design principles](https://www.justinmind.com/ui-design/principles) helpful.
- [ ] Recommend using this resource for [clean CSS](https://israelmitolu.hashnode.dev/writing-cleaner-css-using-bem-methodology).

#### Functionality
- Overview

  - [ ] Develop a single-page application (SPA) for solar panel application.

- Resident Interface

  - [ ] Allow residents to submit a request for a solar panel evaluation by completing a web form with:
    - Name
    - Email
    - Phone Number
    - Address (validated against a provided dataset of Los Angeles addresses)
    - Preferred timeslot
  - [ ] Notify residents that their preferred timeslot is only indicative and that they will receive confirmation a few hours before the scheduled visit.
  - [ ] Store the request status (e.g., pending, visited) using local storage or IndexedDB.
  - [ ] Allow residents to cancel an appointment using an application code sent to their email.

- Admin Interface

  - [ ] Implement a login system accessible through /admin URL where city hall employees can enter an approved email to access the Admin page (no complex authentication required, emails can be validated against a list in a .env file).
  - [ ] Display all appointment requests submitted by residents.
  - [ ] Allow employees to retrieve the most efficient planning for a specified time period (e.g., daily, weekly).
  - [ ] Provide an option to export the planned visits in a downloadable format (PDF, Excel, etc.) with details such as visit time slot, resident’s contact information, and address.

  - Algorithmic Planning

  - [ ] Develop a basic scheduling algorithm that optimizes visit order based on address proximity, traffic, and average visit duration (30 minutes).
  - [ ] Prioritize efficiency, aiming to minimize travel time between consecutive visits.
  - [ ] Example Simple Algorithm: For adjacent addresses, order them by street name and number for consecutive visits.

  - Data Management

  - [ ] Use local storage or IndexedDB to temporarily save resident requests.
  - [ ] Implement data validation to ensure addresses match the provided dataset.

### Extras (Not Required)


## Acceptance Criteria

- Resident Interface

- [ ] Users can submit requests with valid addresses, personal details, and timeslots.
- [ ] Preferred timeslots are submitted but are not guaranteed.
- [ ] Requests persist across sessions in local storage or IndexedDB.
- [ ] Users can cancel appointments using an application code sent to their email.

- Admin Interface

- [ ] Admins can view all resident requests.
- [ ] Admins can generate and print/export the optimized visit schedule.
- [ ] The login restricts access to approved city hall employee emails only.

- Scheduling Algorithm

- [ ] Planning considers the efficiency of visit order based on address and time constraints.
- [ ] Schedule export format includes time slot, address, and contact information for each appointment.

## Acknowledgements

We extend our heartfelt gratitude to the wider developer community, whose invaluable insights and expertise consistently inspire and elevate our projects. We are also deeply thankful for the powerful tools and services provided by [Google](https://google.com), [Cloudinary](https://cloudinary.com), and [AWS](https://aws.amazon.com), which play a crucial role in making our journey possible. Your contributions and innovations drive our success, and for that, we are sincerely grateful.

## About Chingu

If you aren't yet a member of Chingu we invite you to join us. We help our
members transform what they've learned in courses & tutorials into the
practical experience employers need and want.
