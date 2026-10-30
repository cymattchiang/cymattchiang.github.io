# Chung-Yen (Matt) Chiang

Source for the personal academic website at https://cymattchiang.github.io/.
Static HTML, CSS, and JavaScript; no build step or package dependencies.

## Files

| Path | Purpose |
| --- | --- |
| `index.html` | Website content, styles, and navigation |
| `cv/academic.pdf` | Academic CV linked from the introduction and Experience heading |
| `cv/software-industry.pdf` | Software engineering resume linked from the Amazon entry |
| `resume-cv.pdf` | Compatibility copy of the academic CV for the existing public URL |
| `thesis/` | Paper and research summaries linked from the website or CVs |
| `profile.jpg` | Website portrait |
| `favicon.svg` | Website icon |

The academic CV is the primary document. The industry resume is available beside the relevant professional experience.

## Update the CVs

1. Export the new PDF to the appropriate file in `cv/`.
2. When updating the academic CV, also refresh its compatibility copy:

   ```sh
   cp cv/academic.pdf resume-cv.pdf
   ```

3. Preview the site and open both PDF links before committing.

LaTeX sources are maintained separately. Only website assets belong in this repository; keep source archives, backups, and compiler output outside it.

## Local preview

From the repository root:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://127.0.0.1:8000/ in a browser. Deployment follows the repository's GitHub Pages configuration.

## Housekeeping

`.gitignore` excludes macOS metadata and local scratch files. Unused attachments and the legacy CV backup have been archived outside this repository.
