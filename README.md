# Virtual-2D-protein-gel
Get Virtual 2D Gel on http://www.jvirgel.de/ automatically

1. Download protein fasta files form NCBI  
    Excute "Download_Protein_from_NCBI.exe"  
    Input protein's accession number and will find it on NCBI (Database: Protein)

    ```
    Search from NCBI, database:Protein

    #1 Input Accession: EPE32547.1
    Searching EPE32547.1......
    Save as EPE32547.1.fas

    #2 Input Accession: NP_001162128.1
    Searching NP_001162128.1......
    Save as NP_001162128.1.fas
   
    #3 Input Accession: gslgnbsldkgn
    Searching gslgnbsldkgn......
    ERROR: Can't find gslgnbsldkgn
    ```
 
    In this case, Download_Protein_from_NCBI.exe will only generate 3 files,  
    EPE32547.1.fas,  
    NP_001162128.1.fas,  
    and All_fas.fas file, this is for 2Dgel.exe in next step.
   
2. Get virtual 2D protein gel  
    Results were generated by http://www.jvirgel.de/
   
    2-1. Make sure All_fas.fas exist.
        Generate All_fas.fas file by step 1 automatically, or rename your own file.
        

        Excute "Download_Protein_from_NCBI.exe" first, or name fasta file as "All_fas.fas"

    This error message shows when All_fas.fas doesn't exist.
        
    2-2. Input the path way of "chromedrive.exe"  
            If chromedrive.exe was located in C:\User\user\Desktop
        

        Input chromedriver's path: C:\User\user\Desktop

        
    2-3. Get the picture of 2D gel, and MW and pI.  
            This step will finish automatically.
        

        DevTools listening on ws://127.0.0.1:49738/devtools/browser/322c984d-6518-4c1c-8a0f-0c104eb55a6a
        Paste 2 sequences
        Choose: No signal peptide correction (not recommended)
        Choose: HTML-Version
                   
        Save picture as '2dgel.png'
          
        Get results:
        Name                    MW      pi
        "EPE32547.1"...         91.66   9.74
        "NP_001162128.1"...     22.43   8.82
           
        Save results as "2Dgel_result.txt"
        === Finish ===
        
3. Path of Output files
    All files will output to "output" folder.
        
