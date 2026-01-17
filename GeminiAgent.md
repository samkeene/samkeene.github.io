# Gemini Agent Context for Jekyll Site

This document defines the standards and workflows for the Gemini AI agent when assisting with this Jekyll-based static website.

## 1. Role & Responsibilities
- **Primary Goal:** Assist the user in generating, editing, and managing content (posts, pages, data) for the Jekyll site.
- **Secondary Goal:** Maintain repository hygiene through standardized Git practices.

## 2. Content Creation Standards
When asked to write a new post or content:
1.  **Front Matter:** Use YAML format. Ensure fields like `layout`, `title`, and `date` are present.
2.  **File Naming:** Posts MUST follow the `YEAR-MONTH-DAY-title.md` format (e.g., `_posts/2026-01-10-welcome.md`).
3.  **Directory Structure:** 
    - Posts go in `_posts/`.
    - Drafts go in `_drafts/`.
    - Pages (e.g., `about.md`) go in the root or specific subdirectories.

## 3. Jekyll Command Reference
Use these commands to manage the site lifecycle.

| Command | Usage Scenario |
| :--- | :--- |
| `bundle exec jekyll serve` | Start a local development server. |
| `bundle exec jekyll serve --drafts` | Start server and include content from the `_drafts/` folder. |
| `bundle exec jekyll build` | Build the static site to the `_site/` directory. |
| `bundle exec jekyll doctor` | Check for configuration or deprecation issues. |

## 4. Git Workflow & Standards

### Commit Messages
Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:
- `feat: ...` for new content or features.
- `fix: ...` for corrections.
- `docs: ...` for documentation changes.
- `chore: ...` for maintenance tasks.

**Example:** `feat(blog): add post about Jekyll migration`

### Workflow
1.  **Pull First:** Always ensure local state is up to date.
2.  **Atomic Commits:** Separate content additions from configuration or theme changes.
3.  **Push:** Push changes to the `main` branch after verifying the build.

## 5. Interaction Guidelines

- Check `_config.yml` to understand site-wide variables and plugin requirements.

- **Exclusion:** Ensure `GEMINI.md` is added to the `exclude` list in `_config.yml` to prevent it from being built into the static site.

- Ensure all dependencies are handled via `Bundler` (`Gemfile`).



## 6. Environment & Dependency Management



### Ruby Version

- Use a `.ruby-version` file to specify the required Ruby version for the project.

- While `Bundler` can enforce a version in the `Gemfile`, a version manager (like `rbenv` or `rvm`) is needed to switch Ruby versions.



### Bundler (Gemfile)

- Always use `bundle exec` before Jekyll commands to ensure the project-specific gem versions are used.

- Run `bundle install` after modifying the `Gemfile`.

- Commit the `Gemfile.lock` to ensure environment parity across different machines.