# CATALYST HACKATHON (2026-03-06)::: Introducing the Palmetto2 bioLLM infrastructure prototype.

## Invitees 
### CCIT/RCD Engineers
Carl Ehrett <cehrett@clemson.edu>  
Doug Dawson <dndawso@clemson.edu>  
Zachary Gerstner <zigerst@clemson.edu>  
Jill Gemmill <gemmill@clemson.edu>  

### Biologists
Alex Feltus <ffeltus@clemson.edu>  
Xusheng Ai <xai@clemson.edu>  
Tzu-Yu Chu <tzuyuc@clemson.edu>  
Gabriel Serrano <gserran@clemson.edu>  
Varun Sethi <vsethi@g.clemson.edu>  
Sarah Moorshead <smoorsh@g.clemson.edu>   
Macy Rietz <mrietz@g.clemson.edu>  
Maura Korte <mjkorte@clemson.edu>  
William Boone <wbboone@g.clemson.edu>  
Marc Russel Birtwistle <mbirtwi@clemson.edu>  
Jonah Huggins <jrhuggi@g.clemson.edu>  
Afrid <ashirse@g.clemson.edu>   
Amna Islam <amnai@clemson.edu>   
Atalanta Harley-Gasaway <amhrnnd@clemson.edu>  
Siyu Huang <siyuh@clemson.edu>  
Cameron Brown <cbrow37@g.clemson.edu>  
David F Clayton <dfclayt@clemson.edu>  
Antonino Malacrino <amalacr@clemson.edu>  

### Computer Scientists & Engineers
Melissa Smith <smithmc@clemson.edu>  
Adam Niemczura  <aniemcz@clemson.edu>  
Oyinlolu Odetoye <oodetoy@clemson.edu>

### Materials Scientists
Dilpuneet Aidhy <daidhy@clemson.edu>  
Mark Allen Mueller <mmuell3@clemson.edu>  
ORIYOMI RASAK OPETUBO <oopetub@clemson.edu>  
Suyash Varshney <suyashv@clemson.edu>  
mjzakrz <mjzakrz@g.clemson.edu>  
Sriram Vishnubhotla <svishnu@clemson.edu>  

## Background 
Members of the CCIT-RCDE division and faculty from Clemson Genetics & Biochemistry Department, Chemical and Biomolecular Engineering Department, Electrical and Computer Engineering department and the School of Computing have joined forces to create modular poly-domain research generative AI ecosystem (Hub-Spoke model) on Palmetto2 called Clemson Advanced Computational Analytics and Learning for Integrated Science Translation (CATALYST--possible system name).

Phase one of CATALYST development is applying the OpenAI system on Plametto2 (codex, MCP server, vLLM) to build a Life Science research facet called bioLLM (placeholder name).

bioLLM builds upon recent advances in biological foundation models, Stanford's Biomni framework, and openAI LLM middleware (codex, MCP server), the team has created an extensible, locally-deployed AI platform prototype operating on Clemson's Palmetto2 HPC cluster. The ecosystem addresses current limitations in fragmented bioinformatics tools, scalability, security, and sustainability. Through an innovative agentic framework, Clemson researchers will gain access to specialized bioLLMs for genomics, transcriptomics, proteomics, and systems biology applications.   

In order to facilitate usage and harden this system, we will be hosting hackathons in 2026 with exclusive access to alpha test bioLLM ecosystem.  The first hackathon will be a small group of hackers that will test prompt the agentic bioLLM system to perform scientific discovery, usage documentation, and identify gaps in the system.  

## When & Where
The second Workshop will be a drop in on March 6(Fri) from 9am to noon followed by Discord collaboration for 7 days.
There will be synchronous Zoom meeting at 9am-10am https://clemson.zoom.us/j/9452064261   
Feltus will be in Zoom 9am to noon each day.   

## Collaboration. 
Discord server invite:  https://discord.gg/QXJ3eNgq  
Discord server URL: https://discord.com/channels/1461097829706760202/1461097830239305923  

## Pre-workshop tasks (User)
1.	Obtain OpenAI account with your clemson.edu email (not g.clemson.edu)
2.  Install codex with https://git.rcd.clemson.edu/biollms/biocodex
3.  Run some test prompts.

## Pre-workshop tasks (Admin)
1. Tool inventory, format and installation documentation
2. Log parsing documentation.
3. Genomic data access documentation
4. General biological workflow documentation for a Python/bash iterate user:  
    * ExperimentalDesign>>>InputDataCollection>>>Algorithm(Code)>>>Results
    * Working Directory structure (input_data, code, results, methods, logs) 

## Workshop Charge 
You have two choices:
1. Reproduce a recent task/project from your research using bioLLM.
2. Develop a new tool for bioLLM to access.

In concert, you will test the OpenAI LLM and bioLLM agent ability to generate useful biological results from existing tools. Gaps will be documented and submitted as 

###Hello World Prompts

### PROMPT001,PROMPT002: System information  
In the context of this Palmetto2 "bioLLM" system, please provide an overview of agentic AI. Also save an image of the palmetto2 agent architecture (components + data flow + minimal implementation stack).
What tools are available to you on this Palmetto2 "bioLLM" system?


### PROMPT003: Download human genme data files for local use
PURPOSE:
I want to download genomic input data for humans.  
TASK:  
Please write a SLURM script called 'download-human-genome.slurm' to download key human genome files.  Use genome build hg38. Please use ENSEMBL e.g. 'https://ftp.ensembl.org/pub/release-115/fasta/homo_sapiens/dna/' to download these files and save in a directory called 'human_genome':  
hg38 primary genome assembly   
hg38 cDNA and peptide sequences  
hg38 GTF file  

### PROMPT004: Download human gene idenifier mapping file
PURPOSE:  
I want to download a gene identifier mapping file for humans.  
TASK:  
Please write a SLURM script called 'download-human-gene-translator.slurm' that uses the Biomart API 'https://www.ensembl.org/info/data/biomart/index.html' to write a file called 'human-gene-name-map.csv' in a directory called 'human_genome' with these hese comma-separated fields:  
ENSEMBL gene identifier  
ENSEMBL transcript identifier  
ENSEMBL protein identifier  
Official gene name (e.g. BRCA1)  
chromosome name  
chromosome start   
chromosome stop  

## Issue Framework
FReport issues at issues at https://git.rcd.clemson.edu/biollms/biocodex.  
What LLM model did you use?
What was your prompt 
Paste errors or description of incorrect results.
(optional) Performance metrics 

## Example Computatioanl Biology Workflows
https://github.com/feltus/InSilicoDiseaseHypothesis  
https://github.com/feltus/lab-drug-targeting  
https://github.com/feltus/identifying_differentially_expressed_genes  
https://github.com/feltus/biohackathon-finding-dna-eqtls-underlying-a-disease  

## Rewards 
(1) Early access to Palmetto2 LLM infrastructure with high level tech support.


