# TechConnect Flask Marketplace


## Current workflow
- Users and profiles
- Jobs and applications
- Accepted applications create contracts
- Contracts contain milestones, dynamic tasks and deliverables
- Professional milestone payments are released after approved/completed milestones
- TechConnect platform fee is 10% of the completed contract and is settled only at final contract completion
- Messaging is available between contract parties
- Disputes can be opened against a milestone or the whole contract
- Open disputes pause affected milestone payment release and block final contract completion
- Client can review deliverables and request revisions

## Payment model
Milestone payments are released to the professional without deducting the TechConnect 10% fee. The platform fee is calculated against the whole contract at final settlement.

## Run
```bash
python3 app.py
```

The database remains `vibelink.db` for backward compatibility with existing user data.


## Administrator panel

The project includes a protected administrator area:
- `/admin/login` — administrator sign-in
- `/admin` — overview dashboard
- `/admin/users` — user access management
- `/admin/projects` — marketplace project monitoring
- `/admin/contracts` — contract and payment oversight
- `/admin/disputes` — dispute resolution center
- `/admin/audit` — administrative audit log

Create the first admin from the project directory with:

```bash
python3 create_admin.py admin@example.com
```
