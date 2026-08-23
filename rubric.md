# Climate Module: Detailed Rubric

Total: 20 points (of 29 available -- this allows multiple paths through the module)

## 1. Data Reading and Verification (**5 points**)

**5 points**: The notebook correctly reads in each data set and documents the reading
clearly. Sentinel and missing values are identified and handled deliberately, not
silently. Column meanings are checked against the source documentation rather than
assumed from their names. Where a data set is distributed across multiple files, all of
them are accounted for, or the subset used is named and justified.

## 2. Data Visualization (**5 points**)

**5 points**: The data analysis is thorough, appropriate for the data, and well-executed.
Plots are clear, well-labeled, and enhance understanding of the data. Figures are clearly
labeled with legends, titles and axes labels. Where two records of very different
resolution appear on shared axes, the figure does not imply a precision the data does not
have.

## 3. Code Quality and Tool Choice (**5 points**)

**5 points**: The code should be concise, semantically meaningful. The code does not
introduce additional libraries or methods not necessary for the task or beyond the scope
of basic data analysis methods covered in the course so far.

_Tool choice is part of code quality._ Where data exceeds what fits comfortably in memory,
the notebook uses a streaming approach (`ibis` on DuckDB) rather than loading everything
into RAM, and the student can say why. Reporting measured memory and timing to support
that choice earns full credit here; asserting it without measuring does not.

Avoid common LLM-based code-junk that does not follow best practices in data science notebooks:
  - Do not use `print` statements in code cells.  Cells should do one clear isolated task.  The final value on a cell is auto-printed by Jupyter without needing a `print` statement -- this should be used appropriately (e.g. to display small tables or plots).
  - Code should not include unnecessary error handling, such as `try` statements.  Use concise, working code for the data.
  - Code should not create function definitions unless they serve a clear use in making the code more concise and readable.
  - Do not include code comments in most cases.  Codes should be *self-documenting*, with clear variable names and structure.  Comments should be brief and only to clarify technical details.  Use markdown cells to explain the overall logic and flow of the notebook.
  - avoid long chunks of code that are not broken up into smaller, logical steps.  Each code cell should do one thing, and be clearly labeled with a markdown cell above it to explain what it does.

## 4. Verification and Scientific Judgment (**5 points**)

**5 points**: The student can answer the question _how do I know these numbers are right?_
for their own analysis.

  - The verification blocks are completed substantively, in the student's own words, not
    restated from the prompt.
  - Units are checked before quantities are combined. Values in different units are never
    summed.
  - Where a choice of variables changes the answer -- such as which CO2 stressors belong
    in a national total -- the choice is stated and defended on scientific grounds, not
    by pattern-matching on names.
  - At least one result is reconciled against an independent source, with the direction
    and size of any discrepancy quantified and explained rather than waved away.
  - Errors caught in model-generated code are documented. Finding and fixing a real bug
    is worth more here than producing a clean notebook that was never interrogated.

## 5. Narrative (**5 points**)

**5 points**: The notebook makes good use of markdown chunks to tell a clear story.
Instructor-provided headings like "exercise II" are replaced by topical headings like
"Global Temperature".  Data used and plots generated are clearly described ("the plot
shows...") to help a reader understand what they are seeing, where the data comes from,
key take-aways.  <https://climate.nasa.gov/vital-signs> is a great example of supporting
narrative describing the data and results, but tell the story in your own words.

Reflection responses are part of the narrative. An honest account of what the model got
wrong, and of what you contributed beyond accepting its output, is expected.

## 6. Use of GitHub (**4 points**)

**4 points**:

README file is updated with:
  - Authorship information
  - GitHub Actions badge, with correct link to repository
  - Updated description of repository overview.

Repository passes the auto-check on GitHub Actions.

Repository is clearly organized with logical filenames.

Clear, clean record of GitHub commits, appropriate git log messages.
Appropriate use of branches and pull requests if indicated by the instructor.

## Failure conditions

The notebook fabricates data, or presents fictious, made-up, or "example" numbers in
tables or charts as if they are real instead of reading data from the canonical data
sources indicated. (Automatic fail)

This applies without change to numbers produced by a language model. A model that cannot
parse a file will sometimes generate plausible values instead, occasionally announcing
that it has done so and occasionally not. Passing those numbers along as real is the same
failure whether you typed them or accepted them. Checking is your job, and it is the job
this module exists to teach.
