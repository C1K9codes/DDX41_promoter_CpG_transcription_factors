# DDX41 Promoter CpG Transcription Factor Analysis

## Project Overview
This project investigates potential transcription factor interactions within CpG-rich regions of the DDX41 promoter.

The workflow involved extracting promoter sequence data and identifying subsequences for downstream transcription factor analysis.

---

## Objective
To identify and analyze transcription factor binding patterns in CpG-containing regions of the DDX41 promoter sequence.

---

## Workflow

### 1. Retrieve promoter sequence
The promoter sequence for **DDX41** was obtained from the UCSC Genome Browser.

### 2. Extract subsequence
A specific promoter subsequence of interest was extracted from the genomic region for focused analysis.

### 3. CpG region analysis
CpG-containing regions within the promoter subsequence were identified for investigation using CpGplot EMBOSS webtool. The region from 48-522 basepairs was identified as a potential CpG island with more than 60% GC content.

### 4. Transcription factor analysis
The selected sequence was analyzed to identify potential transcription factor binding sites.

### 5. Interpret biological relevance
Predicted transcription factor interactions were evaluated for possible regulatory roles in DDX41 expression.

---

## Data Source
- UCSC Genome Browser

Reference genome version:
- [Add hg19 / hg38]

Coordinates used:
177516961-177518961

---

## Methods
The specific gene i.e DDX41's genomic coordinates were taken from UCSC Genome Browser, Santa Cruz. Based on the exact genomic coordinates and orientation of the strand the promoter sequence coordinates were calculated. The view DNA sequence option was chosen to get the sequence. Afterwards, the DNA sequence was copy-pasted onto CpGplot EMBOSS webtool. The tool then determined the presence of CpG island based on parameters such as more than 200 bp and >50% of GC content. The gene DDX41 has CpG island from 48-522 base pairs which is about 475 bp long CpG stretch. 

From UCSC Genome Browser, the earlier copied and pasted sequence of about 2001 base pairs was taken to R and stored as Biostring/DNAString and subsequence was isoloated correspnding to that CpG island. Then complete pipeline for TF extraction was ran over the sub-sequence extracted and gave precise and most probable motifs and 21 transcription factors. Point to be noted, CpGplot works well for methylation TF data.
---

## Results
- Number of CpG sites identified - one CpG island was identified from 48 bp - 522 bp
- Number of transcription factors detected - 21 transcription factors
- Key transcription factors of interest - ARNT::HIF-1-alpha

---

## Future Work
- Validate predicted binding sites
- Compare across genome builds
- Functional annotation

---

## Author
[Charvi Khanna]
