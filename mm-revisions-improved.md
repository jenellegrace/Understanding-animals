# MM-Revisions - Improved Structure

## Project Overview
This file tracks notes and revisions for jupyter notebooks and code in the 'Understanding Animals' repository. These notes are used to track changes that need to be made for the Wild Winnipeg OER project.

**Status Legend:** ✅ Complete | 🔄 In Progress | ❌ Not Started | ⚠️ Blocked

---

## High-Level Project Tasks

### Data Infrastructure 🔄
- [ ] **HIGH** - Migrate from Google Drive to Borealis API for data access
- [ ] **HIGH** - Test Borealis Python API functionality  
- [ ] **MEDIUM** - Update all data access code across notebooks

### Documentation & Integration ❌
- [ ] **HIGH** - Verify each notebook is linked in OER
- [ ] **HIGH** - Add pressbook links to all notebook introductions
- [ ] **MEDIUM** - Create notebook appendix for OER
- [ ] **LOW** - Add/update 'Run in Colab' labels

### Testing & Quality Assurance 🔄
- [ ] **HIGH** - Test all notebooks in Google Colab
- [ ] **MEDIUM** - Fix credential propagation issues
- [ ] **LOW** - Clean up test outputs and debugging code

---

## Notebook Categories & Status

### 📊 Object Detection & Classification
| Notebook | Status | Priority Issues | Est. Effort |
|----------|--------|----------------|-------------|
| `Completed_boundingboxcoco.ipynb` | ⚠️ | Data access, undefined variables | 2-3 hours |
| `COMPLETED-ResNet50-bounding-boxes.ipynb` | 🔄 | Split into 3 notebooks | 4-5 hours |
| `COMPLETED-yolov5-pretrained.ipynb` | ✅ | Ready | - |
| `Completed.All Datasizes.Classifier.ipynb` | ❌ | Major restructuring needed | 6-8 hours |

### 🎨 Image Generation & Synthesis  
| Notebook | Status | Priority Issues | Est. Effort |
|----------|--------|----------------|-------------|
| `Stable Diffusion.ipynb` | ❌ | Too large, needs splitting | 3-4 hours |
| `Blender.ipynb` | ⚠️ | No code, move to pressbook | 1 hour |
| `Prompt Generator.ipynb` | 🔄 | Broken code blocks | 2 hours |

### 🔍 Dataset Exploration & Filtering
| Notebook | Status | Priority Issues | Est. Effort |
|----------|--------|----------------|-------------|
| `COMPLETED-image-filter.ipynb` | ✅ | Minor repetition cleanup | 1 hour |
| `COMPLETED-random-manual-review.ipynb` | ✅ | Ready | - |
| `COMPLETED-ft-data-prep.ipynb` | 🔄 | Improve intro, add dataset options | 2 hours |

### 📈 Visualization & Analysis
| Notebook | Status | Priority Issues | Est. Effort |
|----------|--------|----------------|-------------|
| `COMPLETED-close-encounters.ipynb` | ✅ | Ready | - |
| `COMPLETED-matplotlib-visualization.ipynb` | ✅ | Ready | - |
| `COMPLETED-random-interactive-image.ipynb` | ✅ | Ready | - |
| `COMPLETED-sightings-bar-graph.ipynb` | ✅ | Ready | - |
| `COMPLETED-treemap.ipynb` | ✅ | Ready | - |
| `COMPLETED_100grid.ipynb` | ✅ | Ready | - |

### 🔧 Miscellaneous Tools
| Notebook | Status | Priority Issues | Est. Effort |
|----------|--------|----------------|-------------|
| `Completed_Photoselect tool notebook.ipynb` | ⚠️ | Broken functions, optional for OER | 3 hours |

---

## Issue Categories

### 🔗 Data Access Issues
**Root Cause:** Google Drive credential propagation failures
- `Completed_boundingboxcoco.ipynb` - Data access method needs change
- `Completed.All Datasizes.Classifier.ipynb` - All Google Drive references need updating
- **Solution:** Implement Borealis API across all notebooks

### 🔧 Code Structure Issues
**Pattern:** Functions broken across multiple code blocks
- `Completed_Photoselect tool notebook.ipynb` - Functions segmented
- `Prompt Generator.ipynb` - Functions broken up
- `Completed.All Datasizes.Classifier.ipynb` - Duplicate functions, broken blocks
- **Solution:** Consolidate functions into single code blocks

