# Required software
Below is a list of essential software tools used in our molecular docking and visualization workflow. Please download and install the versions provided for optimal compatibility.



__1. MGL Tools__ (Molecular Graphics Laboratory)
   🔗 Website: https://ccsb.scripps.edu/mgltools/downloads/   
Version 1.5.7:  https://ccsb.scripps.edu/download/262/  


  
__2. Autodocksuite__ 
   🔗 Website:  https://autodock.scripps.edu/  
(version -4.2.6):  https://autodock.scripps.edu/wp-content/uploads/sites/56/2021/10/autodocksuite-4.2.6.i86Windows.exe  


__3. Avogadro__
   🔗 Website: https://avogadro.cc/  
(version -1.2):  https://sourceforge.net/projects/avogadro/files/avogadro/1.2.0/Avogadro-1.2.0n-win32.exe/download  
  

__4. Open Babel__
   🔗 Website: https://github.com/openbabel/openbabel/releases  
(version -3.1.1): https://github.com/openbabel/openbabel/releases/download/openbabel-3-1-1/OpenBabel-3.1.1-x64.exe  


__5. BIOVIA Discovery Studio Visualizer (Inscription)__
   🔗 Website: https://discover.3ds.com/discovery-studio-visualizer-download  



__6. UCSF Chimera__
   🔗 Website: https://www.cgl.ucsf.edu/chimera/  
(version -1.19-win64): https://www.cgl.ucsf.edu/chimera/cgi-bin/secure/chimera-get.py?file=win64/chimera-1.19-win64.exe  


__Sublime Text__
https://www.sublimetext.com/download_thanks?target=win-x64  
  
__SiteWeb__  
__1)  PubChem (Ligand; molecule)__
https://pubchem.ncbi.nlm.nih.gov/  
  
__2)  RCSB Protein Data Bank (RCSB PDB)__
https://www.rcsb.org/ 


# Exemple  
✾ __1LPB@Luteolin__   
    ♦ (PDB ID: 1LPB) human pancreatic lipase; https://www.rcsb.org/structure/1LPB  
    ♦ Luteolin: https://pubchem.ncbi.nlm.nih.gov/compound/5280445  

# Simple procedure
__1) Preparation Receptor__  
   File ➽ Read Molecule ➽ 1LPB.pdb (open)  
1]	Edit ➽ Delete Water
2]	Edit ➽ Hydrogens  ➽ Add  ➽ Polar Only ("OK")  
3]	Edit ➽ Charges    ➽ Add Kolman Charges  ("OK")  
4]	Edit ➽ Atoms      ➽ Assing AD4 type  ("OK")  
           File ➽ Save ➽ with PDBQT



__2) Preparation ligand__  
1]	Ligand ➽ Input ➽ Open ➽ Choose the  "Ligand.pdb" ➽ "Open  
2]	Ligand ➽ Torsion tree ➽ Selecte Root  
3]	Ligand ➽ Torsion tree ➽ Choose Root  
4]	Ligand ➽ OUTPUT ➽ Save as PDBQT  
            File ➽ Save ➽ with PDBQT

  
__3) ❄ GRID__  
1]	Grid ➽ Macromolecule ➽ Choose ➽ [Choose Macromolecule]  
2]	Grid ➽ Set Map Types ➽ Choose ligand ➽ [Choose Ligand]  
3]	Grid ➽ Grid Box  
4]	Grid ➽ Output ➽ Save GPF  
➽ GPF.gpf  "save"


__4) ❄DOCKING__  
1]	Docking ➽ Macromolecule ➽ set Rigid Filename  
                    ➽ Select "RECEPTOR.pdbqt" & "Open"  
                    ➽ Selecte Ligand & "Select Ligand"  
		   [AutoDpf4 Ligand Parametres] & Accept  
  
2]	Docking ➽ Ligand ➽ Choose
			 [Choose Ligand]  
    3]	Docking ➽ Search Parametres ➽ Genetic Algorithm
					[Geniric Ligand Parametres] & Accept  
     4]	Docking ➽ Ouput ➽ Lamarckian GA(4.2)  
     ➽ Save "DPF.dpf" & "SAVE"

