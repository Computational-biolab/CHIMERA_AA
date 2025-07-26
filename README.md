# CHIMERA_AA: An intergrated Toolkit for protein mutation, minimization,and moleuclar feature analysis. 
Codes for CHIMERA_AA toolkit with separate folders for Chimera and ChimeraX programs are avaialble with thier names
The supplementary_file_AA contains all the test cases along with mutated PDB structures, generated Python files and log files as described in the main study. 
The link to feature extraction Google Colab (Feature_extraction_GC)is (https://colab.research.google.com/drive/1UWqETo1c1eX6uXWxUn3eIY5Q0Gj2UsoJ?usp=sharing).
Details of all included structural and physicochemical features and demonstration of Google Colab with an example can be found in the supplementary file ‘Feature_extraction_GC.pdf’.

Flowchart for running the toolkit in Linux Enviornment
## 1. Mutation
(Users are advised to strictly follow the template as mentioned in the executed file for inputs)
1.	To use CHIMERA_AA  toolkit, user can initialize by selecting either the ChimeraX or Chimera program compatabile commands (separate folders included in the github).
2.	Give execution permission using _chmod +x *_ command and run the CHIMERA_AA.sh script using _./CHIMERA_AA.sh_ command.
3.	Provide details such as PDB ID (for fetching directly from RCSB PDB) or complete local path of file (template displayed in Linux environment during execution), desired output form at (PDB,mmCIF or mol2), the nature of the mutations (single, multiple, or class-wise), residue IDs, chain IDs, new residue/class name (may be referred from the executed file in shell environment) and the output directory path for the generated files with the required mutations (template displayed in Linux environment during execution).
4.	After executing the CHIMERA_AA.sh script, a customized CHIMERA_AA.py Python file is generated with all required commands and ready to be executed in either Chimera or ChimeraX. (Note: There is no change in output files from either case.) 
5.	This file generates the initial structures with desired mutations in the desired format within seconds at the user-specified location in the local system.
## 2. Minimization
1.	Users may further minimize the generated structures by executing minimize.sh script using the command _./minimize.sh_ in the respective folder and entering the path of the folder with generated mutated structure files in the shell file (template displayed in Linux environment during execution). This will generate a separate Python file for each structure executable in the Chimera program.
2.	After running the Python file in the Chimera program, the user needs to manually choose the parameters for minimization when displayed by Chimera and save the structure in the desired format.
## 3. Molecular feature extraction and analysis
After mutation and minimization, the user may run the Feature_extraction_GC file (https://colab.research.google.com/drive/1UWqETo1c1eX6uXWxUn3eIY5Q0Gj2UsoJ?usp=sharing) for the extraction of structural and physicochemical features of protein chains. The feature table of all the structures will be generated and can be downloaded for further analysis.
