# Task List

This file shows the current progress of all tasks in this project.
It is automatically updated by dev0 as tasks are completed.

---

## Phase 1

- [ ] ⏳ **Implement LocalStorage Utility and Mock Data**
  Create a robust client-side storage utility using `localStorage` to persist application state. Define and seed initial mock data including users (patients and staff), patient records, and historical/upcoming appointments. Acceptance Criteria: A utility file exports functions to get, set, and initialize data. The app seeds default data on first load if localStorage is empty.

- [ ] ⏳ **Implement Auth Context and Role-Based Routing**
  Create an Authentication Context to simulate user login. Implement a simple login screen where a user can select to log in as a 'Patient' or 'Staff'. Set up React Router with protected routes based on the active role. Acceptance Criteria: Users can log in/out. Staff are routed to a staff dashboard; patients are routed to a patient dashboard. Unauthorized access redirects to the login page.

## Phase 2

- [ ] ⏳ **Build Patient Dashboard UI**
  Develop the main dashboard for patients. It should display a welcome message, a list of upcoming appointments, and a brief history of past appointments. Acceptance Criteria: Dashboard renders correctly using shadcn/ui cards and lists. Data is pulled from the LocalStorage utility based on the logged-in patient's ID.

- [ ] ⏳ **Build Staff Dashboard and Calendar View**
  Develop the staff dashboard featuring an interactive calendar view (using a simple CSS grid or a lightweight library) to display all clinic appointments. Include a sidebar or summary cards for daily metrics. Acceptance Criteria: Staff can view appointments by day/week. Clicking an appointment opens a details modal. Data is accurately fetched from LocalStorage.

- [ ] ⏳ **Implement Appointment Booking Flow**
  Create a multi-step form or modal for booking new appointments. Patients select a service, date, and time slot. Staff can do the same but must also select a patient. Acceptance Criteria: Form validates inputs. Available time slots are dynamically calculated based on existing appointments. Submitting saves the new appointment to LocalStorage and updates the UI.

- [ ] ⏳ **Implement Patient Records Management (CRUD)**
  Create a dedicated view for staff to manage patient records. Include a data table listing all patients, with actions to view details, edit history, or add a new patient. Acceptance Criteria: Staff can create, read, update, and delete patient profiles. Changes persist to LocalStorage. The table includes search and basic filtering.

## Phase 3

- [ ] ⏳ **Develop AI No-Show Prediction Engine**
  Write a client-side heuristic algorithm that calculates a 'no-show risk score' (0-100%) for an appointment. Factors should include the patient's historical cancellation rate, time of day, and days since last visit. Acceptance Criteria: A utility function takes an appointment and patient data, returning a risk score and a risk category (Low, Medium, High).

- [ ] ⏳ **Develop AI Predictive Scheduling Engine**
  Write a client-side algorithm to suggest optimal appointment times. It should analyze clinic load (finding days with fewer appointments) and patient history (preferring times they usually book). Acceptance Criteria: A utility function returns an array of 3 'Recommended Slots' when given a date range and patient ID.

- [ ] ⏳ **Integrate AI Features into UI**
  Update the Staff Calendar to display warning badges on high-risk no-show appointments using the engine from task-7. Update the Booking Flow to prominently display 'AI Suggested Times' using the engine from task-8. Acceptance Criteria: Visual indicators for no-show risks appear on the staff dashboard. The booking form includes a 'Suggested Times' quick-select section.

## Phase 4

- [ ] ⏳ **Implement In-App Notifications System**
  Create a notification context and a toast UI component to simulate alerts. Trigger notifications when a new appointment is booked, or when an appointment is 24 hours away (simulated on login). Acceptance Criteria: Toast notifications appear in the corner of the screen for key actions. A notification bell in the header shows a history of recent alerts.

---

_Last updated by dev0 automation_
