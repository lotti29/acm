# Template Info

<<<<<<< HEAD
This is a fork of the existing ACM quarto template (https://github.com/quarto-journals/acm). It incorporates an open PR by cderv (https://github.com/quarto-journals/acm/pull/39) that fixes some problems with the current version, namely:
=======
This is a fork of the existing ACM quarto template (https://github.com/quarto-journals/acm). It incorporates an open PR by cderv that fixes some problems with the current version, namely:
>>>>>>> df966f04124ef9e8a0e30c67fc13e5a41c30f4eb
- alt text causing render failure (see below)
- outdated .cls and .bst files
- .cls and .bst configuration in the _extension.yml
- Libertinus fonts not being installed
- incorrect DOI formatting

The template.qmd should now render out of the box. 

Note that the alt text fix is not a true fix, as it only prevents the faulty conversion of fig-alt into ACM's `\Description{}` format. Images in rendered PDFs will therefore not have any `\Description{}` - this may need to be added manually to the .tex file before submission.

# Association of Computing Machinery (ACM)

This Quarto format will help you create documents for the Association of Computing Machinery. To learn more about ACM publications, see [ACM's Information for Authors page](https://www.acm.org/publications/authors/information-for-authors). For more about Quarto and how to use format extensions, see <https://quarto.org/docs/journals/>.

## Creating a New Article

You can use this as a template to create an article for the Association of Computing Machinery. To do this, use the following command:

```quarto use template quarto-journals/acm```

This will install the extension and create an example qmd file and bibiography that you can use as a starting place for your article.


## Installation For Existing Document

You may also use this format with an existing Quarto project or document. From the quarto project or document directory, run the following command to install this format:

```quarto add quarto-journals/acm```

## Usage 

To use the format, you can use the format names `acm-pdf` and `acm-html`. For example:

```quarto render article.qmd --to acm-pdf```

or in your document yaml

```yaml
format:
  pdf: default
  acm-pdf:
    keep-tex: true    
```

You can view a preview of the rendered template at <https://quarto-journals.github.io/acm/>. 

