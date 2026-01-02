# Tasks for FEAT-002: Event Listing

## Backend (C# / ABP Framework)
- [x] Design Event entity (fields: name, date, time, location, category, short description, organizer).
- [x] Implement Event repository/service for CRUD operations (initially only read/list).
- [x] Create API endpoint to fetch ongoing and upcoming events (filter by date/time).
- [x] Add pagination and basic filtering (by category, date).
- [x] Seed database with sample events for testing.

## Frontend (Angular)
- [x] Create Event List component/page.
- [x] Fetch events from backend API and display them in a responsive grid/list.
- [x] Show essential event details: name, date, time, location, category, short description, organizer.
- [x] Implement loading state and error handling for event list.
- [x] Ensure Arabic language support for all labels/content.
- [x] Make the event list responsive for mobile devices.

## QA & Testing
- [x] Test event listing with various screen sizes and slow internet.
- [x] Validate correct filtering and pagination.
- [x] Confirm Arabic text is displayed correctly.

## Documentation
- [x] Document API endpoints and event entity fields.
- [x] Update user guide for event browsing feature.
