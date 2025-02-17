# 3K rice Genomes daya


http://oryzasnp.org/

## MSU rice genome assembly and annotation (MSU7/IRGSP1.0)

[Nipponbare reference main page] (http://rice.plantbiology.msu.edu/annotation_pseudo_current.shtml)

### the assembly 

* [Chromosome-ony version omitting ChrSy and ChrUn segments ] (ftp://ftp.plantbiology.msu.edu/pub/data/Eukaryotic_Projects/o_sativa/annotation_dbs/pseudomolecules/version_7.0/all.dir/all.chrs.con)

* [Full versions including ChrSy and ChrUn](ftp://ftp.plantbiology.msu.edu/pub/data/Eukaryotic_Projects/o_sativa/annotation_dbs/pseudomolecules/version_7.0/all.dir/all.con)

* [Proteins](ftp://ftp.plantbiology.msu.edu/pub/data/Eukaryotic_Projects/o_sativa/annotation_dbs/pseudomolecules/version_7.0/all.dir/all.cdna)


### the annotation

* [gff3 file](ftp://ftp.plantbiology.msu.edu/pub/data/Eukaryotic_Projects/o_sativa/annotation_dbs/pseudomolecules/version_7.0/all.dir/all.gff3)

This will remove ChrSy and ChrUn which are unplaced pseudomolecules and sanitize the annotation

```
grep -v 'ChrSy' all.gff3 |grep -v 'ChrUn' |gt gff3 -sort -tidy -retainids -o all.chrs.gff3
```

## Rice SNP-Seek database

[Web interface](http://oryzasnp.org/iric-portal/)
[Download index page](http://oryzasnp-atcg-irri-org.s3-website-ap-southeast-1.amazonaws.com/)

### 990K CoreSNP dataset, called vs Nipponbare MSU7/IRGSP1.0 genome

* [PLINK ped file](https://s3.amazonaws.com/3kricegenome/reduced/NB-core_v4.ped.gz)
* [PLINK map file](https://s3.amazonaws.com/3kricegenome/reduced/NB-core_v4.map.gz)
* [README](https://s3.amazonaws.com/3kricegenome/reduced/990k_3krg-snp-README.txt)

39d8c264feaa75c9ee4c9b59e7d38c074c8d08f1  NB-core_v4.map.gz
17238669e38bc13831d8d78f3c1f7deca48c229d  NB-core_v4.ped.gz

### 3K RG 6.5mio filtSNP Dataset

* [PLINK ped file](https://s3.amazonaws.com/3kricegenome/reduced/3krg_filt_snp_v4.map.gz)
* [PLINK map file](https://s3.amazonaws.com/3kricegenome/reduced/3krg_filt_snp_v4.ped.gz)
* [README](https://s3.amazonaws.com/3kricegenome/reduced/Filt_3krg-snp-README.txt)

