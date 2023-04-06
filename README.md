# hse_hw3_chromhmm
## Гистоновые метки из UCSC
Name | File
--- | ---
H3K4me2 | wgEncodeBroadHistoneA549H3k04me2Dex100nmAlnRep1.bam
H3K79me2 | wgEncodeBroadHistoneA549H3k79me2Dex100nmAlnRep1.bam
H3K36me3 | wgEncodeBroadHistoneA549H3k36me3Dex100nmAlnRep1.bam
H4K20me1 | wgEncodeBroadHistoneA549H4k20me1Etoh02AlnRep1.bam
H3K9me3 | wgEncodeBroadHistoneA549H3k09me3Etoh02AlnRep1.bam
H3K4me1 | wgEncodeBroadHistoneA549H3k04me1Dex100nmAlnRep1.bam
H3K27ac | wgEncodeBroadHistoneA549H3k27acDex100nmAlnRep1.bam
H3K9ac | wgEncodeBroadHistoneA549H3k09acEtoh02AlnRep1.bam
H3K4me3 | wgEncodeBroadHistoneA549H3k04me3Dex100nmAlnRep1.bam
H3K27me3 | wgEncodeBroadHistoneA549H3k27me3Dex100nmAlnRep1.bam


## таблица из колаба

Клеточная линия | Гистоновая метка | Файл с гистоновой меткой | Файл с контролем
--- | --- | --- | ---
A549 | H3K4me2 | H3K4me2.bam | A549Control.bam
A549 | H3K79me2 | H3K79me2.bam | A549Control.bam
A549 | H3K36me3 | H3K36me3.bam | A549Control.bam
A549 | H4K20me1 | H4K20me1.bam | A549Control.bam
A549 | H3K9me | H3K9me.bam | A549Control.bam
A549 | H3K4me1 | H3K4me1.bam | A549Control.bam
A549 | H3K27ac | H3K27ac.bam | A549Control.bam
A549 | H3K9ac | H3K9ac.bam | A549Control.bam
A549 | H3K4me3 | H3K4me3.bam | A549Control.bam
A549 | H3K27me3 | H3K27me3.bam | A549Control.bam


## Скрины ChromHMM

Emission | Overlap | Transition 
 --- | --- | ---
![Image](/data/emissions_15.png) | ![Image](/data/A549_15_overlap.png) | ![Image](/data/transitions_15.png)

RefSeqTES | RefSeqTSS
 --- | --- 
![Image](/data/A549_15_RefSeqTES_neighborhood.png) | ![Image](/data/A549_15_RefSeqTSS_neighborhood.png)


## Придумка названий
№ | Название | Объяснение | Скрин
 --- | --- | ---| ---
1 | Active Promoter | </li><li> Попадает на интрон или экзон </li> | ![Image](/data/state_1.png)
2 | Weak enhancer/Weak transcribed | </li><li> Чаще всего находятся на RefSeqTES, RefSeqGene, а также на ядерной ламине </li><li> Попадает на интрон </li> | ![Image](/data/state_2.png)
3 | Strong enhancer/Transcriptional elogation | </li><li> Чаще всего находятся на RefSeqTES и RefSeqTSS2Kb, а также на ядерной ламине </li><li> Попадает на интрон </li> | ![Image](/data/state_3.png)
4 | Active Promoter | </li><li> Чаще всего находятся на CpGIslands, RefSeqTES </li><li> Попадает на интрон или экзон </li> | ![Image](/data/state_4.png)
5 | Active Promoter | </li><li> Чаще всего находятся на RefSeqTES и RefSeqTSS2Kb, а также на RefSeqGene </li><li> Попадает на интрон или экзон </li> | ![Image](/data/state_5.png)
6 | Weak enhancer | </li><li> Чаще всего находятся на RefSeqGene и RefSeqTES </li><li> Попадает на интрон </li> | ![Image](/data/state_6.png)
7 | Weak enhancer | <ul><li> Чаще всего находятся на RefSeqTES </li><li> Попадает на интрон </li> | ![Image](/data/state_7.png)
8 | Weak enhancer | <ul><li> Чаще всего находятся на RefSeqTES, а также на ядерной ламине, но реже </li><li> Попадает на интрон </li> | ![Image](/data/state_8.png)
9 | Weak enhancer | </li><li> Чаще всего находятся на RefSeqGene, а также RefSeqTES и RefSeqExon, но реже </li><li> Попадает на интрон </li> | ![Image](/data/state_9.png)
10 | Weak transcribed | </li><li> Чаще всего находятся на RefSeqGene </li><li> Попадает на экзон или интрон </li> | ![Image](/data/state_10.png)
11 | Weak transcribed | </li><li> Чаще всего находятся на RefSeqGene </li><li> Попадает на экзон или интрон </li> | ![Image](/data/state_11.png)
12 | Weak transcribed | <ul><li> Чаще всего находятся на RefSeqGene </li><li> Попадает на экзон или интрон </li> | ![Image](/data/state_12.png)
13 | Repressed | <ul><li> Чаще всего находятся на ядерной ламине, то есть попадает на участок репрессированного гетерохроматима </li><li> Не попадает на ген </li> | ![Image](/data/state_13.png)
14 | Heterochromatin | </li><li> Чаще всего находятся на ядерной ламине, то есть попадает на участок репрессированного гетерохроматима </li><li> Не попадает на ген </li> | ![Image](/data/state_14.png)
15 | Heterochromatin | </li><li> Чаще всего находятся на ядерной ламине, то есть попадает на участок репрессированного гетерохроматима </li><li> Не попадает на ген </li> | ![Image](/data/state_15.png)

