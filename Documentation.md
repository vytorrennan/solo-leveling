# Solo Leveling

## Description:

Quest/Habit Tracker with RPG elements, incluing XP points per completing Quests, Achivements and level up


## Core Features

- User Authentication (Sign Up / Login / Logout)
- Quest Management: Users create, complete, and delete quests
- Gamified Progress: Earn XP and level up as quests are completed
- Co-op Quests: Invite friends to join specific quests and work together
- Achievements: Unlock fun achievements for completing milestones
- Social Features: Comment on each other’s quests
- Charts for Progress Visualization: Display XP progress and level tracking

## Tech Stack

- Frontend: React + React Router + Axios + Recharts/Chart.js for progress tracking
- Backend: ASP.NET Core Web API + Entity Framework Core + SqlServer/SQLite
- Authentication: JWT-based login + OAuth (Google login)
- (Maybe) Real-Time Communication: WebSockets for live quest updates and friend interactions

## Entities

(Constants)
- NotificationType: id, name

(Data)
- Skillset: id, skillset, isDeleted
- Quests: id, title, description, rank, skillset, isCompleted, isDeleted
- User: id, email, username, password, xp, level, isDeleted
- Notifications: id, notificationTypeId, description, isNew, isDeleted

(Relationship Entities)
- UserQuests: userId, questId
- QuestSkillset: questId, skillsetId

## Extra Details

- Create static home page and serve it with react-snap for SEO
