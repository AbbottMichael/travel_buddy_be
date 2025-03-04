![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/81139173/142697132-dbc9d6ae-70ad-495d-a827-61235788512e.gif)

## Travel Buddy -(back end)

[Deployed to Heroku](https://travel-buddy-api.herokuapp.com/)

[![Contributors][contributors-shield]][contributors-url]
[![Issues][issues-shield]][issues-url]
[![Stargazers][stars-shield]][stars-url]
[![Forks][forks-shield]][forks-url]
# Welcome to Travel Buddy
  - The frustrating part about planning a trip with friends is keeping track of all the details. Wouldn’t it be easier if all the details were in one place for all to see? Travel Buddies makes it easy to organize a trip while keeping everyone involved on the same page.

## Table of Contents

- [Overview](#overview)
- [Tools Utilized](#tools-used)
- [Getting Started](#getting-started)
- [Endpoints](#endpoints)
- [Database Schema](#database-schema)
- [Contributing](#contributors)

# README
------

### <ins>Overview</ins>

[Travel Buddy](https://github.com/antoniojking/travel_buddy_be) is a 10 day, 6 person project. The idea was to build a web application that allows users to connect and plan trips to national parks.

- Apply principles of flow control across multiple methods
- Design a one to many relationship using an API backend application
- Design a many to many relationship using an API backend application
- Design self referential relationship using an API backend application
- Write migrations to create tables with columns of varying data types and foreign keys.
- Use Rails to create web pages that allow users to CRUD resources
- Use Rails to allow users to connect with other users
- Create instance and class methods on a Rails model
- Write model and feature tests that fully cover data logic and potential user behavior


## Tools Used

| Development | Testing       | Gems            |
|   :----:    |    :----:     |    :----:       |
| Ruby 2.7.2  | RSpec         | Pry             |
| Rails 5.2.5 | WebMock       | ShouldaMatchers |
| PostgresSQL | VCR           | Capybara        |
| Postico     | Launchy       | Figaro          |
| Atom        | SimpleCov     | Faraday         |
| Github      | Capybara      |                 |
|             | FactoryBot    |                 |


## Getting Started

The `base path` of each endpoint is:

```
https://travel-buddy-api.herokuapp.com/api/v1
```

## Endpoints

The following table presents each API endpoint and its documentation.

Endpoint | Docs/Example
---------|-------------
Get One User | GET /api/v1/users/{user_id}
Find or Create User | GET /api/v1/users/{user_id}
Get User Friendships | GET /api/v1/users/{user_id}/friendships
Create User Friendship | POST /api/v1/users/{user_id}/friendships
Get One Trip | GET /api/v1/trips/{trip_id}
Create Trip | POST /api/v1/trips
Update Trip | PATCH /api/v1/trips/{trip_id}
Get Trips Accommodations | GET /api/v1/trips/{trip_id}/accommodations
Get single Trip Accommodation | GET /api/v1/trips/{trip_id}/accommodations/{accommodation_id}
Create Trip Accommodation | POST /api/v1/trips/{trip_id}/accommodations
Update Trip Accommodation | PATCH /api/v1/trips/{trip_id}/accommodations/{accommodation_id}
Delete Trip Accommodation | DELETE /api/v1/trips/{trip_id}/accommodations/{accommodation_id}
Get Trips Travel Buddies | GET /api/v1/trips/{trip_id}/travel_buddies
Create Trip Travel Buddy | POST /api/v1/trips/{trip_id}/travel_buddies
Get Trip Checklists | GET /api/v1/trips/{trip_id}/checklists
Get single Trip Checklist | GET /api/v1/trips/{trip_id}/checklists/{checklist_id}
Create Trip Checklist | POST /api/v1/trips/{trip_id}/checklists
Get Trip Checklist Items| GET /api/v1/trips/{trip_id}/checklists/{checklist_id}/checklist_items
Create Trip Checklist Item | POST /api/v1/trips/{trip_id}/checklists/{checklist_id}/checklist_items
Update Trip Checklist Item | PATCH /api/v1/trips/{trip_id}/checklists/{checklist_id}/checklist_items/{checklist_item_id}
Delete Trip Checklist Item | DELETE /api/v1/trips/{trip_id}/checklists/{checklist_id}/checklist_items/{checklist_item_id}
Get NPs by State | GET /api/v1/parks?state='WY'
Get NPs by Activity | GET /api/v1/parks?activity='Fishing'
Get NP by Park Code | GET /api/v1/parks/{park_code}
Get Weather | GET /api/v1/weather


## Database Schema
![Screen Shot 2021-09-19 at 10 57 04 AM](https://user-images.githubusercontent.com/81600649/133936054-baac51fb-f3f0-4951-86e2-07f431c02253.png)

### <ins>Contributors</ins>

👤  **Antonio King**
- Github: [Antonio King](https://github.com/antoniojking)
- LinkedIn: [Antonio King](https://www.linkedin.com/in/antoniojking/)

👤  **Elliot Olbright**
- Github: [Elliot Olbright](https://github.com/ElliotOlbright)
- LinkedIn: [Elliot Olbright](https://www.linkedin.com/in/elliotolbright/)

👤  **Carina Sweet**
- Github: [Carina Sweet](https://github.com/chsweet)
- LinkedIn: [Carina Sweet](https://www.linkedin.com/in/carina-h-sweet/)

👤  **Michael Abbott**
- Github: [Michael Abbott](https://github.com/AbbottMichael)
- LinkedIn: [Michael Abbott](https://www.linkedin.com/in/mjabbottdesign/)

👤  **Matt Kragen**
- Github: [Matt Kragen](https://github.com/matt-kragen)
- LinkedIn: [Matt Kragen](https://www.linkedin.com/in/mattkragen/)

👤  **Matt Toensing**
- Github: [Matt Toensing](https://github.com/matttoensing)
- LinkedIn: [Matt Toensing](https://www.linkedin.com/in/matt-toensing/)

<!-- MARKDOWN LINKS & IMAGES -->

[contributors-shield]: https://img.shields.io/github/contributors/antoniojking/travel_buddy_be.svg?style=flat-square
[contributors-url]: https://github.com/antoniojking/travel_buddy_be/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/antoniojking/travel_buddy_be.svg?style=flat-square
[forks-url]: https://github.com/antoniojking/travel_buddy_be/network/members
[stars-shield]: https://img.shields.io/github/stars/antoniojking/travel_buddy_be.svg?style=flat-square
[stars-url]: https://github.comantoniojking/travel_buddy_be/stargazers
[issues-shield]: https://img.shields.io/github/issues/antoniojking/travel_buddy_be.svg?style=flat-square
[issues-url]: https://github.com/antoniojking/travel_buddy_be/issues
<!--

<!-- Docs -->
[get-one-user-docs]: /doc/travel_buddy_endpoints.md#get-one-user
[find-or-create-user-docs]: /doc/travel_buddy_endpoints.md#find-or-create-user
[get-user-friendships-docs]: /doc/travel_buddy_endpoints.md#get-user-friendships
[create-user-friendships-docs]: /doc/travel_buddy_endpoints.md#create-user-friendship
[get-one-trip-docs]: /doc/travel_buddy_endpoints.md#get-one-trip
[create-user-trip-docs]: /doc/travel_buddy_endpoints.md#create-user-trip
[update-user-trip-docs]: /doc/travel_buddy_endpoints.md#update-user-trip
[get-trips-accommodations-docs]: /doc/travel_buddy_endpoints.md#get-trip-accommodations
[create-trip-accommodation-docs]: /doc/travel_buddy_endpoints.md#create-trip-accommodation
[get-trips-travel-buddies-docs]: /doc/travel_buddy_endpoints.md#get-trip-travel-buddies
[create-trip-travel-buddy-docs]: /doc/travel_buddy_endpoints.md#create-trip-travel-buddy
[get-trip-checklists-docs]: /doc/travel_buddy_endpoints.md#get-trip-checklists
[create-trip-checklist-docs]: /doc/travel_buddy_endpoints.md#create-trip-checklist
[create-checklist-item-docs]: /doc/travel_buddy_endpoints.md#create-checklist-item
[get-parks-by-state-docs]: /doc/travel_buddy_endpoints.md#get-parks-by-state
[get-parks-by-activity-docs]: /doc/travel_buddy_endpoints.md#get-parks-by-activity
[get-park-by-parkcode-docs]: /doc/travel_buddy_endpoints.md#get-park-by-parkcode
[get-weather-docs]: /doc/travel_buddy_endpoints.md#get-weather
