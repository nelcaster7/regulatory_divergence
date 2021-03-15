# regulatory_divergence
This is a repository for scripts used in the research study entitled: Gene expression regulatory divergence between two rice ecotypes exposed under non- and water-stress conditions.
This includes PERL and Linux command line scripts
#Authors: Eric Tsai, Shumin Kao, Li-yu Liu, Nelzo Ereful

#Bioinformatics pipeline

1. Data background 

  Rep1: (ir64, apo, f1)x(control, stress)  bp:38  Q33(quality score type)
  Rep2: (ir64, apo, f1)x(control, stress)  bp:90  Q64(quality score type)

2. Quality control    


  2-1. FastQC
  2-2. FASTX Toolkit

3. Mapping Method: Pseudo Reference

  3-1. download reference          
  3-2.bowtie2 index   
  3-3.bowtie2 mapping
  3-4. Samtools sort  
  3-5. Samtools mpileup     
  3-6. modify reference
  3-7 Pseudo Reference check

4. Mapping Method: SNP call  

   4-1. bowtie2 index & samtools index
   4-2. bowtie2 mapping                                         
   4-3. Samtools sort
   4-4. Samtools mpileup                      
   4-5. SNP call

5. Extract F1 read count & Extract Parent read count

   5-1. extract F1 reac count
   5-2. extract parent read count

6.  eXpress:  gene expression level

   6-1. Original gene expression level of APO, IR64, F1
   6-2. read count of APO IR64 including SNP
   6-3. extract F1 read count

7. Differential expression gene & Allelic imbalance test

















