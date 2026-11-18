# Publication-Ready Figure Generation in R

A hands-on 2 half-day course covering effective data visualization principles and practical techniques for creating publication-ready figures in R.
Designed for researchers at the Comprehensive Cancer Center Zurich (CCCZ), University Hospital Zurich (USZ), and University of Zurich (UZH).

## Acknowledgements

| | |
|---|---|
| <img src="assets/images/krauthammer.jpg" width="150" style="vertical-align: middle;"> | <img src="assets/images/cccz.jpg" width="350" style="vertical-align: middle;"> |
| We thank [Prof. Michael Krauthammer](https://krauthammerlab.ch/authors/michaelkrauthammer/) for supporting this course. | Special thanks to **CCCZ** — Dr. Maja Zenz and Ms. Silke Uflacker — for providing coffee breaks. |

---

**Instructor:** Deepak Tanwar — [deepak.tanwar@uzh.ch](mailto:deepak.tanwar@uzh.ch)

---

## Course Format

| | |
|---|---|
| **Format** | 2 half-day intensive workshop |
| **Duration** | 4 hours per half-day (8 hours total) |
| **Audience** | Researchers with basic R programming skills |
| **Prerequisites** | See [setup.md](setup.md) — complete before the course |

---

## Learning Objectives

- **Analyze the principles of effective data visualization:**
  - **Explain** the importance of clarity, accuracy, and aesthetics in creating publication-ready figures.
  - **Identify** common pitfalls in data visualization and how to avoid them.

- **Apply base R graphics for figure creation:**
  - **Create** basic plots (e.g., scatterplots, bar charts, histograms) using base R functions like `plot()`, `barplot()`, and `hist()`.
  - **Customize** plots with titles, labels, legends, and color schemes.

- **Construct advanced visualizations using ggplot2:**
  - **Build** complex and layered visualizations using the `ggplot2` package.
  - **Apply** themes, scales, and `geoms` to create polished and publication-ready figures.

- **Adapt figures for specific publication requirements:**
  - **Adjust** figure dimensions, resolutions, and formats (e.g., PDF, PNG, TIFF) for journal submissions.
  - **Modify** fonts, line weights, and other stylistic elements to meet publication guidelines.

- **Integrate statistical annotations and summaries:**
  - **Add** statistical summaries (e.g., regression lines, confidence intervals) to figures.
  - **Annotate** plots with p-values, correlation coefficients, or other relevant statistics.

- **Generate high-quality figures:**
  - **Use** functions like `ggsave()` or `pdf()` to export figures in high resolution.
  - **Ensure** exported figures meet the technical requirements of target journals or platforms.

- **Assemble multi-panel figures:**
  - **Combine** multiple plots into a single figure using tools like `patchwork`.
  - **Align** and **arrange** subplots to effectively communicate complex data.

- **Implement best practices for reproducibility:**
  - **Write** clean and reusable R scripts for figure generation.
  - **Document** code and workflows to ensure reproducibility and transparency.

---

## Course Schedule

### **Morning (Half-Day 1) — 09:00–12:00**

| Time | Session | Topics | Exercises |
|------|---------|--------|-----------|
| 09:00–09:15 | Welcome | Introductions, course overview, visualization principles | — |
| 09:15–10:15 | **Block 1:** Visualization Principles | Why figures matter, clarity vs. complexity, common mistakes, effective storytelling | [Ex 1](exercises/exercise_block_1.qmd) |
| 10:15–10:30 | *Break* | ☕ Coffee break | — |
| 10:30–11:15 | **Block 2:** Base R Graphics | `plot()`, `barplot()`, `hist()`, customization basics, legends & labels | [Ex 2](exercises/exercise_block_2.qmd) |
| 11:15–12:00 | **Block 3:** ggplot2 Fundamentals | Layers, aesthetics, `geoms`, basic plots, understanding the grammar of graphics | [Ex 3](exercises/exercise_block_3.qmd) |

**What You'll Learn (Morning):**
- Core visualization principles for scientific communication
- Introduction to base R and ggplot2 syntax
- Creating your first publication-ready plots

---

### **Afternoon (Half-Day 2) — 13:00–17:00**

| Time | Session | Topics | Exercises |
|------|---------|--------|-----------|
| 13:00–14:00 | **Block 4:** Styling & Themes | Scales, themes, annotations, legends, color palettes, visual hierarchy | [Ex 4](exercises/exercise_block_4.qmd) |
| 14:00–14:15 | *Break* | ☕ Coffee break | — |
| 14:15–15:15 | **Block 5:** Publication Standards | Figure formats, resolution, dimensions, DPI, journal requirements, exporting with `ggsave()` | [Ex 5](exercises/exercise_block_5.qmd) |
| 15:15–16:00 | **Block 6:** Multi-panel Figures | `patchwork`, layout design, alignment, combined plots with shared legends | [Ex 6](exercises/exercise_block_6.qmd) |
| 16:00–16:15 | *Break* | ☕ Final break | — |
| 16:15–17:00 | **Block 7** + **Final Project** | Advanced topics (faceting, statistical overlays), create publication-ready figures from provided data | [Ex 7](exercises/exercise_block_7.qmd) |

**What You'll Learn (Afternoon):**
- Professional styling and publication-compliant formatting
- Multi-panel figure assembly with patchwork
- Advanced visualization techniques
- Complete workflow for publication-ready figures

---

## Project Structure

This project is structured as follows:

```
publication_ready_figs_R/
├── README.md                          # This file
├── CONTRIBUTING.md                    # Contribution guidelines
├── setup.md                           # Pre-course setup instructions
├── LICENSE                            # MIT License
├── _quarto.yml                        # Quarto configuration
├── index.qmd                          # Course homepage
├── styles.css                         # Custom website styling
│
├── qmd/                               # Course content
│   ├── precourse_preparation.qmd     # Prerequisites & skill assessment
│   └── schedule.qmd                   # Detailed course schedule
│
├── slides/                            # Presentation slides (Blocks 1-7)
│   ├── slide_block_1.qmd             # Visualization Principles
│   ├── slide_block_2.qmd             # Base R Graphics
│   ├── slide_block_3.qmd             # ggplot2 Fundamentals
│   ├── slide_block_4.qmd             # Styling & Themes
│   ├── slide_block_5.qmd             # Publication Standards
│   ├── slide_block_6.qmd             # Multi-panel Figures
│   └── slide_block_7.qmd             # Advanced Topics
│
├── exercises/                         # Hands-on exercises (Blocks 1-7)
│   ├── exercise_block_1.qmd
│   ├── exercise_block_2.qmd
│   ├── exercise_block_3.qmd
│   ├── exercise_block_4.qmd
│   ├── exercise_block_5.qmd
│   ├── exercise_block_6.qmd
│   └── exercise_block_7.qmd
│
├── assets/
│   ├── images/                       # Logos and images
│   │   ├── krauthammer.jpg          # Prof. Krauthammer
│   │   └── cccz.jpg                 # CCCZ logo
│   ├── data/                         # Sample datasets for exercises
│   ├── figs/                         # Course illustrations & examples
│   └── ggplot2/                      # ggplot2-related resources
│
├── docs/                              # Rendered website (auto-generated)
└── renv/                              # Reproducible R environment
```

---

## Prerequisites

**Basic R Programming Skills:**
- Understanding R syntax (objects, functions, operators)
- Ability to create and manipulate basic data structures: vectors, factors, data frames, and lists
- Familiarity with indexing and subsetting data
- Writing simple scripts in RStudio or another R IDE
- Reading and importing data (`read.csv()`, `read.table()`, or `readr`)

**Skill Self-Assessment:**
Unsure if you're ready? Evaluate your R skills:
- [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSdIyeuabd_ZOWXgI1MWHapmaOMu20L9ESkLDZiWnpmkpujyOg/viewform)
- [Coursera R Programming Skill Assessment](https://www.coursera.org/resources/r-programming-skill-assessment)
- [NCEAS R Review and Assessment](https://nceas.github.io/oss-lessons/r-review-and-assessment/r-review-and-assessment.html)

---

## Computational Requirements

- **R** 4.5.1 or later
- **RStudio** (latest version recommended)
- **Quarto** (for rendering course materials)
- **renv** R package installed for reproducible environments
  - See: [renv documentation](https://rstudio.github.io/renv/articles/renv.html)

**Key R packages used in this course:**
- `ggplot2` – Advanced visualization
- `patchwork` – Multi-panel figure assembly
- `tidyverse` – Data manipulation and visualization

---

## Build & Access Instructions

### **View the Course Online**
👉 **[https://dqbm-cccz.github.io/publication_ready_figs_R/](https://dqbm-cccz.github.io/publication_ready_figs_R/)**

Access slides, exercises, and all course materials from the website.

### **Build Locally**

1. **Install Quarto:**
   - Follow the instructions on the [Quarto website](https://quarto.org/docs/get-started/)

2. **Clone the repository:**
   ```bash
   git clone https://github.com/DQBM-CCCZ/publication_ready_figs_R.git
   cd publication_ready_figs_R
   ```

3. **Restore the R environment** (highly recommended):
   ```r
   renv::restore()
   ```

4. **Render the website:**
   ```bash
   quarto render
   ```
   This generates the `docs/` directory with the complete website.

5. **Preview locally:**
   - Open `docs/index.html` in your web browser

---

## Contributing

Contributions are welcome! Whether you're:
- Fixing bugs or typos
- Suggesting improvements to exercises
- Proposing new content
- Sharing resources

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

This course website is inspired by the [SIB course template](https://github.com/sib-swiss/course_website_template).

**Course Delivery:** 2025  
**Instructor:** Deepak Tanwar  
**Institution:** Comprehensive Cancer Center Zurich (CCCZ)  
**Copyright © 2025**
