# Task Manager (Android + Supabase)

A production-style Android app demonstrating authentication, secure
user-scoped CRUD operations, and real-world backend integration using
Supabase.

------------------------------------------------------------------------

# MVP Scope

## Core Features

### Authentication

-   Email and password login
-   Persistent session
-   Logout functionality

### Task Management

-   View list of tasks
-   Create new task
-   Edit task
-   Delete task
-   Update task status (Todo / In Progress / Done)

### UX States

-   Loading indicators
-   Error handling
-   Empty state

------------------------------------------------------------------------

# Screens

1.  Login Screen
2.  Task List Screen
3.  Create Task Screen
4.  Edit Task Screen

------------------------------------------------------------------------

# Tech Stack

-   Kotlin
-   XML Layout
-   MVVM Architecture
-   Supabase Auth
-   Supabase Database (Postgres)
-   Coroutines
-   ViewModel
-   Repository Pattern

------------------------------------------------------------------------

# Architecture

    ui/
      LoginActivity
      TaskListActivity
      TaskAdapter

    viewmodel/
      AuthViewModel
      TaskViewModel

    repository/
      AuthRepository
      TaskRepository

    model/
      Task.kt

    network/
      SupabaseClient.kt

------------------------------------------------------------------------

# Database Schema

| column      | type      |
|-------------|-----------|
| id          | uuid      |
| user_id     | uuid      |
| title       | text      |
| description | text      |
| status      | text      |
| created_at  | timestamp |


Row Level Security Policy:

    user_id = auth.uid()

------------------------------------------------------------------------

# What This Project Demonstrates

-   Real backend integration
-   Authentication flow
-   Secure user-specific data access
-   Proper Android architecture
-   Error handling and async programming

------------------------------------------------------------------------

# Setup

1.  Clone repository
2.  Create Supabase project
3.  Add keys to local.properties:

```{=html}
SUPABASE_URL=your_url
SUPABASE_ANON_KEY=your_key
```

4.  Run project

------------------------------------------------------------------------

# Future Improvements

-   Offline support (Room)
-   Pagination
-   Unit testing
-   UI testing
-   Compose version

------------------------------------------------------------------------

# Author

Tanakorn Arttajin\
Android Developer Portfolio Project for Upwork
