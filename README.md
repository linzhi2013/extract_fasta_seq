# extract_fasta_seq

## 1 Introduction


`extract_fasta_seq` is a tool to extract specific fasta sequences from a fasta file. By Guanliang MENG, see https://github.com/linzhi2013/extract_fasta_seq

## 2 Installation

[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/extract_fasta_seq/README.html)

Or with `pip`

    pip install extract_fasta_seq

There will be a command `extract_fasta_seq` created under the same directory as your `pip` command.

## 3 Usage
    
    $ extract_fasta_seq
    usage: extract_fasta_seq.py [-h] [-q <str> [<str> ...]] [-f <query file>]
                                [-s [<subject file>]] [-s1 <pattern>]
                                [-s2 <pattern>] [-d1 [<int>]] [-d2 [<int>]]
                                [-o [<outfile>]] [-v] [-V] [--lazy] [--version]

    To extract specific fasta sequences from a fasta file. By Guanliang MENG, see
    https://github.com/linzhi2013

    optional arguments:
      -h, --help            show this help message and exit
      -q <str> [<str> ...]  query list. "-s1" and "-d1" have no effect on this
                            option.
      -f <query file>       query list file, one line should contain only one
                            queryid! (but can be mixed with others, and we can use
                            "-s1" and "-d1" option to extract the queryid)
      -s [<subject file>]   subject file [stdin]
      -s1 <pattern>         query file sep_pattern [\s+]
      -s2 <pattern>         subject file sep_pattern [\s+]
      -d1 [<int>]           which field in the query_file is to used? [0]
      -d2 [<int>]           which field in the subject_file is to used? useful for
                            finding out all sequences in the subject_file whose
                            seqids equal to the queryids [0]
      -o [<outfile>]        outfile [stdout]
      -v                    invert the output [False]
      -V                    verbose output
      --lazy                Stop searching once each required seqid has at least
                            one sequence found, which can be problems if some
                            required seqids have more than sequences! Works only
                            for non-invert mode. [False]
      --version             show program's version number and exit
        
## 4 Author
Guanliang MENG

## 5 Citation
Currently I have no plan to publish `extract_fasta_seq`.

**However, if you use this program in your analysis, or you "steal" the idea/codes of this program into your script, I should be one of the co-authors in your publication!!!**





