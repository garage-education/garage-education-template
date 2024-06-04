# Garage Education Presentation Template

This repository contains a LaTeX Beamer template for creating educational presentations. The template is designed to be simple and minimalistic, yet professional and engaging.

## Getting Started

To get started, you need to have a LaTeX distribution installed on your machine. If you don't have one, you can download and install [TeX Live](https://www.tug.org/texlive/) or [MikTeX](https://miktex.org/).

## Structure

The main file of the template is `main.tex`. This file includes the document class, packages, and configurations. It also includes the front page and the chapters of the presentation.

The `preamble` directory contains the preamble file which includes the necessary packages and configurations for the template.

The `Figures` directory is where you can put your images and graphics. The path to this directory is already set in the `main.tex` file.

The `front_page` file contains the code for the front page of the presentation.

The `chapters` directory is where you can put your chapter files. You can include these files in the `main.tex` file.

## Usage

To use this template, you can fork this repository and clone it to your local machine. Then, you can start editing the `main.tex` file and the chapter files in the `chapters` directory.

You can compile the `main.tex` file using your LaTeX distribution. The output will be a PDF file of your presentation.

## Themes

This template supports both light and dark themes. You can choose the theme by uncommenting the corresponding line in the `main.tex` file:

For the light theme:
```latex
\usetheme[showmaxslides]{pureminimalistic}
```

For the dark theme:
```latex
\usetheme[darkmode, showmaxslides]{pureminimalistic}
```

Sure, you can append the above information to the `README.md` file. Here's how you can do it:

## Front Page Configuration

The `front_page.tex` file is where the title page of the presentation is defined. This file contains the title, author, and date information that appears on the first page of the document.

To modify the author and course title, you need to locate the `\title` and `\author` commands in the `front_page.tex` file.

For example, to change the course title to "Advanced Data Engineering", you would modify the `\title` command as follows:

```latex
\title[Advanced Data Engineering] %optional
{Advanced Data Engineering}
```

To change the author to "Moustafa Mahmoud" and his role to "Senior Solution Architect", you would modify the `\author` command as follows:

```latex
\author[John Doe] {
 John Doe \newline
 \footnotesize \textcolor{ballblue}{\textbf{Data Scientist}} \newline
}
```

The text inside the square brackets `[]` is the short version of the title or author, which is used in places where the full title or author would not fit, such as in headers or footers. The text inside the curly braces `{}` is the full version of the title or author, which is used on the title page and in other places where there is enough space.

After making these changes, save the `front_page.tex` file and recompile your LaTeX document to see the changes on the title page.

## Preamble
The `preamble` directory contains various setup files and configurations for the LaTeX document. These files define the overall style, layout, and other settings of the document.

The main file in this directory is `preamble.tex`. This file includes all the necessary packages and configurations for the document. It sets up the document class, loads the necessary LaTeX packages, defines new commands, and sets layout parameters.

To modify the overall settings of the document, you can edit the `preamble.tex` file or add new setup files to the `preamble` directory and include them in the `preamble.tex` file.

## Download The PDF
The `main.pdf` file is generated as an artifact of the GitHub Actions workflow defined in the `build.yml` file. After the LaTeX document is compiled, the `main.pdf` file is uploaded as an artifact.

To find and download the `main.pdf` file, follow these steps:

1. Go to your GitHub repository where the workflow is running.
2. Click on the "Actions" tab.
3. Click on the workflow run you're interested in. This will usually be the most recent run, but you can also select a previous run.
4. In the workflow run summary page, scroll down to the "Artifacts" section.
5. Click on the `main.pdf` artifact to download it.

The downloaded file will be a ZIP archive containing the `main.pdf` file. You can extract this file to view the PDF document.

## Contributing
If you want to contribute to this project, feel free to fork this repository, make your changes, and submit a pull request.


## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.