### 📝 Documentation Issues
**Pattern:** Missing or unclear introductions
- All notebooks need pressbook links
- Several notebooks lack clear purpose statements
- `COMPLETED-ft-data-prep.ipynb` needs dataset comparison info
- **Solution:** Standardize introduction template

### ⚙️ Technical Issues
**Pattern:** CoLab compatibility and undefined variables
- `Completed_boundingboxcoco.ipynb` - 'image_path' variable undefined
- Several notebooks have untested CoLab compatibility
- **Solution:** Systematic CoLab testing protocol

---

## Detailed Notebook Issues

### High Priority Fixes

#### `Completed.All Datasizes.Classifier.ipynb` ❌
**Issues:**
- [ ] Unclear purpose/introduction
- [ ] Google Drive data access needs migration
- [ ] Appears to be merged from 2 notebooks (very long)
- [ ] `mount_google_drive()` function defined twice
- [ ] `safe_get_image_files()` function defined twice  
- [ ] `process_datasets` function defined but unused (typo for `process_dataset`?)
- [ ] Functions broken across code blocks
- [ ] Has pre-run cloud outputs (clarify these can't run in CoLab)

**Recommended Action:** Split into 2 focused notebooks

#### `COMPLETED-ResNet50-bounding-boxes.ipynb` 🔄
**Issues:**
- [ ] Contains 3 independent sections
- [ ] Should be split into 3 separate notebooks

**Recommended Action:** Create focused single-purpose notebooks

#### `Completed_boundingboxcoco.ipynb` ⚠️
**Issues:**
- [ ] Data access method needs change
- [ ] `image_path` variable not defined
- [ ] Removed reference to individual images (can restore from main branch if needed)

### Medium Priority Fixes

#### `Stable Diffusion.ipynb` ❌
**Issues:**
- [ ] Very large file size
- [ ] Consider splitting for better usability

#### `COMPLETED-ft-data-prep.ipynb` 🔄
**Issues:**
- [ ] Introduction needs dataset comparison (beyond COCO)
- [ ] Should explain dataset selection criteria

#### `COMPLETED-image-filter.ipynb` ✅
**Issues:**
- [ ] Somewhat repetitive sections
- [ ] Could add summary of changes needed per filter type

### Low Priority / Optional

#### `Completed_Photoselect tool notebook.ipynb` ⚠️
**Status:** Optional for final OER version
**Issues:**
- [ ] Functions broken into segments
- [ ] Very specific/ideosyncratic functionality
- [ ] Test in CoLab to determine if salvageable

#### `Blender.ipynb` ⚠️
**Status:** Move to pressbook as static content
**Issues:**
- [ ] Very large file
- [ ] Contains no executable code
- [ ] Documents AV's synthetic animal work

---

## Organization Recommendations

### Folder Structure
```
jupyter-notebooks/
├── 01-Dataset-Exploration/
├── 02-Object-Detection/  
├── 03-Classification/
├── 04-Visualization/
├── 05-Synthetic-Generation/
└── 99-Miscellaneous/
```

### Notebook Naming Convention
- Use consistent prefixes: `01-`, `02-`, etc.
- Include functionality in name
- Remove "COMPLETED" prefix after reorganization

---

## Testing Protocol

### CoLab Testing Checklist
- [ ] All code blocks run in sequence without errors
- [ ] Data sources accessible
- [ ] Outputs generate correctly
- [ ] Introduction/documentation accurate
- [ ] Links to pressbook functional

### Quality Standards
- Each notebook should have single, clear purpose
- All functions should be complete in single code blocks
- Introductions must explain purpose and usage
- Data access should work via Borealis API

---

## Completion Tracking

**Overall Progress:** 40% Complete

**Next Sprint Priorities:**
1. Fix data access infrastructure (Borealis API)
2. Split large notebooks (`Completed.All Datasizes.Classifier.ipynb`, `COMPLETED-ResNet50-bounding-boxes.ipynb`)
3. Test all notebooks in CoLab
4. Standardize introductions and documentation

**Estimated Total Effort:** 25-35 hours