# 20250523

**Subject:** Review of Team Discussion and Task Prioritization  
**Attendees:** Mark, AV, Jenelle  
**Purpose:** This is a team meeting focusing on project progress, tool adoption, and task allocation.

## Key Themes & Important Ideas:

### Progress on Grant Application Response

Mark and Yuhao successfully used AI to generate an email response for a grant application based on a discussion transcript.

> Mark notes, "It was, actually, it was quite nice. We just had like a 10-minute discussion about it, and then. Um, and then you how, based on that discussion transcript, just ask that to generate the email response."

This highlights the practical application and efficiency gains from using AI for communication.

### New Codebase Features and Tools (Quote Code)

The discussion introduces updates to the codebase, specifically referencing **Claude Code**. New functionalities have been added, increasing the command count from around five to "quite a few more." Noteworthy features include:

- **cloud.md file with code base documentation:** Useful for setting up new repositories.
- **Install GitHub app MCP:** Enables connection to MCP servers for integration with programs like Revit or Rhino.
- **Memory Files:** Cloud now creates "Repository, like memories of what you've talked about and then refers back to them later." The exact functionality is unclear, but it suggests improved contextual awareness.
- **PR comment:** Functionality for working with pull requests.
- **Vim Feature:** A new feature related to the Vim text editor.
- **Vibe:** A potentially humorous or inside-joke command, as described by AV:
  > "What is slash vibe?"
  >
  > Mark's response: "Oh. Um, the time was part of five coding based on,"
  >
  > AV's comment: "Seems like an inside joke."

### Markdown for Document Formatting and Collaboration

Mark emphasizes the use of Markdown for document formatting and its benefits for collaboration, particularly with Git.

- Markdown allows formatting text files to produce various outputs (Word, PDF, PowerPoint, etc.) while remaining in a text file format.
  > Mark states, "markdown is essentially a way to format text documents... with markdown, you have you're still in a text file, but you can use that text file to produce all different kinds of output."
- **Basic Markdown syntax** (hashtags for headings, asterisks for bold/italic, square brackets for checkboxes) is explained.
- **VS Code's Markdown preview feature** is mentioned as a way to read the formatted document, while editing must be done in the text file:
  > "you can't do it in the preview. The preview doesn't. It's kind of non-interactive, but you can just put a little X there. And that will make the checkbox check in the in the preview."
- Markdown is described as "very git friendly," allowing for easy line-by-line review of changes.

### Task Prioritization and Allocation (Focus on AV and Janelle)

A significant portion of the discussion focuses on organizing and prioritizing tasks, particularly for AV and potentially Janelle.

#### Notebook Revisions

A critical, high-priority task estimated at around 20 hours. This involves:

- Collecting all data sources in a single drive folder and updating data access in notebooks for testing.
- Testing the output of each cell and the notebook as a whole.
- Specific issues needing addressing:
  - Undefined variables
  - Splitting notebooks
  - Broken code blocks
  - Repetition
  - Consolidating functions
- Standard tasks across all notebooks:
  - Adding introductions
  - Verifying code block output
  - Ensuring meaningful output when connected to data

#### Summer Workshop Preparation (Medium Priority)

Preparing materials for a workshop on WSL2, Olama, and Open Web UI installation. Dependencies include talking to Mitch for existing materials/ideas. Mark suggests a simple, step-by-step text guide.

#### Support for Janelle (Support Task)

Assisting Janelle with computer setup, explaining the Git workflow (clone, create, commit, push), practicing with test examples, and delegating some notebook review tasks.

> Mark states, "to give support to Janelle for for setting like any other, like finishing the setup of your computer to... Explain, like the get workflow and perhaps go through that with Janelle... and then to delegate to Janelle. Some of the notebook review tasks."

#### Conference Abstract (Future Task, after notebook work)

Drafting a conference abstract for AI design practices by the June 11th deadline. The abstract could focus on synthetic images with a hint of future work using game engines. It should collect relevant references and up to five images.

#### Literature Reviews (Lower Priority)

Conducting literature reviews for various papers (conference, timber databases, Animals paper) using tools like Deep Research and Library Search for an overview and collection of materials.

#### Cloning and Transferring Alienware (Lower Priority)

Transferring a clone to another Alienware machine.

### Notebook Organization Structure

A suggested organization structure for notebooks is presented:

