# Group Website Contributor Guide

This guide walks you through adding your personal profile, publications, and blog posts to our group website.

## 1. Add Your Personal Information

Each member has a profile under `content/authors/`. To create yours:

### Step 1: Create your author directory

Create a new folder under `content/authors/` using your first name (lowercase) as the identifier. For example:

```
content/authors/yourname/
```

### Step 2: Add your profile photo

Place a photo named **`avatar.jpg`** inside your folder:

```
content/authors/yourname/avatar.jpg
```

### Step 3: Create `_index.md`

Create a file `content/authors/yourname/_index.md` with the following template:

```yaml
---
title: Your Full Name

first_name: YourFirst
last_name: YourLast

superuser: false

role: PhD Student  # or "Master Student", "Postdoc", etc.

organizations:
  - name: 
    url: 

bio: A short one-line bio about your research.

interests:
  - Interest One
  - Interest Two
  - Interest Three

education:
  courses:
    - course: MSc in Computer Science
      institution: Your University
      year: 2024
    - course: BSc in Some Major
      institution: Your University
      year: 2021

social:
  - icon: envelope
    icon_pack: fas
    link: 'mailto:you@example.com'
  - icon: google-scholar
    icon_pack: ai
    link: https://scholar.google.com/citations?user=YOURID
  - icon: github
    icon_pack: fab
    link: https://github.com/yourusername

email: 'you@example.com'

highlight_name: false

user_groups:
  - Students  # Options: "Faculty", "Students", "Alumni"
---

Write a short paragraph about yourself here. This appears on your profile page.
```

### Key notes

- **`user_groups`** controls where you appear on the People page. Use `Faculty`, `Students`, or `Alumni`.
- **`superuser: false`** — only the site owner sets this to `true`.
- **Author identifier** (your folder name) is what you'll use when listing yourself as an author in publications and posts.

---

## 2. Add a New Publication

Publications live under `content/publication/`. Each publication is a folder containing an `index.md` file.

### Step 1: Create the publication folder

Use the naming convention: **`{lastname}-{year}-{keyword}`**

```
content/publication/wang-2026-mymethod/
```

### Step 2: Create `index.md`

Pick the template that matches your publication type:

#### Journal Article

```yaml
---
title: "Your Paper Title"
authors:
  - yourname
  - Second Author
  - panpan
date: "2026-01-15"
publishDate: "2026-01-15T00:00:00Z"
publication_types:
  - article-journal
publication: "*IEEE Robotics and Automation Letters (RA-L)*"
url_pdf: "https://arxiv.org/abs/XXXX.XXXXX"
url_code: "https://github.com/your/repo"
url_project: "https://your-project-page.github.io/"
---
```

#### Conference Paper

```yaml
---
title: "Your Paper Title"
authors:
  - yourname
  - panpan
date: "2026-06-01"
publishDate: "2026-06-01T00:00:00Z"
publication_types:
  - paper-conference
publication: "IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)"
url_pdf: "https://arxiv.org/abs/XXXX.XXXXX"
---
```

#### Preprint

```yaml
---
title: "Your Paper Title"
authors:
  - yourname
  - panpan
date: "2026-03-01"
publishDate: "2026-03-01T00:00:00Z"
publication_types:
  - article
publication: "*arXiv preprint arXiv:XXXX.XXXXX*"
url_pdf: "https://arxiv.org/abs/XXXX.XXXXX"
---
```

### Optional: Add a featured image

Place an image named **`featured.png`** (or `featured.jpg`) in the publication folder to display a thumbnail.

### Key notes

- **Author names**: Use the author folder name (e.g., `yourname`, `panpan`) for group members. For external co-authors, write their full name directly (e.g., `Cewu Lu`).
- **`publication_types`** determines how the paper is categorized in the filter. Valid values:
  - `article-journal` → shows as "Journal article"
  - `paper-conference` → shows as "Conference paper"
  - `article` → shows as "Preprint"
- **`url_pdf`**, **`url_code`**, **`url_project`**, **`url_video`** are all optional — include whichever links are available.

---

## 3. Make a Post

Blog posts live under `content/post/`. Each post is a folder containing an `index.md` file.

### Step 1: Create the post folder

Use the naming convention: **`{YY}-{MM}-{DD}-{slug}`**

```
content/post/26-04-20-my-new-post/
```

### Step 2: Create `index.md`

```yaml
---
title: "Your Post Title"
date: 2026-04-20
authors:
  - yourname
  - panpan
---

Write your opening paragraph here. This part appears as the preview/summary on the post listing page.

<!--more-->

## Section Heading

Everything below `<!--more-->` only appears when the reader clicks into the full post.

You can use standard Markdown:

- **Bold text** and *italic text*
- [Links](https://example.com)
- Images: `![Alt text](image.jpg)`

### Embedding Videos

To embed a Bilibili video:

<div style="max-width:100%; margin:0 auto;">
  <iframe src="https://www.bilibili.com/video/BVXXXXXXXXX" width="100%" height="498" scrolling="no" frameborder="0" allowfullscreen="true"></iframe>
</div>
```

### Key notes

- **`<!--more-->`** splits the summary from the full content. Everything above it shows on the listing page.
- **`authors`** uses the same identifiers as publications — your folder name under `content/authors/`.
- Add `draft: true` to the frontmatter if you're not ready to publish yet.

---

## Quick Reference

| Content       | Location                          | Naming Convention                  | Key File     |
|---------------|-----------------------------------|------------------------------------|--------------|
| Profile       | `content/authors/{name}/`         | lowercase first name               | `_index.md`  |
| Publication   | `content/publication/{name}-{yr}-{kw}/` | `lastname-year-keyword`      | `index.md`   |
| Post          | `content/post/{YY}-{MM}-{DD}-{slug}/`  | `yy-mm-dd-short-description` | `index.md`   |

## Building and Previewing

```bash
# Preview locally
hugo server

# Build for production
hugo
```

After making changes, commit and push to the repository. The site will be rebuilt automatically.
