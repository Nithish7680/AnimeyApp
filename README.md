# Animey 🎌 — Discover Anime Characters, Powers & Dialogues

Animey is an ASP.NET Core Razor Pages Web App where users can explore anime series, their characters, famous dialogues, and special powers. It’s built as a fun yet technical portfolio project to demonstrate full-stack development using Razor Pages, EF Core, and a clean database design.

---

## 🚀 Features

- ✅ Browse list of anime on the homepage
- ✅ View characters of selected anime
- ✅ See character details: Image, Power, Favorite Dialogue
- ✅ Responsive UI (mobile + desktop)
- ✅ Admin panel to add/edit anime and characters (CRUD)
- ✅ Search and Filter characters
- ✅ Power Meter & Character Stats
- ✅ Built with Razor Pages & EF Core
- ✅ SQLite used for development (PostgreSQL/SQL Server-ready)
- ✅ Deployed using Render / Azure (TBD)

---

## 🧱 Tech Stack

- **Frontend**: Razor Pages (.cshtml), Bootstrap 5 / Tailwind
- **Backend**: ASP.NET Core 8 / 6 (Razor Pages)
- **Database**: Entity Framework Core + SQLite
- **Dev Tools**: Visual Studio / VS Code, Git, GitHub
- **Deployment**: Render / Azure App Service / Railway (TBD)

---

## 📦 Database Design

```mermaid
erDiagram
    Anime ||--o{ Character : contains
    Character {
        int Id
        string Name
        string ImageUrl
        string SpecialPower
        string FavoriteDialog
        int AnimeId
    }
    Anime {
        int Id
        string Title
        string CoverImageUrl
    }


---

## 📍 2. Visual Sitemap Wireframe

Here’s the structure of your app:

```text
/ (Home - All Anime)
  ├── /Anime/{animeId}           -> Characters List Page
  │     ├── Character Card       -> Click to open Character Details
  ├── /Character/{characterId}   -> Character Detail Page
  ├── /Admin/AddAnime            -> Add/Edit Anime Page
  ├── /Admin/AddCharacter        -> Add/Edit Character Page


## 📍 3. NugetPackage Manager

| Package                                | Purpose                                         |
| -------------------------------------- | ----------------------------------------------- |
| `Microsoft.EntityFrameworkCore`        | Core EF functionality (models, LINQ, DbContext) |
| `Microsoft.EntityFrameworkCore.Sqlite` | SQLite support                                  |
| `Microsoft.EntityFrameworkCore.Tools`  | Tools for migrations and CLI commands           |

