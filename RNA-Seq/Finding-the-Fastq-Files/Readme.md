# Start Here

There are a lot of different ways that your raw RNA-Seq data can look when you get it back. This depends mostly on who performed the sequencing and on what type of machine. I only know enough about Illumina machines to write a guide about them, so I won't be discussing any other brands of machines here (although fortunately Illumina is the most commonly used right now). 

Starting out with the group that (hopefully) most readers of this guide will fall into: users of the University of Miami sequencing core facility (the one led by Bill Hulme). Our core facility takes the information generated by the sequencing machines and automatically processes it using a program known as CASAVA. This processing step resolves the bases read by the machine for each of the hundreds of millions of reads it generated and de-multiplexes the samples (so multiple samples that were pooled together in the same lane get their reads put in separate fastq files). 
All you have to do with this type of output data is to find the fastq files buried deep within the hard drive they give you. Instructions on how to do that are in the file 'CASAVA-processed output'. 

If you used a different sequencing service (such as a company or a core facility at another university), your output data may or may not look like what is described in the 'CASAVA-processed output' file. If the files you have end with .fastq (or .txt) when uncompressed, open them up with a text editor (best done on whatever computing platform you are going to use to process the data) and see if they conform to the guidelines for a fastq file described here: https://en.wikipedia.org/wiki/FASTQ_format
If your files conform to that format, great! Head on to the section about aligning the reads to the genome.

If you have any other type of files, ask us for help. Its not that this is uncharted territory, its just that there are way too many possibilities for what format your data could be in (and what needs to be done to it) for me to write a comprehensive guide on the subject. 