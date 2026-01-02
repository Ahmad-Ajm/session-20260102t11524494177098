# Event Details Page Specification (FEAT-003)

## Overview
The Event Details Page displays comprehensive information about a selected event, including its agenda (if any), organizer details, and an external registration button. The page must fully support Arabic, be responsive, and optimized for low bandwidth.

## Functional Requirements
1. Display full event details:
   - Event name
   - Date and time
   - Location
   - Category
   - Short and full description
   - Agenda (if provided)
   - Organizer name and contact person
   - External registration button (opens URL in new tab)
2. Support for Arabic language in all UI and content.
3. Responsive design for mobile and desktop.
4. Fast loading and minimal UI elements.

## Non-Functional Requirements
- Built with Angular (frontend), ABP Framework (C# backend), SQL Server database.
- API endpoint to fetch event details by event ID.
- All strings and layout must be RTL (right-to-left) for Arabic.
- Page must load quickly and handle slow internet gracefully.

## Data Model (Event)
- Id: Guid
- Name: string
- Date: DateTime
- Time: string
- Location: string
- Category: string
- ShortDescription: string
- FullDescription: string
- Agenda: string (nullable)
- OrganizerName: string
- OrganizerContact: string
- RegistrationUrl: string

## API Example
GET /api/events/{id}
Response:
{
  "id": "...",
  "name": "...",
  "date": "2024-07-01",
  "time": "10:00",
  "location": "...",
  "category": "...",
  "shortDescription": "...",
  "fullDescription": "...",
  "agenda": "...",
  "organizerName": "...",
  "organizerContact": "...",
  "registrationUrl": "https://..."
}

## UI Components
- EventDetailsComponent (Angular)
- Arabic RTL layout and text
- External registration button (opens in new tab)

## Acceptance Criteria
- All event details are displayed correctly in Arabic.
- Page is fully responsive and loads quickly.
- External registration button works and opens the correct URL.
- Organizer and contact info are clearly visible.
- Agenda is shown if provided, otherwise hidden.
