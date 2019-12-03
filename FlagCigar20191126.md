1 BAM FLAG value 143: 1+2+4+8+128
    1-read paired (0x1)该序列是成对的paired reads中的一个
    2-read mapped in proper pair (0x2)该序列和参考序列完全匹配，无插入或缺失
    4-read unmapped (0x4)该序列无法比对于参考序列
    8-mate unmapped (0x8)与该序列成对的matepair read没有比对到参考序列上
    128-second in pair (0x80)在paired reads中，该序列是与参考序列比对的第二条

2 BAM FLAG value 99: 1+2+32+64
    1-read paired (0x1)该序列是成对的paired reads中的一个
    2-read mapped in proper pair (0x2)该序列和参考序列完全匹配，无插入或缺失
    32-mate reverse strand (0x20)与该序列成对的matepair read其反向互补序列能够比对到参考序列
    64-first in pair (0x40)在paired reads中，该序列是与参考序列比对的第一条

3 BAM FLAG value 516: 4+512
    4-read unmapped (0x4)该序列无法比对于参考序列
    512-read fails platform/vendor quality checks (0x200)该序列没有通过质量控制

4 BAM FLAG value 2064: 16+2048
    16-read reverse strand (0x10)该序列其反向互补序列能够比对到参考序列
    2048-supplementary alignment (0x800)该序列是补充的比对

5 BAM FLAG value 147: 1+2+16+128
    1-read paired (0x1)该序列是成对的paired reads中的一个
    2-read mapped in proper pair (0x2)该序列和参考序列完全匹配，无插入或缺失
    16-read reverse strand (0x10)该序列其反向互补序列能够比对到参考序列
    128-second in pair (0x80)在paired reads中，该序列是与参考序列比对的第二条

6 BAM CIGAR：14M2D31M
    该序列与参考基因组相比(顺次比对)：14bp匹配，2bp缺失，31bp匹配

7 BAM CIGAR：3S6M1D5M
    该序列与参考基因组相比(顺次比对)：3bp为soft clipping ，6pb匹配，1bp缺失，5bp匹配

8 BAM CIGAR: 6M14N5M
    该序列与参考基因组相比(顺次比对)：6bp匹配，14bp为可变剪接，5bp匹配

9 BAM CIGAR: 7M5D8M2I14M  (小写：7m5d8m2i14m）
    该序列与参考基因组相比(顺次比对)：7bp匹配，5bp缺失，8bp匹配，2bp插入，14bp匹配

10 how long is the read with alignment CIGAR of 7M5D8M2I14M?
    该序列与参考基因组相比(顺次比对)：7bp匹配，5bp缺失，8bp匹配，2bp插入，14bp匹配，故该序列长度：7+8+2+14=31bp
