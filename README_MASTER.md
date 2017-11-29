# ProjectTemplateStructure
A template for guiding the creation of new projects

## Inspiration
- [MRI layout](http://nikola.me/folder_structure.html)
- [Code layout](https://drivendata.github.io/cookiecutter-data-science/)

## Variables
- ProjectName = [your project name]

## Scope of this Template
- This template will cover the directories to store data and how to store metadata (generally).
  This template will **NOT** cover how the actual data should be stored.

## So you want to manage data?
### resources
- <sup>[1]</sup>[isacommons](http://www.isacommons.org/index.html)
- <sup>[2]</sup>[axiomdatascience](http://www.axiomdatascience.com/best-practices/index.html#)

### Standards for DirectoryNames and file_names
A standard rule that applies to both directories and file names is to only use alphanumeric characters (and underscore) to name directories and files.
If you have a motivated reason you can include periods [.] and dashes [-], but by default do not include these in your file names (excluding the period the extension uses (e.g. .txt, .csv, .tsv, etc.)

Unless agreed upon for a specific context the following characters are banned for naming directories or files
```
[space][tab],/?'":;|\=+()[]()*&^%$#@!`~
```
#### DirectoryNames
The default naming scheme for directories (i.e. folders) should use [CamelCase](https://en.wikipedia.org/wiki/Camel_case).
However, significant departures could occur if the directory name becomes a part of the file name (see [BIDS](http://bids.neuroimaging.io/bids_spec1.0.2.pdf)). CamelCase is more compact than [snake_case](https://en.wikipedia.org/wiki/Snake_case), and we generally don't need the extra stylized notation (version control, date stamping) that looks better in snake_case. In short, the justification for CamelCase to name directories is two-fold:
1. Compact
2. distinguishes directories from filenames
**NOTE:**: avoid abbreviations if possible, but if the abbreviation is the most sensical name, use all uppercase (e.g. MRI, FMRI). Naming is a balance between length and clarity.

#### file_names
The default naming scheme for files should use [snake_case](https://en.wikipedia.org/wiki/Snake_case). snake_case gives us the lattitude to stylistically timestamp files, yyyymmdd_file_name.txt, or fork files to do something experimental, jdkent_file_name.txt. In general, all alpha characters should be lowercase (e.g. MRI becomes mri, MNI becomes mni, etc.), this will promote consistancy across file names and make it easier to find files.



