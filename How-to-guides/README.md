# MPConnect User Guide

![MPConnect Logo](https://mpconnect.io/assets/mpconnectlogo-68718921.svg)

Welcome to the MPConnect User Guide!

This manual is designed to help you use [MPConnect](https://mpconnect.io), the standalone web application for microplastics analysis and characterization developed by [AbbaTek Group](https://abbatekgroup.com).
MPConnect enables scalable and reproducible research and monitoring of microplastics by leveraging machine learning to automate the physical identification, characterization, and quantification of microplastic particles, enabling repeatable results without requiring specialized expertise.

**MPConnect specializes exclusively in microplastic analysis in water samples.**

## Topics

### This Section

- [General Aspects](#general-aspects)
- [Getting Started](#getting-started)
- [Project Management](#project-management)
- [Batch Upload and Processing](#batch-upload-and-processing)
- [Analysis Types](#analysis-types)

### Other Sections

- [Data Visualization and Reporting](#data-visualization-and-reporting)
- [Troubleshooting](#troubleshooting)

## General Aspects

### Understanding Microplastics

Microplastics are small plastic particles with various physical and chemical properties:

- **Physical**: Shape, size (range), state of degradation
- **Chemical**: Polymer type(s), additives, fillers

Microplastics in a sample (also called a "matrix") can be measured by:

- **Number of particles** (count per sample volume/weight)
- **Mass content** (fraction relative to sample quantity)

Before choosing an analysis method, clearly define:

- The analytical question or objective
- The specific properties of microplastics to measure (e.g., size, shape, polymer type)

### MPConnect Analysis Capabilities

MPConnect provides three distinct analysis approaches for water samples:

- **Physical Analysis**: Particle size, shape, count, and morphological characteristics
- **Spectral Analysis**: Chemical identification and polymer type classification  
- **Combined Physical-Spectral Analysis**: Integrated approach providing comprehensive particle characterization

---

## Getting Started

### Working Environment

All analytical steps (sampling, preparation, detection) must:

- Be undertaken in a plastics-free or low-plastics working conditions.
- Avoid use of plastic tools (e.g. containers, tubes, vessels) unless they're made from plastics not being analyzed.
- Prefer metal, glass, or ceramic labware and equipment.
- Use non-synthetic personal protective equipment (e.g. lab coats, gloves).
- Perform recovery tests during each analytical step to ensure accuracy.
- Where possible, perform sample handling in:
  - Laminar flow hoods
  - Cleanrooms (ISO Class 3 or better)

### Sample Sterilization

Determine if sterilization is needed (especially for wastewater, sewage sludge, organic wastes), as different sterilization methods can affect microplastic integrity:

| Method                          | Risk to Microplastics                            |
|---------------------------------|--------------------------------------------------|
| **Steam sterilization**         | May melt microplastics                           |
| **Radiation** (gamma, beta, UV) | Can degrade polymer chains and oxidize particles |
| **Chemical sterilization**      | May chemically alter surface or structure        |

After sterilization, perform recovery tests to confirm that microplastics are still detectable and intact.

### Quality Control and Documentation

- Record all analytical conditions and steps.
- Include blank samples to check for contamination.

The number of blanks depends on the analytical method being used.
Blank samples help detect cross-contamination from:

- Airborne plastic particles
- Labware residue
- Handling errors

### Particle Size Classification

| Classification | Unit | **Microplastics** | | | | | |**Large microplastics**                                    |
|----------------|------|-------------------|-|-|-|-|-|-----------------------------------------------------------|
|**Particle size classes**|µm|1 to < 5|5 to < 10|10 to < 50|50 to < 100|100 to < 500|500 to < 1 000|1 000 to 5 000|
|**Average particle size**|µm|3|7.5|30|75|300|750|3 000|
|**Massᵃ**                |mg|1,4×10⁻⁸|2,2×10⁻⁷|1.4×10⁻⁵|2,2×10⁻⁴|0,014|0,22|14|
|**Number of particles in 14,13 mg**|number|1,0×10⁹|6,4×10⁷|1,0×10⁶|6,4×10⁴|1 000|64|1|

 ᵃ  Mass here is determined from the average particle size assuming spherical particle with a density of 1.

> Source: Extracted from *ISO/DIS 24187:2021(E), Principles for the analysis of plastics and microplastics present in the environment*, © ISO 2021.

### System Requirements

[Add Info Here - Browser compatibility, network requirements, account setup procedures]

---

## Project Management

### Projects in MPConnect

Projects in MPConnect serve as organizational containers for related water sample analyses. Each project can contain multiple batches of image samples with associated geographic metadata.

### Creating a New Project

To create a new project in MPConnect:

1. **Click "Projects"**  
   Use the navigation bar to access the **Projects** page.

2. **Select the "New" Tab**  
   Click the **New** tab to open the project creation form.

3. **Enter Project Details**  
   - **Project Name**: A descriptive name for your project.  
   - **Project Description**: A summary of the sampling effort, location, or analysis purpose.

4. **Submit the Project**  
   Click **Submit** to save the project. It will now appear in the **Load** tab and be set as the active project on the **Home** screen.

### Project Organization

MPConnect makes it easy to manage multiple projects:

- **View Projects**  
   From the **Projects** page, use the **Load** tab to see a list of existing projects. Each entry shows the project name, description, and number of image batches.

- **Switch Projects**  
   Click on a project name (in blue) to make it the active project. The active project appears on the **Home** screen, where you can upload batches directly.

- **Delete or Export Projects**  
   Use checkboxes to select one or more projects to delete or export. Downloads are available in CSV or JSON format.

---

## Batch Upload and Processing

### Understanding Batches

A batch consists of multiple image samples with latitude and longitude coordinates indicating where each sample was collected. Batches are uploaded to projects for organized analysis.

### Image Requirements

[Add Info Here - Specific file format, size, and quality requirements]

### Required Batch Information

Each batch upload requires the following core information:

- **Batch Name**: A descriptive identifier for the batch
- **Description**: Details about the sampling campaign, conditions, or objectives
- **Latitude**: GPS coordinate of sampling location (decimal degrees)
- **Longitude**: GPS coordinate of sampling location (decimal degrees)

#### Optional Sample Metadata Fields

MPConnect allows you to add custom fields for enhanced sample tracking and analysis. Available optional fields include:

- **Custom**: User-defined field for project-specific metadata
- **Counted**: Indicator if particles have been manually counted
- **Particle #**: Unique identifier for individual particles within samples
- **Colour**: Color classification or description of particles
- **Category**: Pre-classification or grouping of samples
- **Comments**: Additional notes, observations, or special conditions
- **Length (mm)**: Physical measurement data for particles
- **Width (mm)**: Physical measurement data for particles
- **RAMAN ID**: Reference identifier for Raman spectroscopy analysis
- **RAMAN Notes**: Additional notes related to spectroscopic analysis

### Step-by-Step Batch Upload Process

1. **Select Target Project**
   Ensure the correct project is active on the **Home** screen before beginning upload.

2. **Prepare Batch Information**
   - Choose a descriptive Batch Name that identifies the sampling location, date, or conditions
   - Write a comprehensive Description including sampling methodology, environmental conditions, and objectives
   - Set GPS coordinates (Latitude and Longitude) using either:
     - **Manual Entry**: Type coordinates directly in decimal degrees format
     - **Interactive Map**: Click the map button to open an interactive map interface, place the marker on your sampling location, and click "Done" to automatically fill both coordinate fields

3. **Configure Additional Fields**
   - Click "Add New Field" to select relevant optional metadata fields
   - Add multiple fields as needed for your research requirements
   - Consider standardizing field usage across batches for consistency

4. **Image Upload**
   - Upload image files each sample

5. **Validation and Submit**
   - Review all entered information for completeness and accuracy
   - Check that geographic coordinates fall within expected ranges
   - Submit the batch

---

## Analysis Types

MPConnect offers three distinct analysis approaches for water samples:

### Physical Analysis

**What Physical Analysis Provides:**

- Particle count and size distribution
- Shape classification (fiber, fragment, sphere, film)
- Morphological characteristics
- Color analysis
- Spatial distribution mapping

When physical analysis is complete, MPConnect provides detailed classification results with confidence levels for each particle type:

- **Fragments**: Irregular plastic pieces resulting from degradation or fragmentation of larger plastic items
- **Fibers**: Elongated thread-like particles typically from synthetic textiles or rope materials
- **Films**: Thin sheet-like particles from plastic bags, packaging, or degraded film materials
- **Foam**: Expanded plastic particles from polystyrene foam, packaging materials, or insulation
- **Rubbers**: Elastic polymer particles from tire wear, rubber products, or synthetic rubber materials
- **Spheres**: Round particles from microbeads, pellets, or weathered plastic fragments

**When to Use Physical Analysis:**

- When polymer identification is not required
- For rapid screening of large sample sets
- When focusing on particle morphology and size distribution
- For comparative studies of particle shapes across different locations

### Spectral Analysis

**What Spectral Analysis Provides:**

- Polymer identification (PE, PP, PS, PET, PVC, etc.)
- Chemical composition analysis
- Additive and filler detection
- Degradation assessment
- Source attribution capabilities

**When to Use Spectral Analysis:**

[Add Info Here - Specific use cases and benefits]

### Combined Physical-Spectral Analysis

**What Combined Analysis Provides:**

- Complete particle characterization with both morphological and chemical data
- Chemical confirmation of visual particle identification
- Enhanced accuracy with reduced false positives
- Comprehensive particle database linking physical and chemical properties
- Correlation analysis between particle morphology and polymer type

**When to Use Combined Analysis:**

- For comprehensive research studies requiring full particle characterization
- When maximum accuracy and validation are required
- For studies investigating relationships between particle morphology and polymer type
- When building comprehensive databases for long-term monitoring programs

### Selecting Analysis Type

Choose your analysis method based on your research objectives:

- **Physical Analysis Only**: Best for morphological studies, rapid screening, or when chemical identification is not required
- **Spectral Analysis Only**: Ideal when particle identification is already established and only chemical confirmation is needed
- **Combined Analysis**: Recommended for comprehensive studies, regulatory compliance, or when maximum accuracy is required

### Analysis Status and Results Management

**Analysis Status Indicators:**

- **Complete**: Analysis has finished successfully and results are available
- **Processing**: Analysis is currently running
- **Failed**: Analysis encountered an error and needs to be restarted
- **Pending**: Analysis is queued but not yet started

**Results Actions:**
Each completed analysis provides several action options:

- **Return**: Navigate back to the sample list
- **Edit**: Modify analysis parameters
- **Delete**: Remove the analysis results
- **Download**: Export results in various formats (CSV or JSON)
- **Visualize**: View graphical representations of the analysis data

---

## Data Visualization and Reporting

### Dashboard Overview

[Add Info Here - Description of Dashboard layout]

### Analysis Results Display

[Add Info Here - How physical, spectral, and combined analysis results are presented]

### Data Export

[Add Info Here - Available export options/formats]

---

## Troubleshooting

### Common Upload Issues

[Add Info Here - Typical problems during batch upload and solutions]

### Analysis Problems

[Add Info Here - Common analysis issues and troubleshooting steps]

### Performance Issues

[Add Info Here - System performance problems and solutions]

### Getting Help

[Add Info Here - Support contact information and resources]

---

*For the most current information and updates, visit [MPConnect](https://mpconnect.io) or contact [AbbaTek Group](https://abbatekgroup.com/)*