- Data Set Exploration
- Object Detection
- Classification
- Visualization
- Synthetic Generation
- Miscellaneous

This structure is considered helpful for tracking and ensuring each notebook has a "single clear purpose - that's really important."

### Colab Testing Checklist

A checklist for testing notebooks in Google Colab is outlined:

- All code blocks run in sequence without errors.
- Data source is accessible.
- Output generates correctly.
- Introduction documentation is accurate.
- Links to pressbook are functional (not currently possible).
- Each notebook has a single clear purpose.
- Functions are complete in single code blocks.
- Introduction explains purpose and usage.
- Data access works via Borealis (final stage).

### Data Source Management (Google Drive and Borealis)

- Confirmation that notebook data files are already located in a single shared Google Drive folder ("notebook data files").
  > AV confirms, "everything is leading into this."
- Mark clarifies that this setup is sufficient for current testing purposes but will eventually transition to Borealis.
- The process for Borealis integration will involve zipping and unzipping data in Colab.
  > Mark notes, "we'll just take all the folders that are all the files that are in there... And Add them to Borealis, and then we'll be able to access them. We'll probably need to like zip them up, and you know, make them."

### Using AI for Notebook Introductions

AV shares their experience and iteration on prompts for generating notebook introductions using AI.

- Initial prompts were too broad, resulting in generic output.
- Iterated prompts yielded better results, being more specific to the notebook's purpose and details:
  > "it talked about oh, different size. It's very specific to The Notebook itself. That's, that's really great."
- Mark suggests refining prompts for consistency across notebooks to facilitate search and replace for standardization.
- A humorous tangent discusses the "hyper professional" or "hyper excited" tone often generated by models and how to potentially prompt for a more "matter of fact" tone. This includes a discussion of Google's Notebook LM podcast feature and the viral "chicken chicken chicken" paper podcast.

### Adoption of ChatGPT Plus and Notebook LM

- The team decides to set up ChatGPT Plus accounts for AV and Janelle, with Mark providing payment information.
- Mark suggests it will be useful for company projects (literature review, general Q&A) and the notebook work (resolving questions, getting feedback).
- Notebook LM features are discussed, including its "ragged application" capabilities (uploading multiple file types for querying and summarization) and the podcast generation feature (which is found to be "kind of weird" and "kind of creepy" but also "very fun").
- Other Notebook LM features mentioned:
  - Canvas (for writing with live notes/feedback)
  - Deep Research (for conducting structured research with clarifying questions and documented results)
- These are suggested as potentially useful tools for the conference abstract and literature reviews.

### Git Workflow and Saving Practices

A brief review of Git saving practices is provided:

- **Ctrl + S:** Saves to the local machine.
- **Commit:** Saves to the local Git repository.
- **Sync:** Saves the commit to the branch in the cloud (visible to others) and locally.
- **Push:** Merges the branch (implied, though the terminology is slightly simplified).

Good practice includes committing when stepping away and pushing/deleting branches after merging.

## Action Items:

- AV to coordinate with Janelle regarding task allocation and collaboration on project work, aiming for up to 10 hours per week if feasible.
- AV to continue refining prompts for notebook introductions, focusing on consistency and specifying terms for standardization.
- AV to explore using other models (besides the initial one tested) for generating introductions.
- AV and Janelle to set up ChatGPT Plus accounts.
- Mark to provide API keys for necessary tools (specifically Quote Code) via Teams.
- AV and Janelle to explore Notebook LM features like Canvas and Deep Research for potential use in literature reviews and abstract writing.
- AV and Janelle to practice the Git workflow, potentially using the terminal for better internalization, as outlined in the provided cheat sheet.
- AV to perform a "pull" in Git to merge the recent changes made by Mark.

## Notes:

- The "vibe" command remains a point of curiosity, likely an internal joke.
- The suggested weekly schedule generated by the AI is seen as "Micromanaging."
- The AI-generated organization structure for notebooks is considered helpful for clarifying purpose, although the categories are currently "very computer sciency" and may need translation to design disciplines.
- The data is confirmed to be in a single Google Drive folder, simplifying that step for now.
- Cleaning of the data sets is a lower priority at this time.
- The transition to Borealis for data access is a future step.
- Mark will merge his recent work on notebooks.
- This briefing document captures the essential information from the meeting, providing a clear overview of the project status, tools being adopted, and the planned activities for the team.