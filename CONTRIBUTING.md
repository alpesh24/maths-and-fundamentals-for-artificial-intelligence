# Contributing

This repository is organized as a structured curriculum for mathematics, computer science, machine learning, and vision foundations. Contributions should keep the subject map, documentation, and resource metadata consistent.

## What You Can Contribute

- new subject notes or improvements to existing area pages
- better course, literature, and resource links
- metadata updates in `data/resources.yaml`
- diagrams, roadmap visuals, and supporting documentation
- fixes to naming, structure, and cross-links

## Repository Rules

- Keep subject documentation inside `areas/<domain>/<subject>/README.md`.
- Keep shared metadata in `data/resources.yaml`.
- Keep diagrams and images in `assets/`.
- Keep local PDF books in `books/`.
- Do not commit copyrighted PDFs unless you have the right to redistribute them.

## Folder Structure

- `areas/` contains domain pages and subject pages
- `data/resources.yaml` is the source of truth for subjects, links, and local books
- `assets/graphs/` stores subject maps and diagrams
- `books/` mirrors the subject taxonomy for local-only materials

## How To Add A New Resource

1. Update the correct subject entry in `data/resources.yaml`.
2. Add the resource under one of:
   - `resources.courses`
   - `resources.literature`
   - `resources.other_resources`
3. If the subject page should show the new link, update that subject `README.md`.
4. Keep labels clear and stable.

## How To Add A Local Book

1. Place the file in the matching `books/<domain>/<subject>/` folder.
2. Add a matching entry under `local_books` in `data/resources.yaml`.
3. Use the real file name in `file_name`.
4. Use a repo-relative path in `path`.

## How To Add A New Subject

1. Create the subject folder under the correct domain in `areas/`.
2. Add a `README.md` for that subject.
3. Create the matching folder in `books/`.
4. Add the subject entry to `data/resources.yaml`.
5. Link the subject from the domain `README.md`.
6. Update the root [README.md](README.md) if the top-level index changes.

## Writing Guidelines

- Use consistent English naming for subjects and slugs.
- Prefer short, clear explanations over long prose.
- Keep prerequisite and downstream links accurate.
- Use relative paths inside the repository.
- Keep Markdown tables simple and easy to scan.

## Before You Open A PR

- check that links you added are valid
- confirm paths in `data/resources.yaml` match real files and folders
- confirm new subjects appear in the right domain
- avoid duplicate resources unless there is a strong reason
- keep unrelated formatting changes out of the same contribution

## Recommended Workflow

1. Update `data/resources.yaml` first.
2. Update the relevant `areas/.../README.md` files.
3. Update the root `README.md` only if navigation or taxonomy changed.
4. Add or update files in `assets/` if the graph or visuals changed.

## Notes On Books

- `books/` is intended for local organization.
- Public contributions should prefer metadata and official links over uploading copyrighted files.
- If a book is local-only, still record it in `data/resources.yaml` so the catalog stays complete.
