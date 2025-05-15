# mm-revisions

- This is file for keeping track of notes and revisions related to jupyter notebooks and code in the 'Understanding Animals' respository. These notes will be used to keep track of changes that need to be made - when you make a complete an edit please mark the checkbox to indicate that this change has been completed.

## general notes

- Are all of these jupyter notebooks referenced in the OER? This is something to check - we should have at least one link to each OER in the text. It could also be helpful to add a list of Notebooks as an appendix.
- We need to figure out how to access the datasources in each jupyter notebook: deciding whether this will happen in google drive or a library source (better). It appears that Borealis does have a python API - this will be ideal - we just need to check this out and confirm that it works, then replace all the code for accessing data in the notebooks.
- I'm not sure what is the best way to test the code - I think I'll do this in CoLab as this is where the notebooks will be accessed. Ideally we would test the code using the data in google drive: but this is currently not working for some reason (error: 'MessageError: Error: credential propagation was unsuccessful').  

## file notes

- 'Completed_boundingboxcoco.ipynb'
  - Data access method needs to be changed.
  - 'image_path' variable is not defined
  - removed reference to individual images in the box 'Module: Set up the Object Detection Model & Image Directory' - I'm not sure why these were here as they don't seem to be doing any important work. This text can be restored if needed from the main branch before merging.
- 


## checklist of changes

- [ ] check that each jupyter notebook is linked at least once in the OER
- [ ] add a list of jupyter notebooks to the OER as an appendix
- [ ] figure out how to connect to data sources - and change all references to google drive accordingly

