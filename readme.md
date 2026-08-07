# iFarm

- [Introduction](#introduction)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Inspiration](#inspiration)

## Introduction

Ever wondered how you'd conduct surveillance farming? look no further. this system enables one to have become the "Big brother" on your own farm, always monitoring your livestock and plants despite of the distance. you get timely reminders of their feeding/watering schedules, quickly detect ailing animals/plants before they spread any ailments to the rest and are able to view any intruders that might decide to give you a visit. all this being just the tip of the iceberg...

## Features

- [ ] **Plants**
- [ ] **Animals**
    - [ ] **ML Module**:
        - [ ] build a facial recognition model, allow to distinguish between regulars and intruders in the pen.
        - [ ] build a facial recognition model to tag animals.
        - [ ] allow for live notifications, via SMS or email, of what is going on in the barn, e.g an intruder appears or maybe the animal is in distress.
        - [ ] monitor animals for different ailments and be able to flag them appropriately. send notification alerts for confirmed ailments, e.g chicken hunching over might be sick. Also it will be handy on early detection of chicken diseases and reporting.
        - [ ] have a count of all the animals in a barn to ensure none went missing.
        - [ ] send remainders for feeding times with correct quantities of feed to give.
        - [ ] calculate feed remaining in store, and be able to track it accordingly, giving urgent notifications, via email or SMS when it is about to run out, say T-3 days.

    - [ ] **IoT Module**:
        - [ ] have a live stream camera, broadcast on a secure channel
        - [ ] stream should broadcast over wifi if available, and default to bluetooth essentially.
        - [ ] embed stream within webapp.
        - [ ] be able to play certain predefined sounds when a given condition is met, say an intruder gets into the barn.
        - [ ] play live audio from webapp, allow for a sort of conversational call with someone in the barn.

    - [ ] **Webapp Module**:
        - [ ] **User Roles & Permissions** - implement RBAC(Role Based Access) within the application. This will include 2 main roles at first:
            - admin: allow for priviledged access incase trouble-shooting is necessary.
            - farmer: normal day to day use.
        - [ ] **Social Authentication** - allow users to login with third party services into the app. Primarily this will be using Google only, but more applications can be added on the fly.
        - [ ] **Two-Factor Authentication (2FA)** - Add an additional layer of security by integrating two-factor authentication. Using a users email, connection via Google Authenticator or an SMS-based verification should be essential.
        - [ ] **Password Reset Flow** - Add a password recovery option where users can request a reset link.
        - [ ] **Session Management** - Manage how long a user can remain logged in without any activity.
        - [ ] **Logging** - log all major actions performed in the program
        - [ ] **Testing** - Writing thorough unit, integration and e2e tests.
        - [ ] **Docker** - containerize the application using docker to allow for easier deployment to whatever platform I'll use.

## Tech Stack

- Database: MariaDb
- Frontend: Jinja2 templates & Bootstrap
- Backend: FastAPI

## Inspiration

iFarm was initially the title of my final year project, which turned out just [fine](https://github.com/mbvgua/iFarm/tree/1c944ebf704ce9d0dc6006dbd66c988811b0f74f), however over the years I gravitated towards building farm oriented applications and systems, and this led me to build on top of it. Hopefully its gotten better with every re-write :)
