# Setup Instructions

Please complete all setup steps **before the course starts** to ensure you're ready on day one.

## Prerequisites

### Basic R Programming Skills

You should be comfortable with the following before taking this course:

- Understanding R syntax (objects, functions, operators)
- Ability to create and manipulate basic data structures: vectors, factors, data frames, and lists
- Familiarity with indexing and subsetting data
- Writing simple scripts in RStudio or another R IDE
- Reading and importing data (`read.csv()`, `read.table()`, or `readr`)

### Skill Self-Assessment

Unsure if you're ready? Evaluate your R skills using one of these resources:

- [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSdIyeuabd_ZOWXgI1MWHapmaOMu20L9ESkLDZiWnpmkpujyOg/viewform)
- [Coursera R Programming Skill Assessment](https://www.coursera.org/resources/r-programming-skill-assessment)
- [NCEAS R Review and Assessment](https://nceas.github.io/oss-lessons/r-review-and-assessment/r-review-and-assessment.html)

If you're not comfortable with the fundamentals, consider taking an introductory R course first.

---

## Computational Requirements

You'll need the following software installed on your computer:

| Software | Version | Purpose |
|----------|---------|---------|
| **R** | 4.5.1 or later | Statistical computing and graphics |
| **RStudio** | Latest version | Integrated Development Environment (IDE) for R |
| **renv** | (R package) | Manages reproducible R environments |

---

## Installation Guide

### 1. Install R

**On macOS:**
```bash
# Using Homebrew (recommended)
brew install r

# Or download from CRAN
# https://cran.r-project.org/bin/macosx/
```

**On Windows:**
- Download the installer from [CRAN](https://cran.r-project.org/bin/windows/base/)
- Run the installer and follow the prompts

**On Linux (Ubuntu/Debian):**
```bash
sudo apt-get update
sudo apt-get install r-base r-base-dev
```

**Verify installation:**
```r
# In R console
R.version$version.string
```

### 2. Install RStudio

1. Download from [https://www.rstudio.com/products/rstudio/download/](https://www.rstudio.com/products/rstudio/download/)
2. Choose the free RStudio Desktop version
3. Install following the platform-specific instructions
4. Launch RStudio

### 3. Install renv (R Package)

Open RStudio and run the following in the R console:

```r
install.packages("renv")
```

This package helps manage consistent R environments across projects and collaborators.

### 4. Clone the Course Repository

```bash
git clone https://github.com/DQBM-CCCZ/publication_ready_figs_R.git
cd publication_ready_figs_R
```

### 5. Restore the Course Environment

Open RStudio with the `publication_ready_figs_R.Rproj` file, then run:

```r
renv::restore()
```

This will install all required R packages in the exact versions we use for this course.

---

## Verify Your Setup

To confirm everything is working, run this in RStudio:

```r
# Check R version
R.version$version.string

# Check renv is installed
library(renv)

# Load key packages we'll use
library(ggplot2)
library(patchwork)
library(tidyverse)

# Create a simple plot to verify graphics
plot(mtcars$mpg ~ mtcars$hp)
```

You should see:
- R version 4.5.1 or later
- All packages load without errors
- A scatter plot appears

---

## Troubleshooting

### "Command not found: git"
Install Git from [https://git-scm.com/downloads](https://git-scm.com/downloads)

### "renv::restore() fails with package installation errors"
1. Update all packages: `update.packages()`
2. Try again: `renv::restore()`
3. If issues persist, contact the instructor at [deepak.tanwar@uzh.ch](mailto:deepak.tanwar@uzh.ch)

### "RStudio won't open the project"
- Ensure you're opening the `.Rproj` file, not individual scripts
- Restart RStudio if needed

### "Graphics not displaying"
- Check that you have X11 (macOS) or appropriate graphics drivers (Linux)
- Restart RStudio

---

## Getting Help

If you encounter issues during setup:

1. **Check the troubleshooting section above**
2. **Search for the error message online** — most issues have documented solutions
3. **Contact the instructor:** [deepak.tanwar@uzh.ch](mailto:deepak.tanwar@uzh.ch)

Please reach out early so we can help you get ready for the course!

---

## Optional: Advanced Setup

If you're comfortable with version control and want to contribute to the course materials:

```bash
# Fork the repository on GitHub first, then:
git clone https://github.com/YOUR-USERNAME/publication_ready_figs_R.git
cd publication_ready_figs_R
git remote add upstream https://github.com/DQBM-CCCZ/publication_ready_figs_R.git
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for details on submitting improvements.
