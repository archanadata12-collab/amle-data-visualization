# Data Visualisation with Python

A hands-on module on data visualisation in Python with Matplotlib, Seaborn, and Plotly. In the first part you learn when to use an exploratory or an explanatory chart, tour the three libraries on the Palmer Penguins dataset, and build a stakeholder-ready set of plots from the 2020 Kaggle Data Science Survey. In the second part you work in a small group and recreate the same charts in all three libraries, using Seattle weather and US airport data.

## Learning Objectives

By the end of this repository, you should be able to:

- Create scatter, line, bar, and distribution charts with Matplotlib, Seaborn, and Plotly.
- Choose between an exploratory and an explanatory chart for a given audience.
- Choose the right chart type for a given data type and question.
- Prepare a survey dataset by filtering, aggregating, and reshaping it, and build charts that answer specific stakeholder questions.
- Apply the elements of a good plot to every figure: a clear title, axis labels with units, and a readable legend.
- Build an interactive map of point data with Plotly.

## Learning Path

Work through the modules in this order.

### 1 - Basics

The two purposes of visualisation, a tour of the three libraries, and the main exercise.

| File | Description |
| --- | --- |
| [**01 - Exploratory vs Explanatory Visualisation**](1_basics/01_exploratory_vs_explanatory.md) | Reading on the two purposes of visualisation and the explore, refine, polish workflow. |
| [**02 - Introduction to Data Visualisation**](1_basics/02_plotting_intro.ipynb) | A tour of Matplotlib, Seaborn, and Plotly across many chart types, with checkpoints, on the Palmer Penguins dataset. |
| [**03 - Exercise: Kaggle Data Science Survey 2020**](1_basics/03_exercise_kaggle_survey.ipynb) | The main exercise: answer stakeholder questions about the 2020 Kaggle survey with at least one plot from each library. |
| [**04 - Chart Gallery**](1_basics/04_chart_gallery.ipynb) | A worked gallery from minimal to publication-styled charts in all three libraries, with a clickable table of contents. |

### 2 - Group Work

Recreate the same charts in several libraries and compare the results. Start with the task file to find your group's chart and dataset, then build your plots in the template notebook.

| File | Description |
| --- | --- |
| [**01 - Task**](2_group_work/01_task.md) | The brief: group assignments, datasets, and what makes a plot good. |
| [**02 - Exercise: Group Work Template**](2_group_work/02_exercise_template.ipynb) | Starter notebook with one section per library (Matplotlib, Seaborn, Plotly) for your group's plots. |

### Additional Folders and Files

| File / Folder | Description |
| --- | --- |
| [**Data**](data/) | Datasets for both modules: Palmer Penguins and the 2020 Kaggle survey for module 1, Seattle weather and US airports for module 2. |
| [**Docs**](docs/) | The 2020 Kaggle survey methodology and answer choices, for reading the survey questions. |
| [**Assets**](assets/) | Images used in the lessons and the example plot from the group-work brief. |
| [**Solutions**](solutions/) | Worked solutions to the two exercises. |
| [**pyproject.toml**](pyproject.toml) | Project configuration and dependencies. |
| [**uv.lock**](uv.lock) | Dependency lock file. |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a **placeholder**. Replace it, including the `< >` brackets, with your own value. For example, `cd <repo-name>` becomes `cd my-data-visualisation`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> Module 2 is group work. If you are working in a group, only **one person** should complete this step, then add the others as collaborators in the next step.

---

### 2. Add Collaborators (Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

Teammates should accept the invitation before continuing.

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like `git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder and Install Dependencies

This installs all dependencies and creates a virtual environment in `.venv/`.

```bash
cd <repo-name>
uv sync
```

---

### 5. Open the Notebooks

> [!NOTE]
> Open VS Code from the project root so it automatically detects the environment created by `uv sync`.

Launch VS Code in the project root:

```bash
code .
```

Then open a notebook and select the Python environment created by `uv sync` as the kernel.

## References & Further Reading

- [**Matplotlib tutorials**](https://matplotlib.org/stable/tutorials/index.html): Official guides from the basics to advanced plotting.
- [**Seaborn user guide and tutorial**](https://seaborn.pydata.org/tutorial.html): The official Seaborn tutorial covering statistical plots and styling.
- [**Plotly Python Graphing Library**](https://plotly.com/python/): Official documentation for Plotly's interactive charts.
- [**Plotly scatter plots on maps**](https://plotly.com/python/scatter-plots-on-maps/): Official guide to the geographical maps used in the group work.
- [**From Data to Viz**](https://www.data-to-viz.com/): A decision tree for picking the right chart type, with common caveats to avoid.
- [**The Python Graph Gallery**](https://python-graph-gallery.com/): Hundreds of reproducible chart examples in Matplotlib, Seaborn, and Plotly.
- [**Fundamentals of Data Visualization**](https://clauswilke.com/dataviz/): A free online book by Claus Wilke on making figures that are clear and honest.
- [**Storytelling with Data**](https://www.storytellingwithdata.com/): Practical guidance and worked makeovers for turning exploratory charts into explanatory ones.
- [**Jupyter Notebooks in VS Code**](https://code.visualstudio.com/docs/datascience/jupyter-notebooks): How to run and debug notebooks inside VS Code.
