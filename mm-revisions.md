# mm-revisions

- This is file for keeping track of notes and revisions related to jupyter notebooks and code in the 'Understanding Animals' respository. These notes will be used to keep track of changes that need to be made - when you make a complete an edit please mark the checkbox to indicate that this change has been completed.

## general notes

- Are all of these jupyter notebooks referenced in the OER? This is something to check - we should have at least one link to each OER in the text. It could also be helpful to add a list of Notebooks as an appendix.
- We need to figure out how to access the datasources in each jupyter notebook: deciding whether this will happen in google drive or a library source (better). It appears that Borealis does have a python API - this will be ideal - we just need to check this out and confirm that it works, then replace all the code for accessing data in the notebooks.
- I'm not sure what is the best way to test the code - I think I'll do this in CoLab as this is where the notebooks will be accessed. Ideally we would test the code using the data in google drive: but this is currently not working for some reason (error: 'MessageError: Error: credential propagation was unsuccessful').
- Some of these notebooks offer a very specific and ideosyncratic piece of functionality - something that is not integral to the OER (Completed_Photoselect tool notebook.ipynb is one example). These notebooks can be kept in a collection of miscellaneous notebooks if they work; and if there are issues we can safely leave them out of the final version.
- It will make sense to organize the notebooks in folders by type.
- In several notebooks there are functions that have been broken into multiple code blocks - this is hard to read and I think should be avoided. There is a simple fix: to recombine the function into a single code block.
- All notebooks need an **introduction** that clearly describes what is the function of this notebook. This should include a section that describes **what you can do with it**. Some notebooks have this and some do not. There should also be a link in each notebook introduction to the pressbook.

## file notes

- **Completed_boundingboxcoco.ipynb**
  - Data access method needs to be changed.
  - 'image_path' variable is not defined
  - removed reference to individual images in the box 'Module: Set up the Object Detection Model & Image Directory' - I'm not sure why these were here as they don't seem to be doing any important work. This text can be restored if needed from the main branch before merging.
- **Completed_Photoselect tool notebook.ipynb**
  - I think this won't work, because the functions have been broken up into segments. Check in colab.
- **Completed.All Datasizes.Classifier.ipynb**
  - The introduction does not clearly state what is the purpose of this notebook and what you can do with it.
  - All google drive data references need to be changed.
  - This notebook seems to result from merging two notebooks: a number of functions appear twice, and the notebook is very long. I think this can reasonably be divided into two notebooks.
  - 'mount_google_drive()' function is defined twice in the notebook.
  - 'safe_get_image_files() function is defined twice in the notebook.
  - The 'process_datasets' function is defined but not used (should be 'process_dataset' ?).
  - Functions are sometimes broken up between code blocks.
  - Some code has been run in the cloud and the outputs are provided as images. This is helpful, but it should be more clear that the code in this case is not intended to be run in colab. Code that cannot be run in colab could be moved to the Pressbook.
- **Prompt Generator**
  - Functions are broken up between code blocks.
- **Blender**
  - Very large file.
  - Explains AV's work on synthetic animal images in blender.
  - Does not contain any code - this can be included in the pressbook as static content. 
- **Stable-Diffusion**
  - Too large - possibly split up.
- **COMPLETED-image-filter.ipynb**
  - Very useful notebook.
  - Somewhat repetitive: each section repeats the first section with minor changes. Possibly include a section that simply indicates what needs to be changed for each type of filter.
- **COMPLETED-random-manual-review.ipynb**
  - Very useful notebook.
- **COMPLETED-ft-data-prep.ipynb**
  - Very useful.
  - Introduction should indicate other datasets (in addition to COCO) that could be used with this notebook for YOLO training, and why you might choose one dataset over another.
- **COMPLETED-ResNet50-bounding-boxes.ipynb**
  - Very useful notebook.
  - There are three sections that are essentially independent of each other: I think these should be broken up into three separate notebooks.


## checklist of changes

- [ ] check that each jupyter notebook is linked at least once in the OER
- [ ] add a link to the pressbook in the introduction to each notebook
- [ ] add or update a 'run in colab' label for all notebooks
- [ ] add a list of jupyter notebooks to the OER as an appendix
- [ ] figure out how to connect to data sources - and change all references to google drive accordingly
- [ ] run all jupyter notebooks in colab and fix (or note) errors
- [ ] organize the notebooks into folders by functionality (or by OER table of contents)
- [ ] where functions have been divided into multiple code blocks, recombine into a single block, or make it clear that separate code blocks are not intended to be run individually (for example by including them as screenshots). As a rule, it should be possible to run all the code blocks in the notebook in sequence without generating an error, and ideally with output that is related to a specific code block rather than coming all at once.
- [ ] revisit notebook introductions: add link to pressbook and make sure that the introduction clearly states what you can do with this notebook.
- [ ] revisit notebook focus: split up if the purpose of the notebook and what you can do with it is not clear.
- [ ] for notebooks with no code ('Blender') - integrate this content in the pressbook. 

