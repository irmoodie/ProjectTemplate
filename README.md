# ProjectTemplate
 📊 A project template for reproducible manuscripts, primarily using R (with the targets package) and Quarto.

## 1. How to download this repository

You can download this repository in several ways:

1. **Download as ZIP**: Click the "Code" button at the top of the repository page and select "Download ZIP". Extract the contents to your desired location.
2. **Download from Releases**: Navigate to the "Releases" section on the repository page and download the latest release package.
3. **Fork the Repository**: If you are familiar with Git, you can fork the repository to your own GitHub account and clone it to your local machine using the command:
  ```sh
  git clone https://github.com/your-username/ProjectTemplate.git
  ```

Choose the method that best suits your workflow.

### 1.1 Note on Submodules

I do not recommend using this repository as a submodule, as it will not be updated with that use case in mind.

## 2. Folder structure and files

Here's a brief overview of the folder structure and key files in this repository:

- 📂 `R`: This folder should contain all `.R` files that define the functions used in the `{targets}` pipeline.
- 📂 `data`: Store raw and processed data files here.
- 📂 `ms`: Contains the manuscript files, typically in Quarto `.qmd` format.
- 📂 `output`: This is where the results, such as figures and tables, will be saved.
- 📂 `bib`: This is where the `.bib` reference file should be stored, along with the `.csl` citation style, and any template files. Currently a template `.docx` file is included, as is `the-american-naturalist.csl`.

## 3. How to use this template

This repository is designed to be used as a template for a reproducible workflow and manuscript. It has been created to suit my use case, but released as others may also find it helpful.

Once downloaded, install and initialise the `{targets}` package:

```r
install.packages("targets")
targets::use_targets()
```
Then, you can start the pipeline with:

```r
tar_make()
```

This will execute the pipeline and produce the results in the `output` folder.

## 4. Customizing the template

Feel free to customize the template to better fit your specific needs. You can modify the folder structure, add new functions, or change the manuscript format as required.

## 5. Getting help

If you encounter any issues or have questions, please [open an issue](https://github.com/irmoodie/ProjectTemplate/issues).
