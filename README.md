# Harvey Brown Dental Clinic App

> Smart dental appointment management with AI-driven insights.

## Overview
The Harvey Brown Dental Clinic App is a modern, responsive single-page application designed to streamline appointment scheduling and clinic management. It serves both clinic staff and patients, providing tailored dashboards for booking appointments, managing schedules, and maintaining patient records.

To optimize clinic operations, the application features client-side "AI" integrations. Using heuristic algorithms, the system provides **predictive scheduling** to suggest optimal appointment times and calculates **no-show risk scores** to help staff proactively engage with at-risk patients.

## Tech Stack
- **Framework:** React + Vite
- **Styling:** Tailwind CSS
- **UI Components:** shadcn/ui
- **Icons:** Lucide React
- **Data Persistence:** Client-side `localStorage` (No backend required)

## Features
- **Role-based Access:** Distinct experiences for Patients and Staff/Dentists.
- **Interactive Calendar:** Comprehensive daily, weekly, and monthly views for staff.
- **Self-Service Booking:** Easy-to-use appointment scheduling, rescheduling, and cancellation.
- **Patient Management:** Full CRUD capabilities for patient records and history.
- **AI No-Show Prediction:** Heuristic scoring system that flags high-risk appointments.
- **Predictive Scheduling:** Smart time-slot suggestions based on clinic load and historical preferences.
- **In-App Notifications:** Simulated alerts and reminders for upcoming appointments.

## Getting Started

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Run the development server:**
   ```bash
   npm run dev
   ```

3. **Build for production:**
   ```bash
   npm run build
   ```

## Documentation
- [TASKLIST.md](./TASKLIST.md) - Detailed breakdown of project tasks and phases.
- [LEARNINGS.md](./LEARNINGS.md) - Developer notes and architectural decisions.
- [.dev0/RULES.md](./.dev0/RULES.md) - AI agent instructions and coding standards.