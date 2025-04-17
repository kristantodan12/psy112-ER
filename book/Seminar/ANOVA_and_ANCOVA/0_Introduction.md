---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# ANOVA and ANCOVA

In this first session of the practical part of the evaluation research seminar, we will cover the basics of analyzing data collected using various experimental designs. We will apply analysis of variance (ANOVA) and analysis of covariance (ANCOVA) models. You should already be familiar with these methods from your Bachelor studies. We recap the basic principles of these models in order to reinforce the foundation for understanding why these models are, in many cases, not appropriate for analyzing data collected in applied experimental research. We aim to summarize four types of models and this may be too much for the class. We will go slowly and the chapters we do not manage to cover will remain your homework. Please note that it is crucial to review these topics in order to be able to follow the new topics of the seminar. 

In general, the practical sessions will cover explanations, code examples and you will be required to complete brief exercises. We will go through the answers together.

Enjoy!

## Introduction Slide

::::{raw} html
<iframe src="../../../_static/Session1.pdf" width="100%" height="600px" style="border: none;">
    <p style="text-align: center;">Your browser does not support embedding PDFs.<br>
    <a href="../../../_static/Session1.pdf" target="_blank" rel="noopener noreferrer">Download the PDF instead</a>.</p>
</iframe>
::::

## Environment Setup

For this practical session (psy112), we will use the Conda environment you previously set up for the psy126 module as a base. You can find the original setup instructions for reference here:
[psy126 Setup Guide](https://leonardozaggia.github.io/psy126/book/introduction/1_psy126/1_Setup.html)

We need to install a few additional packages specifically for this course, which provide tools for advanced statistical analysis (like ANOVA/ANCOVA), data visualization, and formula handling.

**Steps:**

1.  **Open your Conda Terminal:**
    * _Windows:_ Anaconda Prompt or Anaconda Powershell
    * _macOS/Linux:_ Terminal

2.  **Activate your psy126 Environment:**
    *(Replace `psy126_env` below if you named your environment differently)*
    ```bash
    conda activate psy126_env
    ```
    Your terminal prompt should now show the environment name in parentheses, like `(psy126_env) C:\Users\...`.

3.  **Install Required Packages:**
    Run the following command using `pip` (the Python package installer) within your activated environment. This will install `seaborn` (for plotting), `pingouin` (for stats), `statsmodels` (for stats models/ANOVA), and `patsy` (for formulas):
    ```bash
    pip install seaborn pingouin statsmodels patsy
    ```
    Press Enter and wait for the packages and their dependencies to download and install.

4.  **Verify (Optional):**
    You can quickly check if a key package like `pingouin` is installed:
    * Start Python by typing `python` in your activated terminal.
    * At the `>>>` prompt, type `import pingouin`.
    * If no `ModuleNotFoundError` appears, it's installed correctly.
    * Exit Python by typing `exit()`.

Your environment is now updated and ready for the psy112 practical session.


