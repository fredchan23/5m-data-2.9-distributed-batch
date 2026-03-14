# 2.9 Distributed Batch Processing and Transformation

## Dependencies

Refer to the following markdown file for the respective sections of the class:

- [Pre-Class](./pre-class.md)
- [Lesson](./lesson.md)
- [Assignment](./assignment/assignment.md)
- [Reference](./reference.md)

## Python Environment Setup

This repository includes a frozen Conda environment file at [spark.yml](./spark.yml). New users should create and activate this environment before running any Python scripts or notebooks in this repo.

Create the environment:

```bash
conda env create -f spark.yml
```

Activate it:

```bash
conda activate spark
```

Run Python code from this environment:

```bash
python your_script.py
```

For notebooks, start Jupyter from the same activated environment so PySpark, pandas, and the other pinned packages come from `spark`:

```bash
jupyter notebook
```

If you are using VS Code, select the `spark` interpreter or kernel before running notebook cells or Python files.

## Dataset Setup

The analysis notebook [notebook/oist_spark_analysis.ipynb](./notebook/oist_spark_analysis.ipynb) depends on the Olist Brazilian E-Commerce CSV dataset, which should not be committed to this repository.

Before running that notebook, download the dataset from Kaggle and place the required CSV files under `notebook/oist-data/`.

See [notebook/oist-data/README.md](./notebook/oist-data/README.md) for the download link and the exact filenames expected by the notebook.

## Lesson Objectives

Learners will understand:

- Big data ecosystem and the evolution of data processing on distributed architectures
  - Hadoop Distributed File System (HDFS)
  - MapReduce
  - Spark

Learners will be able to:

- Use Spark to process data in a distributed batch manner

## Lesson Plan

| Duration | What                    | How or Why                                               |
| -------- | ----------------------- | -------------------------------------------------------- |
| - 5mins  | Start zoom session      | So that learners can join early and start class on time. |
| 20 mins  | Activity                | Recap on self-study and prework materials.               |
| 40 mins  | Concept                 | Part 1 - Big Data Ecosystem and Batch Processing.        |
|          | **1 HR MARK**           |
| 30 mins  | Code-along              | Part 2: Hands-on with Spark (DataFrames).                |
| 10 mins  | Break                   |                                                          |
| 20 mins  | Code-along              | Part 2: Hands-on with Spark (DataFrames).                |
|          | **2 HR MARK**           |
| 50 mins  | Code-along              | Part 2: Hands-on with Spark (SQL and Pandas API).        |
| 10 mins  | Briefing / Q&A          | Brief on references, assignment, quiz and Q&A.           |
|          | **END CLASS 3 HR MARK** |
