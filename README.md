# SpaceDock-home-assignment-
author: Jakub Stejskal


## 🛰️ EPIC 1 — Ship Traffic Monitoring

**Goal**  
Provide real-time overview of ships around and within the station.

**User Stories**
- View list of all currently docked ships
- View list of ships in station airspace (callsign, class)
- Distinguish scheduled vs. unscheduled / unknown ships
- Expand ship entry to view full ship detail
- Display scan warnings (explosives, alien infestation, reactor leakage) in list & detail
- Filter ships by status

**Actors**
- Space Traffic Controller
- Station Director (read-only)

---

## 🔗 EPIC 2 — Docking & Undocking Operations

**Goal**  
Enable operational handling of physical docking processes.

**User Stories**
- Assign a docking port to an arriving ship
- Change assigned docking port
- Undock a docked ship
- Initiate refueling for a docked ship

**Actors**
- Space Traffic Controller

---

## 📋 EPIC 3 — Landing & Takeoff Request Management

**Goal**  
Manage formal approval workflow for docking and departure.

**User Stories**
- Captain submits docking request
- Captain submits takeoff request
- Enforce one request per ship per day limit
- Controller approves/denies docking request
- Controller approves/denies takeoff request
- Director approves/denies unscheduled docking request
- Director approves/denies unscheduled takeoff request
- Change approval decision before docking/departure
- Maintain audit trail for all requests and decisions

**Actors**
- Ship Captain
- Space Traffic Controller
- Station Director
- Audit System

---

## 🔄 EPIC 4 — Ship Status & State Management

**Goal**  
Ensure consistent and valid lifecycle of ship states.

Ship status is governed by a controlled state model.

**User Stories**
- System automatically updates ship status based on workflow events
- Display ship status in list and detail
- Filter ships by status
- Transition ship to "Quarantined"
- Prevent invalid state transitions
- Maintain history of status changes

**Actors**
- System
- Space Traffic Controller

---

## 📡 EPIC 5 — Ship Communication Integration

**Goal**  
Enable secure communication between station and ships.

**User Stories**
- Initiate voice transmission to a selected ship
- Pass ship frequency and encryption codes to External Comms System
- Log communication initiation events

**Actors**
- Space Traffic Controller
- External Comms System

---

## 📅 EPIC 6 — Flight Schedule Management

**Goal**  
Manage planned arrivals and departures.

**User Stories**
- Create scheduled flight (flight number, ship, date, destination)
- Update scheduled flight
- Delete scheduled flight
- List all scheduled flights
- Edit flights in draft mode
- Publish draft flight schedule
- Assign ship to scheduled flight

**Actors**
- Station Director

---

## 💰 EPIC 7 — Docking Fees & Billing

**Goal**  
Manage financial aspects of docking operations.

**User Stories**
- Manage docking fee schedule / pricing
- Apply docking fee to a docked ship
- View docking fee summary

**Actors**
- Station Director

---

## 🛂 EPIC 8 — KYC & Passenger Verification

**Goal**  
Ensure regulatory compliance and passenger validation.

**User Stories**
- View persons on ship crew roster
- View person detail with flight history (dates, departure, destination, ship)
- View person’s citizenship status within Human Colony Federation
- Run KYC check on passengers entering the station

**Actors**
- Station Director

---

## 🖥️ EPIC 9 — Public Information Displays

**Goal**  
Provide arrival/departure information for station crew and visitors.

**User Stories**
- Display scheduled arrivals on lobby screens (airport-style)
- Display scheduled departures on lobby screens
- Display arrivals/departures at docking port screens
- Automatically refresh information

**Actors**
- Station Crew (passive consumer)

---

## 🔔 EPIC 10 — Notifications

**Goal**  
Inform stakeholders about critical workflow events.

**User Stories**
- Send push notification to Director when unscheduled request requires approval
- Notify Director about pending approval
- Mark notification as handled

**Actors**
- Station Director (tablet / communicator)
2. Non-functional requirements

3. Entity relationship model
![ERD diagram](Spacedock_ERD.drawio.png)

4. --

5. Questions for the customer
